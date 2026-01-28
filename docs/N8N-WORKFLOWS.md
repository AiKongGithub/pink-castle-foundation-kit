# n8n Automation Workflows

> **Version:** 1.0
> **Last Updated:** 2026-01-28
> **Project:** Content 15,300 - Pink Castle Foundation Kit
> **n8n Instance:** localhost:5678 (Docker)

---

## Overview

เอกสารนี้อธิบาย n8n workflows สำหรับ automate กระบวนการผลิต content 15,300 ชิ้น รวมถึง integration กับ Notion, file management, และ status tracking

### Architecture

```
┌─────────────────────────────────────────────────────────────────────┐
│                    CONTENT PIPELINE AUTOMATION                       │
├─────────────────────────────────────────────────────────────────────┤
│                                                                      │
│  ┌─────────┐     ┌─────────┐     ┌─────────┐     ┌─────────┐       │
│  │ Notion  │────►│   n8n   │────►│ Storage │────►│ Notify  │       │
│  │Database │     │Workflows│     │(G.Drive)│     │(Slack)  │       │
│  └─────────┘     └─────────┘     └─────────┘     └─────────┘       │
│       │               │                               │             │
│       │               │                               │             │
│       ▼               ▼                               ▼             │
│  - Source files   - Process      - Archive       - Status          │
│  - Status track   - Transform    - Organize      - Alerts          │
│  - QC workflow    - Trigger      - Backup        - Reports         │
│                                                                      │
└─────────────────────────────────────────────────────────────────────┘
```

---

## Workflow Catalog

### Active Workflows

| ID | Workflow Name | Trigger | Purpose |
|----|---------------|---------|---------|
| WF-01 | Content Status Sync | Notion Trigger | Sync status changes to tracking |
| WF-02 | Daily Progress Report | Schedule (Daily) | Generate daily production report |
| WF-03 | QC Review Reminder | Schedule (Hourly) | Remind pending QC items |
| WF-04 | File Organization | Manual/Webhook | Organize completed files |
| WF-05 | Batch Status Update | HTTP Webhook | Bulk update content status |

### Planned Workflows

| ID | Workflow Name | Trigger | Purpose |
|----|---------------|---------|---------|
| WF-06 | NotebookLM Monitor | Schedule | Check NotebookLM progress |
| WF-07 | Export Automation | Webhook | Auto-export completed content |
| WF-08 | Analytics Dashboard | Schedule (Weekly) | Generate weekly analytics |

---

## WF-01: Content Status Sync

### Purpose
ซิงค์สถานะจาก Notion Database เมื่อมีการเปลี่ยนแปลง

### Workflow Diagram

```
┌────────────────┐     ┌────────────────┐     ┌────────────────┐
│ Notion Trigger │────►│ Transform Data │────►│ Update Tracking│
│ (Page Updated) │     │    (Code)      │     │   (Notion)     │
└────────────────┘     └────────────────┘     └────────────────┘
                                                      │
                                                      ▼
                                              ┌────────────────┐
                                              │ Send Slack     │
                                              │ Notification   │
                                              └────────────────┘
```

### Configuration

```json
{
  "name": "WF-01: Content Status Sync",
  "nodes": [
    {
      "name": "Notion Trigger",
      "type": "n8n-nodes-base.notionTrigger",
      "parameters": {
        "databaseId": "42f92631baf341f8a52dabf77f7e1327",
        "event": "pageUpdated",
        "pollTimes": {
          "item": [{"mode": "everyMinute", "minute": 5}]
        }
      }
    },
    {
      "name": "Transform Status",
      "type": "n8n-nodes-base.code",
      "parameters": {
        "jsCode": "const statusMap = {\n  'Draft': { emoji: '📝', priority: 1 },\n  'In Progress': { emoji: '🔄', priority: 2 },\n  'Review': { emoji: '🔍', priority: 3 },\n  'Published': { emoji: '✅', priority: 4 }\n};\n\nconst item = $input.first();\nconst status = item.json.properties.Status?.select?.name || 'Unknown';\nconst title = item.json.properties.Title?.title[0]?.plain_text || 'Untitled';\n\nreturn [{\n  json: {\n    title,\n    status,\n    ...statusMap[status],\n    timestamp: new Date().toISOString()\n  }\n}];"
      }
    },
    {
      "name": "Slack Notification",
      "type": "n8n-nodes-base.slack",
      "parameters": {
        "channel": "#content-production",
        "text": "{{$json.emoji}} *{{$json.title}}* → {{$json.status}}"
      }
    }
  ]
}
```

---

## WF-02: Daily Progress Report

### Purpose
สร้างรายงานความคืบหน้าประจำวันและส่งให้ทีม

### Workflow Diagram

```
┌────────────────┐     ┌────────────────┐     ┌────────────────┐
│    Schedule    │────►│ Query Notion   │────►│ Calculate      │
│  (9:00 AM)     │     │   Database     │     │   Statistics   │
└────────────────┘     └────────────────┘     └────────────────┘
                                                      │
                       ┌────────────────┐             │
                       │ Format Report  │◄────────────┘
                       │   (Markdown)   │
                       └────────────────┘
                              │
              ┌───────────────┼───────────────┐
              ▼               ▼               ▼
       ┌───────────┐   ┌───────────┐   ┌───────────┐
       │   Slack   │   │   Email   │   │  Notion   │
       │  Message  │   │  Summary  │   │  Update   │
       └───────────┘   └───────────┘   └───────────┘
```

### Configuration

```json
{
  "name": "WF-02: Daily Progress Report",
  "nodes": [
    {
      "name": "Daily 9AM",
      "type": "n8n-nodes-base.scheduleTrigger",
      "parameters": {
        "rule": {
          "interval": [{"field": "cronExpression", "expression": "0 9 * * *"}]
        }
      }
    },
    {
      "name": "Query Content DB",
      "type": "n8n-nodes-base.notion",
      "parameters": {
        "operation": "getAll",
        "databaseId": "42f92631baf341f8a52dabf77f7e1327",
        "returnAll": true
      }
    },
    {
      "name": "Calculate Stats",
      "type": "n8n-nodes-base.code",
      "parameters": {
        "jsCode": "const items = $input.all();\n\nconst stats = {\n  total: items.length,\n  draft: 0,\n  inProgress: 0,\n  review: 0,\n  published: 0,\n  today: 0\n};\n\nconst today = new Date().toDateString();\n\nitems.forEach(item => {\n  const status = item.json.properties.Status?.select?.name;\n  const updated = new Date(item.json.last_edited_time).toDateString();\n  \n  if (status === 'Draft') stats.draft++;\n  if (status === 'In Progress') stats.inProgress++;\n  if (status === 'Review') stats.review++;\n  if (status === 'Published') stats.published++;\n  if (updated === today) stats.today++;\n});\n\nstats.progress = Math.round((stats.published / stats.total) * 100);\n\nreturn [{ json: stats }];"
      }
    },
    {
      "name": "Format Report",
      "type": "n8n-nodes-base.code",
      "parameters": {
        "jsCode": "const s = $input.first().json;\nconst date = new Date().toLocaleDateString('th-TH');\n\nconst report = `\n📊 *Daily Progress Report - ${date}*\n\n*Overall Progress:* ${s.progress}%\n\n📝 Draft: ${s.draft}\n🔄 In Progress: ${s.inProgress}\n🔍 Review: ${s.review}\n✅ Published: ${s.published}\n\n*Today's Activity:* ${s.today} items updated\n*Total Items:* ${s.total}\n`;\n\nreturn [{ json: { report, ...s } }];"
      }
    }
  ]
}
```

---

## WF-03: QC Review Reminder

### Purpose
เตือน ปลัดซัน เมื่อมี content รอ review

### Workflow Diagram

```
┌────────────────┐     ┌────────────────┐     ┌────────────────┐
│    Schedule    │────►│ Query Pending  │────►│   Filter >     │
│ (Every Hour)   │     │    Reviews     │     │   24 Hours     │
└────────────────┘     └────────────────┘     └────────────────┘
                                                      │
                                                      ▼
                                              ┌────────────────┐
                                              │ IF has items   │
                                              └────────────────┘
                                                      │
                                           ┌──────────┴──────────┐
                                           ▼                     ▼
                                    ┌───────────┐         ┌───────────┐
                                    │   Send    │         │   Skip    │
                                    │ Reminder  │         │           │
                                    └───────────┘         └───────────┘
```

### Configuration

```json
{
  "name": "WF-03: QC Review Reminder",
  "nodes": [
    {
      "name": "Hourly Check",
      "type": "n8n-nodes-base.scheduleTrigger",
      "parameters": {
        "rule": {
          "interval": [{"field": "hours", "hoursInterval": 1}]
        }
      }
    },
    {
      "name": "Query Pending Reviews",
      "type": "n8n-nodes-base.notion",
      "parameters": {
        "operation": "getAll",
        "databaseId": "42f92631baf341f8a52dabf77f7e1327",
        "filterType": "manual",
        "filters": {
          "and": [
            {
              "property": "Status",
              "select": {"equals": "Review"}
            },
            {
              "property": "QC Status",
              "select": {"equals": "Pending"}
            }
          ]
        }
      }
    },
    {
      "name": "Filter Old Items",
      "type": "n8n-nodes-base.code",
      "parameters": {
        "jsCode": "const items = $input.all();\nconst now = new Date();\nconst oneDay = 24 * 60 * 60 * 1000;\n\nconst oldItems = items.filter(item => {\n  const created = new Date(item.json.created_time);\n  return (now - created) > oneDay;\n});\n\nreturn oldItems.map(item => ({\n  json: {\n    title: item.json.properties.Title?.title[0]?.plain_text,\n    hours: Math.round((now - new Date(item.json.created_time)) / (60 * 60 * 1000)),\n    url: item.json.url\n  }\n}));"
      }
    },
    {
      "name": "Has Items?",
      "type": "n8n-nodes-base.if",
      "parameters": {
        "conditions": {
          "number": [{"value1": "={{$json.length}}", "operation": "larger", "value2": 0}]
        }
      }
    },
    {
      "name": "Send Reminder",
      "type": "n8n-nodes-base.slack",
      "parameters": {
        "channel": "#qc-reviews",
        "text": "⚠️ *QC Review Reminder*\n\nItems waiting >24 hours:\n{{$json.map(i => `• ${i.title} (${i.hours}h)`).join('\\n')}}"
      }
    }
  ]
}
```

---

## WF-04: File Organization

### Purpose
จัดระเบียบไฟล์ที่ผลิตเสร็จแล้วตาม folder structure

### Workflow Diagram

```
┌────────────────┐     ┌────────────────┐     ┌────────────────┐
│    Webhook     │────►│  Parse File    │────►│ Determine      │
│ (New File)     │     │   Metadata     │     │  Destination   │
└────────────────┘     └────────────────┘     └────────────────┘
                                                      │
                                                      ▼
                                              ┌────────────────┐
                                              │ Move to Folder │
                                              │  (G. Drive)    │
                                              └────────────────┘
                                                      │
                                                      ▼
                                              ┌────────────────┐
                                              │ Update Notion  │
                                              │   (File Link)  │
                                              └────────────────┘
```

### Folder Structure

```
Google Drive/
└── Content-15300/
    ├── Sources/
    │   └── SWP3-Transcripts/
    │       ├── Ch01/
    │       ├── Ch02/
    │       └── ...
    ├── Production/
    │   ├── Audio/
    │   ├── Video-Scripts/
    │   ├── Mind-Maps/
    │   ├── Reports/
    │   ├── Flashcards/
    │   ├── Quizzes/
    │   ├── Infographics/
    │   ├── Slides/
    │   └── Data-Tables/
    ├── QC-Approved/
    │   └── [Same structure as Production]
    └── Archives/
        └── NotebookLM-Exports/
```

### Configuration

```json
{
  "name": "WF-04: File Organization",
  "nodes": [
    {
      "name": "Webhook Trigger",
      "type": "n8n-nodes-base.webhook",
      "parameters": {
        "path": "file-organization",
        "httpMethod": "POST"
      }
    },
    {
      "name": "Parse Metadata",
      "type": "n8n-nodes-base.code",
      "parameters": {
        "jsCode": "const { filename, format, chapter, status } = $input.first().json;\n\nconst formatFolders = {\n  'audio': 'Audio',\n  'video': 'Video-Scripts',\n  'mindmap': 'Mind-Maps',\n  'report': 'Reports',\n  'flashcards': 'Flashcards',\n  'quiz': 'Quizzes',\n  'infographic': 'Infographics',\n  'slides': 'Slides',\n  'datatable': 'Data-Tables'\n};\n\nconst baseFolder = status === 'Approved' ? 'QC-Approved' : 'Production';\nconst destination = `Content-15300/${baseFolder}/${formatFolders[format]}/Ch${chapter.padStart(2, '0')}/`;\n\nreturn [{\n  json: {\n    filename,\n    destination,\n    format,\n    chapter\n  }\n}];"
      }
    },
    {
      "name": "Move File",
      "type": "n8n-nodes-base.googleDrive",
      "parameters": {
        "operation": "move",
        "fileId": "={{$json.fileId}}",
        "folderId": "={{$json.destinationFolderId}}"
      }
    },
    {
      "name": "Update Notion",
      "type": "n8n-nodes-base.notion",
      "parameters": {
        "operation": "update",
        "pageId": "={{$json.notionPageId}}",
        "properties": {
          "File Link": {
            "url": "={{$json.fileUrl}}"
          }
        }
      }
    }
  ]
}
```

---

## WF-05: Batch Status Update

### Purpose
อัพเดทสถานะหลายรายการพร้อมกัน ผ่าน API

### API Endpoint

```
POST http://localhost:5678/webhook/batch-status-update
Content-Type: application/json

{
  "items": [
    {"pageId": "xxx", "status": "Review"},
    {"pageId": "yyy", "status": "Published"}
  ],
  "updatedBy": "จูล่ง"
}
```

### Workflow Diagram

```
┌────────────────┐     ┌────────────────┐     ┌────────────────┐
│    Webhook     │────►│  Split Items   │────►│   Loop Each    │
│ (Batch Data)   │     │                │     │    Item        │
└────────────────┘     └────────────────┘     └────────────────┘
                                                      │
                                                      ▼
                                              ┌────────────────┐
                                              │ Update Notion  │
                                              │    Page        │
                                              └────────────────┘
                                                      │
                                                      ▼
                                              ┌────────────────┐
                                              │ Log Results    │
                                              └────────────────┘
```

### Configuration

```json
{
  "name": "WF-05: Batch Status Update",
  "nodes": [
    {
      "name": "Webhook",
      "type": "n8n-nodes-base.webhook",
      "parameters": {
        "path": "batch-status-update",
        "httpMethod": "POST",
        "responseMode": "responseNode"
      }
    },
    {
      "name": "Split Items",
      "type": "n8n-nodes-base.splitInBatches",
      "parameters": {
        "batchSize": 1,
        "options": {}
      }
    },
    {
      "name": "Update Notion",
      "type": "n8n-nodes-base.notion",
      "parameters": {
        "operation": "update",
        "pageId": "={{$json.pageId}}",
        "properties": {
          "Status": {
            "select": {"name": "={{$json.status}}"}
          }
        }
      }
    },
    {
      "name": "Collect Results",
      "type": "n8n-nodes-base.code",
      "parameters": {
        "jsCode": "const results = $input.all();\nconst success = results.filter(r => !r.json.error).length;\nconst failed = results.length - success;\n\nreturn [{\n  json: {\n    total: results.length,\n    success,\n    failed,\n    timestamp: new Date().toISOString()\n  }\n}];"
      }
    },
    {
      "name": "Response",
      "type": "n8n-nodes-base.respondToWebhook",
      "parameters": {
        "respondWith": "json",
        "responseBody": "={{$json}}"
      }
    }
  ]
}
```

---

## Integration Points

### Notion Database

**Database ID:** `42f92631baf341f8a52dabf77f7e1327`

**Required Properties for Automation:**

| Property | Type | Used By |
|----------|------|---------|
| Title | title | All workflows |
| Status | select | WF-01, WF-02, WF-05 |
| QC Status | select | WF-03 |
| Chapter | select | WF-04 |
| Format | multi_select | WF-04 |
| File Link | url | WF-04 |
| Due Date | date | WF-03 |
| Assigned To | people | WF-03 |

### Slack Channels

| Channel | Purpose | Used By |
|---------|---------|---------|
| #content-production | General updates | WF-01, WF-02 |
| #qc-reviews | QC notifications | WF-03 |
| #alerts | Critical issues | All |

### Google Drive

**Root Folder:** `Content-15300`
**Service Account:** Required for automation

---

## Exportable Templates

### Import Instructions

1. Copy JSON configuration
2. In n8n, go to **Workflows** → **Import from JSON**
3. Paste and import
4. Update credentials:
   - Notion API token
   - Slack Bot token
   - Google Drive service account
5. Activate workflow

### Credentials Required

| Service | Credential Type | Notes |
|---------|-----------------|-------|
| Notion | API Token | Internal integration |
| Slack | Bot Token | With chat:write scope |
| Google Drive | Service Account | JSON key file |

---

## Monitoring & Debugging

### Execution Logs

```bash
# View recent executions
curl http://localhost:5678/api/v1/executions

# View specific execution
curl http://localhost:5678/api/v1/executions/{id}
```

### Common Issues

| Issue | Cause | Solution |
|-------|-------|----------|
| Notion trigger not firing | Rate limit | Increase poll interval |
| Slack message fails | Token expired | Refresh OAuth token |
| File not found | Wrong path | Verify folder IDs |
| Timeout | Large batch | Reduce batch size |

### Health Checks

```bash
# Check n8n status
curl http://localhost:5678/healthz

# Check workflow status
curl http://localhost:5678/api/v1/workflows
```

---

## Usage Examples

### Example 1: Update Single Item Status

```bash
curl -X POST http://localhost:5678/webhook/batch-status-update \
  -H "Content-Type: application/json" \
  -d '{
    "items": [{"pageId": "abc123", "status": "Review"}],
    "updatedBy": "จูล่ง"
  }'
```

### Example 2: Trigger File Organization

```bash
curl -X POST http://localhost:5678/webhook/file-organization \
  -H "Content-Type: application/json" \
  -d '{
    "filename": "SWP3-Ch09-audio-20260128.wav",
    "format": "audio",
    "chapter": "9",
    "status": "Pending"
  }'
```

### Example 3: Manual Progress Report

```bash
curl -X POST http://localhost:5678/webhook/manual-report
```

---

## Roadmap

### Phase 2 (Current)
- [x] WF-01: Content Status Sync
- [x] WF-02: Daily Progress Report
- [x] WF-03: QC Review Reminder
- [x] WF-04: File Organization
- [x] WF-05: Batch Status Update

### Phase 3 (Future)
- [ ] WF-06: NotebookLM progress monitoring
- [ ] WF-07: Auto-export to final destinations
- [ ] WF-08: Weekly analytics dashboard
- [ ] WF-09: Automated backup workflow
- [ ] WF-10: Error alerting system

---

## Tags

`#n8n` `#automation` `#workflow` `#notion` `#integration`

---

> *Pink Castle Foundation Kit v1.0*
> *n8n Automation Workflows - Content 15,300 Project*
