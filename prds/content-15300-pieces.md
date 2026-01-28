# Content 15,300 Pieces PRD

# Product Requirements Document

> **Version:** 1.0
> **Author:** จูล่ง (CTO) / กุนซือสุมาอี้ (MD)
> **Date:** 2026-01-28
> **Status:** Draft
> **Approver:** ท่านแม่ทัพ Kong

---

## 🎯 Overview

### What (อะไร)
ระบบสร้างและจัดการคอนเทนต์ 15,300 ชิ้น สำหรับ SWP3 Curriculum ผ่าน NotebookLM และ AI Tools

### Why (ทำไม)
- เปลี่ยน 340 ไฟล์จาก SWP3 Curriculum (347 ชม.) เป็นคอนเทนต์หลากหลายรูปแบบ
- สร้าง Value จาก Knowledge Assets ที่มีอยู่
- ขยาย Reach ผ่านหลาย Platforms และ Formats

### Who (ใคร)
- **Primary:** นักเรียนที่สนใจ Digital Marketing / AI
- **Secondary:** ผู้ประกอบการที่ต้องการเรียนรู้
- **Tertiary:** Content Creators ที่ต้องการ Reference

### When (เมื่อไหร่)
- **Start:** กุมภาพันธ์ 2026
- **Phase 1 Complete:** มีนาคม 2026
- **Full Production:** Q2 2026

---

## 📋 Problem Statement

**Current Situation:**
- มี SWP3 Curriculum 340 ไฟล์ (347 ชม.) ที่ยังไม่ได้ใช้ประโยชน์เต็มที่
- คอนเทนต์อยู่ในรูปแบบเดียว (Video/PDF)
- ไม่มีระบบจัดการ Content Pipeline

**Desired Outcome:**
- แปลง 340 ไฟล์ เป็น 9 รูปแบบ = 3,060 ชิ้นต่อรอบ
- มี Content Pipeline ที่ทำงานอัตโนมัติ
- สร้าง Revenue จาก Content Assets

---

## 🎯 Goals

### Primary Goals (ต้องมี)
1. สร้างระบบ Content Generation Pipeline
2. แปลง SWP3 340 ไฟล์ เป็น 9 รูปแบบ
3. มี Content Management System ติดตามสถานะ

### Secondary Goals (ควรมี)
1. Automation ผ่าน n8n workflows
2. Integration กับ NotebookLM API
3. Analytics Dashboard สำหรับ Performance

### Non-Goals (ไม่ทำ)
1. สร้างคอนเทนต์ใหม่จาก scratch (ใช้ source ที่มีอยู่)
2. Manual content creation (ใช้ AI/Automation)
3. Real-time publishing (batch processing)

---

## 📦 Requirements

### Must Have (P0) - จำเป็น
| # | Requirement | Description | Acceptance Criteria |
|---|-------------|-------------|---------------------|
| 1 | Content Source Management | จัดการ 340 source files จาก SWP3 | มี inventory ครบทุกไฟล์ |
| 2 | 9 Output Formats | Audio, Video, Mind Map, Report, Flashcards, Quiz, Infographic, Slides, Data Table | แต่ละ format มี template |
| 3 | NotebookLM Integration | ใช้ NotebookLM สร้าง outputs | API/Manual workflow defined |
| 4 | Content Tracking | ติดตามสถานะทุก content piece | Dashboard แสดงสถานะ |
| 5 | Quality Control | QC process ก่อน publish | Checklist per format |

### Should Have (P1) - สำคัญ
| # | Requirement | Description | Acceptance Criteria |
|---|-------------|-------------|---------------------|
| 1 | n8n Automation | Workflow อัตโนมัติ | 3+ workflows ทำงานได้ |
| 2 | Batch Processing | ประมวลผลทีละหลาย files | Process 10+ files/batch |
| 3 | Version Control | Track versions ของ content | Git-based versioning |

### Nice to Have (P2) - ดีถ้ามี
| # | Requirement | Description | Acceptance Criteria |
|---|-------------|-------------|---------------------|
| 1 | AI Quality Scoring | ให้คะแนนคุณภาพอัตโนมัติ | Score 1-10 per piece |
| 2 | Auto-Publishing | Push to platforms อัตโนมัติ | 2+ platforms supported |
| 3 | Performance Analytics | Track engagement | Basic metrics dashboard |

---

## 👤 User Stories

### Story 1: Content Generator
```
As a Content Creator,
I want to generate multiple content formats from a single source file,
So that I can maximize the value of existing knowledge assets.
```

**Acceptance Criteria:**
- [ ] Select source file from SWP3 inventory
- [ ] Choose output format(s)
- [ ] Generate content via NotebookLM
- [ ] Review and approve output
- [ ] Track in content management system

### Story 2: Content Manager
```
As a Content Manager,
I want to see the status of all 15,300 content pieces,
So that I can track progress and identify bottlenecks.
```

**Acceptance Criteria:**
- [ ] Dashboard shows total/completed/pending counts
- [ ] Filter by source file, format, status
- [ ] Export reports for stakeholders
- [ ] Identify blocked items

### Story 3: Quality Reviewer
```
As a Quality Reviewer (ปลัดซัน),
I want to review content before publishing,
So that we maintain high quality standards.
```

**Acceptance Criteria:**
- [ ] Queue of items pending review
- [ ] Checklist per format type
- [ ] Approve/Reject with comments
- [ ] Track revision history

---

## 🔄 Content Pipeline Flow

```
[SWP3 Source] → [NotebookLM] → [9 Formats] → [QC Review] → [Publish]
    340 files       │              │              │            │
                    ▼              ▼              ▼            ▼
              Process each    Generate      ปลัดซัน       Platforms
              with prompts    outputs       reviews       (YouTube,
                                                          Blog, etc.)
```

**Flow Description:**
1. **Source Selection:** เลือก source file จาก SWP3 inventory
2. **Format Selection:** เลือก 1-9 formats ที่ต้องการ
3. **Generation:** ใช้ NotebookLM/AI สร้าง content
4. **Quality Control:** ปลัดซัน review ตาม checklist
5. **Publishing:** Push to designated platforms

---

## 🏗️ Technical Approach

### Architecture
```
┌─────────────────────────────────────────────────────────┐
│                   Pink Castle CMS                        │
├─────────────────────────────────────────────────────────┤
│  Source Manager  │  Generator  │  QC System  │ Publisher │
│    (Inventory)   │ (NotebookLM)│  (Review)   │ (Outputs) │
└────────┬─────────┴──────┬──────┴──────┬──────┴─────┬────┘
         │                │             │            │
         ▼                ▼             ▼            ▼
    Google Drive     NotebookLM    Notion DB    Multi-Platform
    (340 files)        API        (Tracking)    (YouTube, Blog)
```

### Technology Stack
| Layer | Technology | Reason |
|-------|------------|--------|
| Source Storage | Google Drive | SWP3 files already there |
| Content Generation | NotebookLM | Best for knowledge synthesis |
| Workflow Automation | n8n | Already integrated with Pink Castle |
| Tracking | Notion Database | Team already uses Notion |
| Publishing | Platform APIs | YouTube, Blog, Social |

### Key Technical Decisions
1. **NotebookLM as primary generator:** Best quality for knowledge content
2. **Notion for tracking:** Single source of truth for status
3. **n8n for automation:** Reduce manual work, scale operations

---

## 📊 9 Content Formats

| # | Format | Description | Output per Source |
|---|--------|-------------|-------------------|
| 1 | Audio Overview | 10-15 min audio summary | 1 |
| 2 | Video Summary | 5-10 min video | 1 |
| 3 | Mind Map | Visual concept map | 1 |
| 4 | Report | Written summary (1-2 pages) | 1 |
| 5 | Flashcards | 10-20 Q&A cards | 1 set |
| 6 | Quiz | 10 questions with answers | 1 set |
| 7 | Infographic | Visual summary | 1 |
| 8 | Slides | Presentation (10-15 slides) | 1 deck |
| 9 | Data Table | Structured data extract | 1 |

**Calculation:**
- 340 source files × 9 formats = **3,060 pieces per round**
- 5 rounds = **15,300 pieces total**

---

## 📊 Success Metrics

| Metric | Current | Target | How to Measure |
|--------|---------|--------|----------------|
| Content pieces created | 0 | 15,300 | Notion tracking |
| Completion rate | 0% | 100% | Dashboard |
| QC pass rate | N/A | 90%+ | Review stats |
| Avg. time per piece | N/A | < 30 min | Time tracking |
| Platform engagement | 0 | TBD | Analytics |

---

## 📅 Timeline

| Phase | Milestone | Date | Owner | Status |
|-------|-----------|------|-------|--------|
| 0 | PRD Approved | 2026-01-31 | กุนซือ | ⬜ |
| 1 | System Setup | 2026-02-07 | จูล่ง | ⬜ |
| 2 | Pilot (100 pieces) | 2026-02-14 | All | ⬜ |
| 3 | Round 1 (3,060) | 2026-02-28 | All | ⬜ |
| 4 | Round 2-3 (6,120) | 2026-03-31 | All | ⬜ |
| 5 | Round 4-5 (6,120) | 2026-04-30 | All | ⬜ |
| 6 | Complete (15,300) | 2026-04-30 | All | ⬜ |

---

## 🔗 Dependencies

### External Dependencies
| Dependency | Provider | Status | Risk |
|------------|----------|--------|------|
| NotebookLM API | Google | Available | Low |
| Google Drive Access | Google | ✅ Ready | Low |
| n8n Instance | Self-hosted | ✅ Ready | Low |

### Internal Dependencies
| Dependency | Team | Status |
|------------|------|--------|
| SWP3 File Inventory | กุนซือ | ✅ Complete (340 files) |
| Notion Database Setup | จูล่ง | ⬜ Pending |
| QC Checklist per Format | ปลัดซัน | ⬜ Pending |

---

## ⚠️ Risks

| Risk | Likelihood | Impact | Mitigation |
|------|------------|--------|------------|
| NotebookLM rate limits | Medium | High | Batch processing, schedule |
| Quality inconsistency | Medium | Medium | QC process, templates |
| Time overrun | Medium | Medium | Automation, parallel work |
| Storage costs | Low | Low | Optimize file sizes |

---

## ❓ Open Questions

- [ ] NotebookLM API access - need to verify capabilities (Owner: จูล่ง, Due: 2026-01-30)
- [ ] Publishing platforms priority - which first? (Owner: ท่านแม่ทัพ, Due: 2026-01-31)
- [ ] Revenue model for content - free vs paid? (Owner: กุนซือ, Due: 2026-02-05)

---

## 📚 References

### Related Documents
- [SWP3 Curriculum Overview](https://notion.so/...)
- [NotebookLM Documentation](https://notebooklm.google/)
- [n8n Workflows](https://github.com/AiKongGithub/pink-house-n8n)

### External Resources
- [NotebookLM Best Practices](https://support.google.com/notebooklm)
- [Content Repurposing Strategies](https://...)

---

## ✅ Approval

### Review Checklist
- [x] Requirements are clear and testable
- [x] Success metrics are defined
- [x] Timeline is realistic
- [x] Risks are identified and mitigated
- [x] Dependencies are documented

### Sign-off

| Role | Name | Status | Date |
|------|------|--------|------|
| Author | จูล่ง (CTO) | ✅ Created | 2026-01-28 |
| Deputy MD | ปลัดซัน | ⬜ Reviewed | - |
| MD | กุนซือสุมาอี้ | ⬜ Approved | - |
| Chairman | ท่านแม่ทัพ Kong | ⬜ Final Approval | - |

---

## 📝 Changelog

| Date | Author | Changes |
|------|--------|---------|
| 2026-01-28 | จูล่ง | Initial draft using TEMPLATE.md |

---

> **สามประสานจึงไร้พ่าย!** 🚩

*Created using Pink Castle Foundation Kit v1.0*
*PRD Template test - Day 3*
