# Notion Database Setup - Content Production

> **Created:** 2026-01-28
> **Project:** Content 15,300 Pieces
> **Status:** Ready for Use

---

## Database Information

| Field | Value |
|-------|-------|
| Name | Content Production - 15,300 Pieces |
| URL | https://www.notion.so/42f92631baf341f8a52dabf77f7e1327 |
| Data Source ID | `0eed8158-8d80-45d3-9cb6-3a747f915043` |
| Parent Page | Pink Castle - บันทึกความคืบหน้า |
| Parent ID | `2f25dcbd-48ac-81bd-8604-e66a6318e98d` |

---

## Database Schema

### Properties

| Property | Type | Options/Description |
|----------|------|---------------------|
| **Title** | title | ชื่อ content piece |
| **Chapter** | select | บทที่ 1-23 (15 options) |
| **Source File** | text | ชื่อไฟล์ต้นทาง |
| **Format** | multi_select | 9 formats (Audio, Video, etc.) |
| **Status** | select | Draft, In Progress, Review, Published |
| **QC Status** | select | Pending, Passed, Failed |
| **Assigned To** | people | ผู้รับผิดชอบ |
| **Due Date** | date | กำหนดส่ง |
| **Duration** | text | ความยาวของ source file |
| **Priority** | select | High, Medium, Low |

---

## Chapter Options

| # | Chapter Name | Color |
|---|--------------|-------|
| 1 | บทที่ 1: 8 ขั้นตอนสร้างความมั่งคั่ง | blue |
| 2 | บทที่ 2: วิธีการทำการตลาดออนไลน์ | blue |
| 3 | บทที่ 3: วิธีสร้างธุรกิจออนไลน์ | blue |
| 4 | บทที่ 4: Sale Funnel | green |
| 5 | บทที่ 5: ค้นหาไอเดียธุรกิจ | green |
| 6 | บทที่ 6: สร้างเว็บไซต์ | green |
| 7 | บทที่ 7: คีย์เวิร์ดหมื่นล้าน | orange |
| 8 | บทที่ 8: กลยุทธ์ Topic | orange |
| 9 | บทที่ 9: Video Marketing | orange |
| 10 | บทที่ 10: Youtube Marketing | red |
| 11 | บทที่ 11-14: Paid Traffic & Ads | purple |
| 12 | บทที่ 15: Top Sponsor | red |
| 13 | บทที่ 16-17: Email & Webinar | pink |
| 14 | บทที่ 18-19: Grow Audience & Website | red |
| 15 | บทที่ 20-23: Advanced | gray |

---

## Format Options (9 Types)

| # | Format | Color | Thai Name |
|---|--------|-------|-----------|
| 1 | Audio Overview | blue | ภาพรวมแบบเสียง |
| 2 | Video Summary | red | ภาพรวมแบบวิดีโอ |
| 3 | Mind Map | green | แผนผังความคิด |
| 4 | Report | gray | รายงาน |
| 5 | Flashcards | yellow | แฟลชการ์ด |
| 6 | Quiz | orange | แบบทดสอบ |
| 7 | Infographic | purple | อินโฟกราฟิก |
| 8 | Slides | pink | ชุดสไลด์ |
| 9 | Data Table | brown | ตารางข้อมูล |

---

## Status Workflow

```
Draft → In Progress → Review → Published
gray      blue         yellow    green
```

---

## QC Status

| Status | Color | Description |
|--------|-------|-------------|
| Pending | gray | รอ QC review |
| Passed | green | ผ่าน QC |
| Failed | red | ไม่ผ่าน - ต้องแก้ไข |

---

## Priority Levels

| Priority | Color | Use Case |
|----------|-------|----------|
| High | red | บทยาว (Top 5) |
| Medium | yellow | บททั่วไป |
| Low | green | บทสั้น |

---

## How to Use

### Creating a Content Entry

1. Go to database: https://www.notion.so/42f92631baf341f8a52dabf77f7e1327
2. Click "New" to add a page
3. Fill in:
   - **Title**: ชื่อ content (e.g., "Youtube Marketing ตอนที่ 1 - Audio Overview")
   - **Chapter**: เลือกบท
   - **Source File**: ชื่อไฟล์ต้นฉบับ
   - **Format**: เลือก format(s) ที่สร้าง
   - **Status**: เริ่มต้นเป็น Draft
   - **Priority**: High/Medium/Low
   - **Assigned To**: ผู้รับผิดชอบ
   - **Due Date**: กำหนดส่ง

### Status Update Flow

1. **Draft** → เริ่มสร้าง
2. **In Progress** → กำลังทำ
3. **Review** → ส่ง ปลัดซัน review
4. **Published** → ผ่าน QC และเผยแพร่แล้ว

### QC Process

1. ปลัดซัน receives Review items
2. Check against QC checklist
3. Mark QC Status:
   - **Passed** → Ready for publish
   - **Failed** → Return for revision

---

## API Integration (for n8n)

### Data Source ID
```
0eed8158-8d80-45d3-9cb6-3a747f915043
```

### Example: Create Page via API

```json
{
  "parent": {"data_source_id": "0eed8158-8d80-45d3-9cb6-3a747f915043"},
  "properties": {
    "Title": "Content Title",
    "Chapter": "บทที่ 10: Youtube Marketing",
    "Source File": "youtube-marketing-01.mp4",
    "Format": "[\"Audio Overview\", \"Mind Map\"]",
    "Status": "Draft",
    "QC Status": "Pending",
    "Priority": "High"
  }
}
```

---

## Related Resources

- **Inventory**: `ai_docs/swp3-inventory.md`
- **PRD**: `prds/content-15300-pieces.md`
- **Plan**: `.claude/PRPs/plans/content-15300-pieces.plan.md`
- **SWP3 Source**: https://www.notion.so/2f35dcbd48ac819caeecd539d98bd5a6
- **Google Drive**: https://drive.google.com/drive/folders/1KAlBxMglhbU_4YJ4pLDwVxWaLmk6vjsc

---

> **สามประสานจึงไร้พ่าย!**
>
> *Pink Castle Foundation Kit v1.0*
