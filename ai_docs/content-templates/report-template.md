# Report Template

> **Format:** Report (รายงาน)
> **Tool:** NotebookLM
> **Output:** Written summary document
> **Length:** 1-2 pages (500-1000 words)

---

## Purpose

Create a comprehensive written summary of source content that can be read independently, shared, or used as reference material.

---

## Template Structure

### Header
```
# [Topic Title]

**Source:** [Original content name]
**Date:** [Creation date]
**Duration:** [Original content duration]
**Category:** [Chapter/Topic]
```

### Executive Summary (100-150 words)
```
## สรุปภาพรวม

[2-3 sentences covering the main topic and key takeaways]
```

### Key Concepts (300-500 words)
```
## แนวคิดหลัก

### 1. [Concept 1 Title]
[Explanation in 2-3 paragraphs]

### 2. [Concept 2 Title]
[Explanation in 2-3 paragraphs]

### 3. [Concept 3 Title]
[Explanation in 2-3 paragraphs]
```

### Practical Applications (100-200 words)
```
## การนำไปใช้

- [Application 1]
- [Application 2]
- [Application 3]
```

### Key Takeaways (50-100 words)
```
## สิ่งที่ได้เรียนรู้

1. [Takeaway 1]
2. [Takeaway 2]
3. [Takeaway 3]
```

### References (Optional)
```
## แหล่งอ้างอิง

- [Reference 1]
- [Reference 2]
```

---

## NotebookLM Prompt

```
Create a written report from this content that:
1. Has a clear executive summary
2. Covers 3-5 main concepts in detail
3. Includes practical applications
4. Ends with clear takeaways
5. Is 500-1000 words in Thai
6. Uses professional but accessible language
```

---

## Example Output

**Source:** บทที่ 8: กลยุทธ์การทำ Topic - Topic Cluster คืออะไร

```markdown
# Topic Cluster: กลยุทธ์ยึดหน้า 1 Google

**Source:** SWP3 บทที่ 8 - Topic Cluster คืออะไร
**Date:** 28 มกราคม 2569
**Duration:** 1:21:57
**Category:** Content Strategy

---

## สรุปภาพรวม

Topic Cluster เป็นกลยุทธ์การจัดโครงสร้างเนื้อหาบนเว็บไซต์
ที่ช่วยให้ Google เข้าใจความเชี่ยวชาญของเราในหัวข้อนั้นๆ
โดยการสร้างเนื้อหาที่เชื่อมโยงกันอย่างเป็นระบบ ทำให้เว็บไซต์
มีโอกาสติดอันดับบน Google มากขึ้น

---

## แนวคิดหลัก

### 1. Pillar Page คืออะไร

Pillar Page คือหน้าหลักที่ครอบคลุมหัวข้อใหญ่อย่างกว้างขวาง
เปรียบเสมือน "หนังสือ" ที่มีสารบัญครบถ้วน โดยแต่ละหัวข้อ
จะลิงก์ไปยังบทความย่อย (Cluster Content) ที่ลงลึกในแต่ละ
หัวข้อย่อย...

### 2. Cluster Content คืออะไร

Cluster Content คือบทความย่อยที่เจาะลึกในแต่ละหัวข้อ
เปรียบเสมือน "บท" ในหนังสือ โดยทุกบทจะลิงก์กลับไป
หา Pillar Page และลิงก์หากันภายใน Cluster...

### 3. Internal Linking Strategy

การเชื่อมโยงภายในเป็นกุญแจสำคัญ ทุก Cluster Content
ต้องลิงก์กลับไปหา Pillar Page และสามารถลิงก์หากัน
ภายในกลุ่มเดียวกันได้...

---

## การนำไปใช้

1. **เลือกหัวข้อหลัก** - หาหัวข้อที่มีความเชี่ยวชาญ
2. **วิจัย Keywords** - หา keywords ที่เกี่ยวข้อง
3. **สร้าง Pillar Page** - เขียนเนื้อหาครอบคลุม
4. **สร้าง Cluster Content** - เขียนบทความย่อย 5-10 ชิ้น
5. **เชื่อมโยง** - ใส่ internal links ทุกบทความ

---

## สิ่งที่ได้เรียนรู้

1. Topic Cluster ช่วยให้ Google เข้าใจความเชี่ยวชาญ
2. Pillar Page + Cluster Content + Internal Links = สูตรสำเร็จ
3. ต้องวางแผนก่อนเริ่มเขียน
```

---

## Quality Checklist

### Content Quality
- [ ] Executive summary is clear and concise
- [ ] All main concepts covered
- [ ] Information is accurate
- [ ] Practical applications are useful

### Structure
- [ ] Follows template structure
- [ ] Proper headings hierarchy
- [ ] Logical flow
- [ ] 500-1000 words

### Language
- [ ] Professional but accessible
- [ ] No grammar errors
- [ ] Consistent terminology
- [ ] Thai language is natural

### Usefulness
- [ ] Can stand alone without source
- [ ] Easy to reference
- [ ] Actionable takeaways
- [ ] Shareable

---

## QC Scoring (ปลัดซัน)

| Criteria | Weight | Score (1-5) | Notes |
|----------|--------|-------------|-------|
| Content Accuracy | 30% | | |
| Structure | 20% | | |
| Clarity | 20% | | |
| Practicality | 20% | | |
| Language | 10% | | |
| **Total** | 100% | | |

**Pass Threshold:** 70% (3.5/5 average)

---

## Export Formats

- Markdown (.md)
- PDF
- Google Doc
- Notion page

---

## Tags

`#report` `#summary` `#notebooklm` `#document` `#reference`

---

> *Pink Castle Foundation Kit v1.0*
