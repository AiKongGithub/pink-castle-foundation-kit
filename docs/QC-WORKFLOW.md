# QC Workflow - Content 15,300 Project

> **Version:** 1.0
> **Last Updated:** 2026-01-28
> **Reviewer:** ปลัดซัน (Deputy QC Officer)
> **Project:** Content Production Pipeline

---

## Overview

เอกสารนี้กำหนดกระบวนการควบคุมคุณภาพ (Quality Control) สำหรับโครงการ Content 15,300 ชิ้น ครอบคลุมเกณฑ์คุณภาพ, Checklist, และ Flow การ Review

### Team Roles

| Role | Person | Responsibility |
|------|--------|----------------|
| Chairman | ท่านสหาย Kong | Final approval, Strategic direction |
| MD กุนซือ | สุมาอี้ (Claude.ai) | Content planning, Strategy |
| Deputy ปลัดซัน | QC Officer | Quality review, Approval |
| CTO จูล่ง | Claude Code | Content production, Technical |

---

## QC Flow

```
┌─────────────────────────────────────────────────────────────┐
│                     QC WORKFLOW                              │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│   ┌──────────┐    ┌──────────┐    ┌──────────────────┐      │
│   │  DRAFT   │───►│  REVIEW  │───►│  APPROVED/       │      │
│   │  (จูล่ง) │    │ (ปลัดซัน)│    │  REVISION        │      │
│   └──────────┘    └──────────┘    └──────────────────┘      │
│        │               │                    │                │
│        ▼               ▼                    ▼                │
│   - Create content  - Check quality     - Pass: Publish     │
│   - Self-check      - Score criteria    - Fail: Return      │
│   - Submit          - Write report      - Feedback given    │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

### Status Definitions

| Status | Description | Next Action |
|--------|-------------|-------------|
| `Draft` | Content created, pending review | Submit to ปลัดซัน |
| `In Review` | Being reviewed by ปลัดซัน | Wait for feedback |
| `Approved` | Passed QC, ready to publish | Move to Published |
| `Revision` | Failed QC, needs fixes | Fix and resubmit |
| `Published` | Live on platform | Archive source |

---

## Quality Criteria by Format

### Pass Threshold
**ทุก format ต้องได้คะแนนเฉลี่ย ≥ 3.5/5 (70%) จึงจะผ่าน QC**

---

### 1. Audio Overview (ภาพรวมเสียง)

| Criteria | Weight | Score (1-5) | Description |
|----------|--------|-------------|-------------|
| Content Accuracy | 25% | | เนื้อหาถูกต้องตามต้นฉบับ |
| Clarity | 25% | | อธิบายชัดเจน เข้าใจง่าย |
| Structure | 20% | | มีโครงสร้าง: เปิด-เนื้อหา-สรุป |
| Language | 20% | | ภาษาไทยถูกต้อง เหมาะกับการฟัง |
| Duration | 10% | | 10-15 นาทีตามกำหนด |

**Key Checklist:**
- [ ] ครอบคลุม Key Points ทั้งหมด
- [ ] มี Opening Hook
- [ ] มีการยกตัวอย่างประกอบ
- [ ] สรุปท้ายชัดเจน
- [ ] ความยาวเหมาะสม (10-15 นาที)

---

### 2. Video Summary (สรุปวิดีโอ)

| Criteria | Weight | Score (1-5) | Description |
|----------|--------|-------------|-------------|
| Content Accuracy | 25% | | เนื้อหาถูกต้อง ครบถ้วน |
| Visual Appeal | 25% | | มีคำแนะนำ Visual ชัดเจน |
| Engagement | 20% | | มี Hook, CTA, กระตุ้นความสนใจ |
| Structure | 20% | | มี Intro-Body-Outro ชัดเจน |
| Duration | 10% | | 5-10 นาทีตามกำหนด |

**Key Checklist:**
- [ ] มี Timestamp/Segments ครบ
- [ ] Visual suggestions เหมาะสม
- [ ] Hook ดึงดูด (5 วินาทีแรก)
- [ ] มี Call-to-Action
- [ ] ความยาวเหมาะสม (5-10 นาที)

---

### 3. Mind Map (แผนที่ความคิด)

| Criteria | Weight | Score (1-5) | Description |
|----------|--------|-------------|-------------|
| Completeness | 25% | | ครอบคลุมทุกหัวข้อสำคัญ |
| Hierarchy | 25% | | โครงสร้างลำดับชั้นถูกต้อง |
| Connections | 20% | | ความสัมพันธ์ระหว่างหัวข้อชัด |
| Readability | 20% | | อ่านเข้าใจง่าย สแกนได้เร็ว |
| Technical | 10% | | Mermaid syntax ถูกต้อง render ได้ |

**Key Checklist:**
- [ ] Central node ชัดเจน
- [ ] 4-6 Main branches
- [ ] Sub-branches ไม่เกิน 3 ระดับ
- [ ] Mermaid syntax valid
- [ ] Export ได้หลาย format

---

### 4. Report (รายงานเขียน)

| Criteria | Weight | Score (1-5) | Description |
|----------|--------|-------------|-------------|
| Content Accuracy | 30% | | ข้อมูลถูกต้อง อ้างอิงได้ |
| Structure | 25% | | มีโครงสร้าง: บทนำ-เนื้อหา-สรุป |
| Depth | 20% | | ลงลึกเพียงพอ มี insights |
| Readability | 15% | | อ่านง่าย ย่อหน้าเหมาะสม |
| Length | 10% | | 500-1000 คำตามกำหนด |

**Key Checklist:**
- [ ] Executive Summary มี
- [ ] Key Takeaways 3-5 ข้อ
- [ ] อ้างอิง Source ชัดเจน
- [ ] Actionable recommendations
- [ ] 500-1000 คำ

---

### 5. Flashcards (แฟลชการ์ด)

| Criteria | Weight | Score (1-5) | Description |
|----------|--------|-------------|-------------|
| Content Coverage | 25% | | ครอบคลุม concepts สำคัญ |
| Question Clarity | 25% | | คำถามชัดเจน ตรงประเด็น |
| Answer Quality | 25% | | คำตอบกระชับ จำง่าย |
| Learning Value | 25% | | ช่วยให้เรียนรู้/จดจำได้จริง |

**Key Checklist:**
- [ ] 10-20 cards ต่อ source
- [ ] Mix card types (Definition, Concept, List, Application)
- [ ] คำถามชัดเจน ไม่กำกวม
- [ ] คำตอบกระชับ (1-3 ประโยค)
- [ ] พร้อม import Anki/Quizlet

---

### 6. Quiz (แบบทดสอบ)

| Criteria | Weight | Score (1-5) | Description |
|----------|--------|-------------|-------------|
| Content Coverage | 25% | | ทดสอบ key concepts ครบ |
| Question Clarity | 25% | | คำถามชัดเจน ไม่กำกวม |
| Answer Accuracy | 25% | | เฉลยถูกต้อง คำอธิบายดี |
| Learning Value | 25% | | ช่วยทบทวนความรู้ |

**Key Checklist:**
- [ ] 10 ข้อต่อ quiz
- [ ] Mix: 60% Multiple Choice, 30% True/False, 10% Fill-in
- [ ] Mix: 30% Easy, 40% Medium, 30% Hard
- [ ] ทุกข้อมี Explanation
- [ ] Answer Key ครบถ้วน

---

### 7. Infographic (อินโฟกราฟิก)

| Criteria | Weight | Score (1-5) | Description |
|----------|--------|-------------|-------------|
| Content Clarity | 25% | | เนื้อหาชัด เข้าใจง่าย |
| Visual Appeal | 25% | | ออกแบบสวย น่าสนใจ |
| Brand Consistency | 20% | | ตรง Pink Castle style guide |
| Readability | 20% | | อ่าน/สแกนได้เร็ว |
| Technical Quality | 10% | | Resolution เหมาะสม mobile-ready |

**Key Checklist:**
- [ ] Title ชัดเจน (5-8 คำ)
- [ ] 5-7 key points
- [ ] ข้อความกระชับ (10 คำ/จุด)
- [ ] Icon suggestions เหมาะสม
- [ ] Color scheme ตาม brand

---

### 8. Slides (ชุดสไลด์)

| Criteria | Weight | Score (1-5) | Description |
|----------|--------|-------------|-------------|
| Content Coverage | 25% | | ครอบคลุม main concepts |
| Visual Design | 25% | | ออกแบบดี ไม่แน่น |
| Clarity | 20% | | 1 idea per slide |
| Flow | 20% | | ลำดับเหมาะสม transition ดี |
| Technical | 10% | | ใช้งานได้ใน Slides/PowerPoint |

**Key Checklist:**
- [ ] 10-15 slides
- [ ] Title → Agenda → Content → Summary → CTA
- [ ] 1 main idea per slide
- [ ] Max 5 bullets per slide
- [ ] Visual suggestions included

---

### 9. Data Table (ตารางข้อมูล)

| Criteria | Weight | Score (1-5) | Description |
|----------|--------|-------------|-------------|
| Data Accuracy | 30% | | ข้อมูลถูกต้อง ครบถ้วน |
| Completeness | 25% | | ครอบคลุม data points สำคัญ |
| Structure | 25% | | โครงสร้างเหมาะสม หาง่าย |
| Usability | 20% | | Export ได้ ใช้งานจริงได้ |

**Key Checklist:**
- [ ] Headers ชัดเจน
- [ ] Data จัดหมวดหมู่ดี
- [ ] Consistent formatting
- [ ] Export ได้ (CSV, Markdown, JSON)
- [ ] พร้อมใช้ใน Sheets/Notion

---

## QC Review Process

### Step 1: Submission (จูล่ง)

1. Complete content creation
2. Run self-check against checklist
3. Fill in QC Request Form
4. Submit via Notion or commit

**Self-Check Template:**
```markdown
## Self-Check Report
- Content: [Title]
- Format: [Format Type]
- Source: [Chapter/File]
- Date: [YYYY-MM-DD]

### Checklist Completed:
- [x] Item 1
- [x] Item 2
- [ ] Item 3 (explain)

### Notes:
[Any concerns or questions]
```

---

### Step 2: Review (ปลัดซัน)

1. Receive submission notification
2. Review against criteria
3. Score each criterion (1-5)
4. Calculate weighted average
5. Write feedback
6. Approve or Request Revision

**Review Timeframe:**
- Standard: 24-48 hours
- Urgent: 4-8 hours
- Batch (10+ items): 1 week

---

### Step 3: Decision

**If Score ≥ 3.5 (70%):**
- Status → `Approved`
- Move to publishing queue
- Archive source files

**If Score < 3.5 (70%):**
- Status → `Revision`
- Return with specific feedback
- Creator fixes and resubmits
- Re-review (faster turnaround)

---

## QC Report Template

```markdown
# QC Report

## Basic Information
| Field | Value |
|-------|-------|
| Content ID | [ID] |
| Title | [Title] |
| Format | [Format Type] |
| Source | [Chapter/File] |
| Creator | จูล่ง |
| Reviewer | ปลัดซัน |
| Review Date | [YYYY-MM-DD] |

## Scoring

| Criteria | Weight | Score | Weighted |
|----------|--------|-------|----------|
| [Criterion 1] | 25% | [1-5] | [calc] |
| [Criterion 2] | 25% | [1-5] | [calc] |
| [Criterion 3] | 25% | [1-5] | [calc] |
| [Criterion 4] | 25% | [1-5] | [calc] |
| **Total** | 100% | | **[avg]** |

## Decision

- [ ] ✅ **APPROVED** (Score ≥ 3.5)
- [ ] ❌ **REVISION REQUIRED** (Score < 3.5)

## Feedback

### Strengths:
1. [What was done well]
2. [What was done well]

### Areas for Improvement:
1. [Specific issue + how to fix]
2. [Specific issue + how to fix]

### Required Changes (if Revision):
- [ ] Change 1
- [ ] Change 2

## Reviewer Signature

ปลัดซัน | [Date]
```

---

## Batch QC Process

สำหรับ review content จำนวนมาก (10+ ชิ้นต่อครั้ง)

### Batch Submission Format

```markdown
# Batch QC Request

**Batch ID:** BATCH-[YYYYMMDD]-[NUMBER]
**Submitted:** [Date]
**Total Items:** [Count]
**Format:** [Single format or Mixed]

## Items

| # | Content ID | Title | Format | Source |
|---|------------|-------|--------|--------|
| 1 | [ID] | [Title] | [Format] | [Source] |
| 2 | [ID] | [Title] | [Format] | [Source] |
| ... | ... | ... | ... | ... |

## Notes
[Any batch-specific notes]
```

### Batch Review Report

```markdown
# Batch QC Report

**Batch ID:** BATCH-[YYYYMMDD]-[NUMBER]
**Reviewed:** [Date]
**Reviewer:** ปลัดซัน

## Summary

| Metric | Value |
|--------|-------|
| Total Items | [Count] |
| Approved | [Count] (%) |
| Revision | [Count] (%) |
| Average Score | [Score] |

## Results

| # | Content ID | Score | Status | Notes |
|---|------------|-------|--------|-------|
| 1 | [ID] | [Score] | ✅/❌ | [Brief] |
| 2 | [ID] | [Score] | ✅/❌ | [Brief] |
| ... | ... | ... | ... | ... |

## Overall Feedback
[General observations and recommendations]
```

---

## Escalation Process

### When to Escalate

| Situation | Escalate To |
|-----------|-------------|
| Score borderline (3.3-3.5) | MD กุนซือ |
| Dispute between Creator/Reviewer | Chairman |
| Repeated failures (3+ times) | Chairman |
| Technical issues | CTO จูล่ง |
| Timeline concerns | MD กุนซือ |

### Escalation Format

```markdown
# QC Escalation Request

**Date:** [YYYY-MM-DD]
**Escalated By:** [Name]
**Escalate To:** [Name]

## Issue
[Description of the issue]

## Context
[Relevant background]

## Recommendation
[Proposed solution]

## Urgency
- [ ] Low (1 week)
- [ ] Medium (2-3 days)
- [ ] High (24 hours)
- [ ] Critical (immediate)
```

---

## Metrics & Reporting

### Weekly QC Dashboard

| Metric | Target | Actual |
|--------|--------|--------|
| Items Reviewed | 100/week | [Actual] |
| Approval Rate | ≥80% | [Actual] |
| Avg Score | ≥3.8 | [Actual] |
| Avg Review Time | ≤24h | [Actual] |
| Revision Turnaround | ≤48h | [Actual] |

### Monthly QC Report

1. **Volume Metrics**
   - Total items reviewed
   - Items by format
   - Items by chapter

2. **Quality Metrics**
   - Approval rate by format
   - Average scores by format
   - Revision rate trends

3. **Efficiency Metrics**
   - Review turnaround time
   - Revision cycle time
   - Bottleneck identification

4. **Insights & Actions**
   - Common issues found
   - Process improvements
   - Training needs

---

## Quick Reference

### Scoring Scale

| Score | Description | Thai |
|-------|-------------|------|
| 5 | Excellent - Exceeds expectations | ดีเยี่ยม |
| 4 | Good - Meets all requirements | ดี |
| 3 | Acceptable - Meets minimum | พอใช้ |
| 2 | Below Standard - Needs improvement | ต้องปรับปรุง |
| 1 | Poor - Major revision needed | ไม่ผ่าน |

### Status Colors

| Status | Color | Emoji |
|--------|-------|-------|
| Draft | Gray | 📝 |
| In Review | Yellow | 🔍 |
| Approved | Green | ✅ |
| Revision | Red | ❌ |
| Published | Blue | 🚀 |

### Quick Decisions

| Average Score | Decision |
|---------------|----------|
| 4.5+ | Approved - Excellent work |
| 3.5-4.4 | Approved - Good with minor notes |
| 3.0-3.4 | Borderline - Review needed |
| < 3.0 | Revision Required |

---

## Tags

`#qc` `#workflow` `#quality` `#review` `#content-production`

---

> *Pink Castle Foundation Kit v1.0*
> *QC Workflow Document - Content 15,300 Project*
