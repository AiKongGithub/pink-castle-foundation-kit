# Production Pipeline - Content 15,300 Project

> **Version:** 1.0
> **Last Updated:** 2026-01-28
> **Phase:** 3 - Content Production
> **Status:** Active

---

## Overview

เอกสารนี้กำหนดกระบวนการผลิต content แบบ batch processing สำหรับโครงการ Content 15,300 ชิ้น ครอบคลุม workflow, tracking, naming conventions, และ folder structure

---

## Production Workflow

### High-Level Flow

```
┌─────────────────────────────────────────────────────────────────────┐
│                    PRODUCTION PIPELINE                               │
├─────────────────────────────────────────────────────────────────────┤
│                                                                      │
│  ┌─────────┐   ┌─────────┐   ┌─────────┐   ┌─────────┐   ┌───────┐ │
│  │ SELECT  │──►│ PREPARE │──►│ PRODUCE │──►│   QC    │──►│PUBLISH│ │
│  │ Chapter │   │ Sources │   │ Content │   │ Review  │   │ Store │ │
│  └─────────┘   └─────────┘   └─────────┘   └─────────┘   └───────┘ │
│       │             │             │             │             │     │
│       ▼             ▼             ▼             ▼             ▼     │
│   - Priority    - Transcripts  - 9 formats  - Checklist  - Notion  │
│   - Inventory   - NotebookLM   - Templates  - Scoring    - Storage │
│   - Schedule    - Organization - Batch      - Feedback   - Archive │
│                                                                      │
└─────────────────────────────────────────────────────────────────────┘
```

### Detailed Steps

#### Step 1: SELECT Chapter
1. Check production schedule
2. Verify source materials available
3. Review chapter metadata (files, duration)
4. Confirm not already in progress

#### Step 2: PREPARE Sources
1. Gather source files (videos, transcripts)
2. Create/verify transcripts
3. Upload to NotebookLM
4. Create chapter notebook

#### Step 3: PRODUCE Content
1. Generate 9 formats using templates
2. Follow batch processing order
3. Save with proper naming
4. Track time and issues

#### Step 4: QC Review
1. Self-check with QC checklist
2. Submit to ปลัดซัน
3. Receive feedback
4. Fix issues if needed

#### Step 5: PUBLISH & Store
1. Move to approved folder
2. Update Notion database
3. Archive source materials
4. Log completion metrics

---

## Batch Processing

### Batch Structure

```
Batch = 5 Chapters
Chapter = 9 Formats
Format = 1 Content Piece

1 Batch = 5 × 9 = 45 pieces
Full Project = 7 Batches × ~45 = ~315 pieces (core)
              + variations = 15,300 pieces
```

### Batch Schedule

| Batch | Chapters | Priority | Est. Duration |
|-------|----------|----------|---------------|
| 1 | Ch 1-5 | 🔴 HIGH | 1 week |
| 2 | Ch 6-10 | 🔴 HIGH | 1 week |
| 3 | Ch 11-15 | 🟡 MEDIUM | 1 week |
| 4 | Ch 16-20 | 🟡 MEDIUM | 1 week |
| 5 | Ch 21-25 | 🟢 LOW | 1 week |
| 6 | Ch 26-30 | 🟢 LOW | 1 week |
| 7 | Ch 31 | 🟢 LOW | 2 days |

### Batch Processing Order (Per Chapter)

Process formats in this order for efficiency:

| Order | Format | Reason |
|-------|--------|--------|
| 1 | Source Summary | Foundation for all others |
| 2 | Mind Map | Quick, establishes structure |
| 3 | Data Table | Extract facts first |
| 4 | Report | Written analysis |
| 5 | Flashcards | Uses report content |
| 6 | Quiz | Uses flashcard content |
| 7 | Audio Overview | Longest generation |
| 8 | Video Summary | Uses audio script |
| 9 | Infographic | Final visual |
| 10 | Slides | Comprehensive |

---

## Progress Tracking

### Notion Database Integration

**Database ID:** `42f92631baf341f8a52dabf77f7e1327`

#### Required Properties

| Property | Type | Values/Format |
|----------|------|---------------|
| Title | title | `[ChXX] [Format] - [Topic]` |
| Chapter | select | Ch01 - Ch31 |
| Format | select | 9 formats |
| Status | select | Pending, In Progress, Review, Approved, Published |
| Producer | people | จูล่ง |
| QC Reviewer | people | ปลัดซัน |
| Batch | select | Batch 1-7 |
| Created Date | date | Auto |
| Due Date | date | Based on schedule |
| QC Score | number | 1-5 |
| Notes | text | Issues, feedback |
| File Link | url | Google Drive link |

#### Status Workflow

```
Pending → In Progress → Review → Approved → Published
                           ↓
                       Revision → Review
```

### Progress Dashboard (Manual Check)

Weekly tracking template:

```markdown
## Weekly Progress - [Week Number]

### Production Metrics
| Metric | Target | Actual | % |
|--------|--------|--------|---|
| Pieces Produced | 100 | | |
| QC Passed | 80 | | |
| Published | 70 | | |

### By Chapter
| Chapter | Formats Done | Status |
|---------|--------------|--------|
| Ch XX | 9/9 | ✅ Complete |
| Ch XX | 5/9 | 🔄 In Progress |
| Ch XX | 0/9 | ⏳ Pending |

### Issues
- [ ] Issue 1
- [ ] Issue 2

### Next Week Plan
- [ ] Target chapters
- [ ] Target pieces
```

---

## File Naming Convention

### Format

```
SWP3-Ch[XX]-[Format]-[ShortTitle]-v[Version].[ext]
```

### Components

| Component | Format | Example |
|-----------|--------|---------|
| Course | SWP3 | SWP3 |
| Chapter | Ch[XX] (2 digits) | Ch09 |
| Format | Abbreviated | audio, video, mind, rpt, flash, quiz, info, slide, data |
| Title | Short (max 20 chars) | business-ideas |
| Version | v[N] | v1, v2 |
| Extension | Based on format | .md, .json, .mmd |

### Examples

```
SWP3-Ch09-audio-business-ideas-v1.md
SWP3-Ch09-mind-business-ideas-v1.mmd
SWP3-Ch09-quiz-business-ideas-v1.md
SWP3-Ch01-slide-orientation-v1.md
```

### Format Abbreviations

| Format | Abbreviation | Extension |
|--------|--------------|-----------|
| Source Summary | src | .md |
| Audio Overview | audio | .md |
| Video Summary | video | .md |
| Mind Map | mind | .md (.mmd for Mermaid) |
| Report | rpt | .md |
| Flashcards | flash | .md, .csv |
| Quiz | quiz | .md, .json |
| Infographic | info | .md |
| Slides | slide | .md |
| Data Table | data | .md, .csv |

---

## Output Folder Structure

### Main Structure

```
pink-castle-foundation-kit/
├── production/
│   ├── batch-01/
│   │   ├── ch01-orientation/
│   │   ├── ch02-speed-wealth/
│   │   ├── ch03-marketing/
│   │   ├── ch04-workshop-1/
│   │   └── ch05-business-online/
│   ├── batch-02/
│   │   └── ...
│   └── ...
├── approved/
│   ├── audio/
│   ├── video/
│   ├── mind-maps/
│   ├── reports/
│   ├── flashcards/
│   ├── quizzes/
│   ├── infographics/
│   ├── slides/
│   └── data-tables/
├── pilot/
│   └── ch09-business-ideas/  (existing)
└── archives/
    ├── sources/
    └── notebooklm-exports/
```

### Per-Chapter Folder

```
ch01-orientation/
├── SWP3-Ch01-src-orientation-v1.md
├── SWP3-Ch01-audio-orientation-v1.md
├── SWP3-Ch01-video-orientation-v1.md
├── SWP3-Ch01-mind-orientation-v1.md
├── SWP3-Ch01-rpt-orientation-v1.md
├── SWP3-Ch01-flash-orientation-v1.md
├── SWP3-Ch01-quiz-orientation-v1.md
├── SWP3-Ch01-info-orientation-v1.md
├── SWP3-Ch01-slide-orientation-v1.md
├── SWP3-Ch01-data-orientation-v1.md
└── _metadata.json
```

### Metadata File (_metadata.json)

```json
{
  "chapter": 1,
  "title": "ปฐมนิเทศ",
  "english_title": "Orientation",
  "batch": 1,
  "source_files": 1,
  "source_duration": "1:49:00",
  "formats_completed": 9,
  "status": "approved",
  "producer": "จูล่ง",
  "qc_reviewer": "ปลัดซัน",
  "qc_score": 4.5,
  "production_date": "2026-01-29",
  "approval_date": "2026-01-30",
  "notes": ""
}
```

---

## Automation Integration

### n8n Webhooks

| Webhook | URL | Trigger |
|---------|-----|---------|
| Start Production | `/webhook/start-production` | Begin new chapter |
| Update Status | `/webhook/update-status` | Status change |
| Complete Format | `/webhook/complete-format` | Format done |
| Request QC | `/webhook/request-qc` | Submit for review |
| QC Complete | `/webhook/qc-complete` | QC finished |

### Notion Auto-Sync

When file is committed:
1. n8n detects new file (via webhook or polling)
2. Parses filename for metadata
3. Creates/updates Notion page
4. Sets appropriate status

### Status Update Triggers

| Event | Status Change | Notification |
|-------|---------------|--------------|
| File created | → In Progress | Log only |
| All formats done | → Review | Slack: ปลัดซัน |
| QC passed | → Approved | Slack: All |
| QC failed | → Revision | Slack: จูล่ง |
| Published | → Published | Log only |

---

## Quality Gates

### Before Production
- [ ] Source materials verified
- [ ] NotebookLM notebook created
- [ ] Previous chapters complete (if dependent)

### After Each Format
- [ ] Content follows template
- [ ] Naming convention correct
- [ ] File in correct folder
- [ ] Self-QC checklist passed

### Before QC Submission
- [ ] All 9 formats complete
- [ ] Metadata file created
- [ ] Files committed to Git
- [ ] Notion entries created

### Before Publication
- [ ] QC score ≥ 3.5/5
- [ ] All feedback addressed
- [ ] Final files in approved folder
- [ ] Notion status updated

---

## Time Tracking

### Per-Format Benchmarks

| Format | Target | Max |
|--------|--------|-----|
| Source Summary | 15 min | 20 min |
| Mind Map | 15 min | 20 min |
| Data Table | 20 min | 25 min |
| Report | 25 min | 35 min |
| Flashcards | 20 min | 25 min |
| Quiz | 30 min | 40 min |
| Audio Overview | 30 min | 45 min |
| Video Summary | 25 min | 35 min |
| Infographic | 15 min | 20 min |
| Slides | 30 min | 40 min |
| **Total** | **225 min** | **305 min** |

### Per-Chapter Target
- Standard: 4 hours
- Complex: 5 hours
- Maximum: 6 hours

### Weekly Target
- Minimum: 20 chapters = 180 formats
- Target: 25 chapters = 225 formats
- Stretch: 30 chapters = 270 formats

---

## Escalation Process

### When to Escalate

| Situation | Escalate To | Timeline |
|-----------|-------------|----------|
| Source not available | MD กุนซือ | Same day |
| Blocked >24 hours | MD กุนซือ | Next day |
| QC dispute | Chairman | Within 48h |
| Technical failure | Chairman | Immediate |
| Behind schedule >1 week | Chairman | Weekly review |

### Escalation Format

```markdown
## Production Escalation

**Date:** [YYYY-MM-DD]
**Chapter:** [Chapter number]
**Issue:** [Brief description]
**Impact:** [What's blocked]
**Tried:** [What was attempted]
**Need:** [What's needed to resolve]
**Urgency:** Low / Medium / High / Critical
```

---

## Quick Reference

### Daily Checklist

```markdown
## Daily Production Checklist

Morning:
- [ ] Check Notion for assignments
- [ ] Review yesterday's QC feedback
- [ ] Prepare source materials

Production:
- [ ] Complete target formats
- [ ] Update Notion status
- [ ] Commit to Git

Evening:
- [ ] Log time spent
- [ ] Note any blockers
- [ ] Plan tomorrow
```

### Commands

```bash
# Create new chapter folder
mkdir -p production/batch-XX/chXX-[topic]

# Commit chapter
git add production/batch-XX/chXX-*
git commit -m "feat: ChXX - [Topic] - [N] formats complete"

# Push to remote
git push origin main
```

---

## Tags

`#pipeline` `#production` `#workflow` `#batch` `#tracking`

---

> *Pink Castle Foundation Kit v1.0*
> *Production Pipeline - Phase 3*
