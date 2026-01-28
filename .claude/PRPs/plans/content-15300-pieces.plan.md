# Feature: Content 15,300 Pieces Production Pipeline

## Summary

Build a content production pipeline to transform 340 SWP3 curriculum files into 15,300 content pieces across 9 formats using NotebookLM and automation tools. The system will track progress via Notion and enable batch processing for scale.

## User Story

As a Content Manager,
I want to transform source curriculum files into multiple content formats,
So that I can maximize the value of knowledge assets and reach more audiences.

## Problem Statement

340 SWP3 curriculum files (347 hours) exist but only in original format. No systematic way to repurpose into multiple content types for different platforms and audiences.

## Solution Statement

Create a Content Production Pipeline with:
1. Source inventory management (340 files tracked)
2. NotebookLM integration for 9 output formats
3. Notion-based tracking system
4. QC workflow with ปลัดซัน review
5. Batch processing capability via n8n

## Metadata

| Field            | Value                                             |
| ---------------- | ------------------------------------------------- |
| Type             | NEW_CAPABILITY                                    |
| Complexity       | HIGH                                              |
| Systems Affected | NotebookLM, Notion, n8n, Google Drive             |
| Dependencies     | NotebookLM API, Notion API, n8n instance          |
| Estimated Tasks  | 12                                                |

---

## UX Design

### Before State
```
┌─────────────────────────────────────────────────────────────────┐
│                        BEFORE STATE                              │
├─────────────────────────────────────────────────────────────────┤
│                                                                  │
│   ┌─────────────┐                                               │
│   │  Google     │                                               │
│   │  Drive      │  ───► 340 files sitting unused                │
│   │  (SWP3)     │                                               │
│   └─────────────┘                                               │
│                                                                  │
│   USER_FLOW: Manual access to files when needed                  │
│   PAIN_POINT: No repurposing, single format, no tracking        │
│   DATA_FLOW: Files → Manual download → Use once → Forget        │
│                                                                  │
└─────────────────────────────────────────────────────────────────┘
```

### After State
```
┌─────────────────────────────────────────────────────────────────┐
│                         AFTER STATE                              │
├─────────────────────────────────────────────────────────────────┤
│                                                                  │
│   ┌─────────┐    ┌──────────┐    ┌─────────┐    ┌──────────┐   │
│   │ Google  │───►│NotebookLM│───►│  9      │───►│ Notion   │   │
│   │ Drive   │    │ Pipeline │    │ Formats │    │ Tracking │   │
│   │ (340)   │    └──────────┘    └─────────┘    └──────────┘   │
│   └─────────┘         │               │              │          │
│                       ▼               ▼              ▼          │
│                  ┌──────────┐   ┌─────────┐   ┌──────────┐     │
│                  │   n8n    │   │   QC    │   │ Publish  │     │
│                  │ Workflow │   │ Review  │   │ Outputs  │     │
│                  └──────────┘   └─────────┘   └──────────┘     │
│                                                                  │
│   USER_FLOW: Select source → Choose formats → Generate → QC     │
│   VALUE_ADD: 340 files × 9 formats = 3,060 pieces per round     │
│   DATA_FLOW: Source → NotebookLM → Formats → QC → Publish       │
│                                                                  │
└─────────────────────────────────────────────────────────────────┘
```

### Interaction Changes
| Location | Before | After | User Impact |
|----------|--------|-------|-------------|
| Source Files | Manual access | Inventory system | Easy selection |
| Content Creation | None | 9 format options | Multi-format output |
| Progress | Unknown | Notion dashboard | Full visibility |
| Quality | Ad-hoc | QC workflow | Consistent quality |

---

## Mandatory Reading

**CRITICAL: Team MUST review these before starting:**

| Priority | Resource | Why Read This |
|----------|----------|---------------|
| P0 | NotebookLM Documentation | Understand capabilities & limits |
| P0 | SWP3 File Inventory | Know the source material |
| P1 | n8n Workflow Guide | Automation setup |
| P1 | Notion API Docs | Tracking integration |

---

## Files/Systems to Setup

| Item | Action | Justification |
|------|--------|---------------|
| `Notion Database: Content Inventory` | CREATE | Track all 15,300 pieces |
| `Notion Database: Source Files` | CREATE | Track 340 source files |
| `n8n Workflow: Content Generator` | CREATE | Automation pipeline |
| `Google Drive: Output Folders` | CREATE | Store generated content |
| `QC Checklist per Format` | CREATE | Quality standards |

---

## NOT Building (Scope Limits)

Explicit exclusions to prevent scope creep:

- Real-time publishing (batch only)
- New content from scratch (source-based only)
- Custom UI/app (use Notion + n8n)
- AI training/fine-tuning
- Multi-language translation (Thai only first)

---

## Step-by-Step Tasks

Execute in order. Each task is atomic and independently verifiable.

### Task 1: CREATE Source File Inventory

- **ACTION**: Create Notion database with all 340 SWP3 files
- **IMPLEMENT**: Fields: Title, Duration, File Type, Drive Link, Status
- **OWNER**: จูล่ง
- **VALIDATE**: Count = 340, all links working

### Task 2: CREATE Content Output Database

- **ACTION**: Create Notion database for tracking outputs
- **IMPLEMENT**: Fields: Source, Format, Status, Quality Score, Reviewer, Publish Date
- **OWNER**: จูล่ง
- **VALIDATE**: Relations to Source inventory working

### Task 3: CREATE 9 Format Templates

- **ACTION**: Define template/prompt for each format
- **IMPLEMENT**:
  - Audio Overview prompt
  - Video Summary prompt
  - Mind Map structure
  - Report template
  - Flashcards format
  - Quiz format
  - Infographic outline
  - Slides structure
  - Data Table schema
- **OWNER**: กุนซือ + ปลัดซัน
- **VALIDATE**: Each template tested on 1 source file

### Task 4: CREATE QC Checklists

- **ACTION**: Quality checklist per format type
- **IMPLEMENT**: 5-10 criteria per format
- **OWNER**: ปลัดซัน
- **VALIDATE**: Checklists documented, team trained

### Task 5: SETUP NotebookLM Workflow

- **ACTION**: Document manual NotebookLM process
- **IMPLEMENT**: Step-by-step guide with screenshots
- **OWNER**: จูล่ง
- **VALIDATE**: Process repeatable by any team member

### Task 6: CREATE n8n Workflow - Source Tracker

- **ACTION**: Workflow to sync Drive files with Notion
- **IMPLEMENT**: Trigger: Schedule (daily), Action: Update inventory
- **OWNER**: จูล่ง
- **VALIDATE**: Notion reflects Drive state

### Task 7: CREATE n8n Workflow - Progress Reporter

- **ACTION**: Workflow to generate progress reports
- **IMPLEMENT**: Daily summary to team channel
- **OWNER**: จูล่ง
- **VALIDATE**: Report accurate and timely

### Task 8: PILOT - Generate 10 pieces

- **ACTION**: Test full pipeline with 10 source files
- **IMPLEMENT**: 1 source × 9 formats + 1 additional
- **OWNER**: All
- **VALIDATE**: 10 pieces created, QC'd, tracked

### Task 9: PILOT REVIEW - Adjust process

- **ACTION**: Review pilot results, fix issues
- **IMPLEMENT**: Document learnings, update templates
- **OWNER**: All
- **VALIDATE**: Issues documented in issues/

### Task 10: BATCH - Generate 100 pieces

- **ACTION**: Scale test with 100 pieces
- **IMPLEMENT**: ~11 sources × 9 formats
- **OWNER**: All
- **VALIDATE**: 100 pieces in Notion, 90%+ QC pass

### Task 11: ROUND 1 - Generate 3,060 pieces

- **ACTION**: First full round of production
- **IMPLEMENT**: 340 sources × 9 formats
- **OWNER**: All
- **VALIDATE**: Notion shows 3,060 tracked

### Task 12: DOCUMENTATION - Process Guide

- **ACTION**: Complete process documentation
- **IMPLEMENT**: Runbook for ongoing production
- **OWNER**: ปลัดซัน
- **VALIDATE**: New team member can follow

---

## Testing Strategy

### Validation Checkpoints

| Checkpoint | Test | Pass Criteria |
|------------|------|---------------|
| Inventory | Count source files | 340 files tracked |
| Templates | Test each format | All 9 produce valid output |
| QC | Review sample | Checklist covers all issues |
| Automation | Run n8n workflows | No errors, correct data |
| Scale | Batch 100 | 90%+ success rate |

### Edge Cases Checklist

- [ ] Source file missing from Drive
- [ ] NotebookLM rate limit hit
- [ ] Format generation fails
- [ ] QC reviewer unavailable
- [ ] Notion API timeout
- [ ] Duplicate content detection

---

## Validation Commands

### Level 1: INVENTORY_CHECK
```bash
# Verify Notion database has correct count
# Should show 340 source files
```

### Level 2: FORMAT_TEST
```bash
# Test each of 9 formats with 1 source
# All should produce valid output
```

### Level 3: PIPELINE_TEST
```bash
# Run full pipeline for 10 pieces
# Check: Created → QC'd → Tracked
```

### Level 4: SCALE_TEST
```bash
# Run for 100 pieces
# Success rate >= 90%
```

---

## Acceptance Criteria

- [ ] 340 source files inventoried in Notion
- [ ] 9 format templates created and tested
- [ ] QC checklist per format documented
- [ ] n8n workflows operational
- [ ] Pilot (10) completed successfully
- [ ] Batch (100) achieves 90%+ success
- [ ] Process documented for team

---

## Completion Checklist

- [ ] Task 1-4: Setup complete
- [ ] Task 5-7: Automation ready
- [ ] Task 8-9: Pilot passed
- [ ] Task 10: Batch validated
- [ ] Task 11: Round 1 started
- [ ] Task 12: Documentation done

---

## Risks and Mitigations

| Risk | Likelihood | Impact | Mitigation |
|------|------------|--------|------------|
| NotebookLM limits | MEDIUM | HIGH | Batch scheduling, rate limits |
| Quality variance | MEDIUM | MEDIUM | QC process, templates |
| Time underestimate | HIGH | MEDIUM | Parallel processing, automation |
| Team bandwidth | MEDIUM | HIGH | Clear ownership, priorities |

---

## Notes

**Key Decisions:**
1. Use Notion over custom app - faster to implement, team familiar
2. Manual NotebookLM first, automate later - understand process before scaling
3. QC before publish - quality over speed

**Future Enhancements:**
- Auto-publishing to platforms
- AI quality scoring
- Multi-language support
- Analytics dashboard

---

> **สามประสานจึงไร้พ่าย!** 🚩

*Plan created using /prp-plan command*
*Pink Castle Foundation Kit v1.0*
