# Flashcards Template

> **Format:** Flashcards (แฟลชการ์ด)
> **Tool:** NotebookLM + Anki/Quizlet
> **Output:** Q&A cards for memorization
> **Quantity:** 10-20 cards per source

---

## Purpose

Create question-answer cards that help learners memorize and recall key concepts from source content through spaced repetition.

---

## Template Structure

### Card Format
```
FRONT (Question):
[Clear, specific question]

BACK (Answer):
[Concise, memorable answer]
[Optional: Example or mnemonic]
```

### Card Types

#### 1. Definition Cards
```
Q: [Term] คืออะไร?
A: [Clear definition in 1-2 sentences]
```

#### 2. Concept Cards
```
Q: [What/Why/How question about concept]
A: [Explanation with key points]
```

#### 3. List Cards
```
Q: [X] สิ่งสำคัญของ [Topic] มีอะไรบ้าง?
A: 1. [Item 1]
   2. [Item 2]
   3. [Item 3]
```

#### 4. Application Cards
```
Q: จะนำ [Concept] ไปใช้อย่างไร?
A: [Step-by-step or practical application]
```

#### 5. Comparison Cards
```
Q: [A] ต่างจาก [B] อย่างไร?
A: [Key differences]
```

---

## NotebookLM Prompt

```
Create flashcards from this content that:
1. Include 10-20 Q&A pairs
2. Cover key definitions, concepts, and applications
3. Use clear, specific questions
4. Have concise, memorable answers
5. Mix different card types
6. Are in Thai language
7. Format as "Q: ... / A: ..."
```

---

## Example Output

**Source:** บทที่ 4.1: Lead Magnet

```
=== CARD 1 (Definition) ===
Q: Lead Magnet คืออะไร?
A: ของแจกฟรีที่มีคุณค่า เพื่อแลกกับข้อมูลติดต่อ
   ของผู้มุ่งหวัง (เช่น อีเมล, เบอร์โทร)

=== CARD 2 (List) ===
Q: Lead Magnet มีกี่ประเภทหลักๆ?
A: 5 ประเภท:
   1. E-book / PDF Guide
   2. Checklist / Template
   3. Video Training
   4. Free Trial / Demo
   5. Quiz / Assessment

=== CARD 3 (Concept) ===
Q: ทำไม Lead Magnet ต้องแก้ปัญหาเฉพาะเจาะจง?
A: เพราะคนจะให้ข้อมูลติดต่อเมื่อเห็นคุณค่าที่ชัดเจน
   และตรงกับปัญหาที่เขามี

=== CARD 4 (Application) ===
Q: 5 ขั้นตอนสร้าง Lead Magnet มีอะไรบ้าง?
A: 1. ระบุปัญหาของกลุ่มเป้าหมาย
   2. เลือกรูปแบบที่เหมาะสม
   3. สร้างเนื้อหาที่มีคุณค่า
   4. ออกแบบให้น่าสนใจ
   5. สร้างหน้า Landing Page

=== CARD 5 (Comparison) ===
Q: Lead Magnet ต่างจาก Tripwire อย่างไร?
A: Lead Magnet = ฟรี (แลกด้วย email)
   Tripwire = ราคาถูก (แลกด้วยเงิน + สร้าง buyer)

=== CARD 6 (Definition) ===
Q: Capture Page คืออะไร?
A: หน้าเว็บที่ออกแบบมาเฉพาะ เพื่อเก็บข้อมูลติดต่อ
   โดยใช้ Lead Magnet เป็นตัวล่อ

=== CARD 7 (List) ===
Q: องค์ประกอบสำคัญของ Capture Page มีอะไรบ้าง?
A: 1. Headline ที่ดึงดูด
   2. รูปภาพ Lead Magnet
   3. Bullet points ประโยชน์
   4. Form กรอกข้อมูล
   5. Call-to-Action ชัดเจน

=== CARD 8 (Concept) ===
Q: หลักการ "Quick Win" ใน Lead Magnet คืออะไร?
A: ให้ผู้รับสามารถนำไปใช้และเห็นผลได้ทันที
   ไม่ต้องใช้เวลาหรือทรัพยากรมาก

=== CARD 9 (Application) ===
Q: จะวัดผลความสำเร็จของ Lead Magnet ได้อย่างไร?
A: 1. Conversion Rate (% คนกรอกฟอร์ม)
   2. Lead Quality (คุณภาพผู้สนใจ)
   3. Cost per Lead (ค่าใช้จ่ายต่อคน)

=== CARD 10 (Definition) ===
Q: Opt-in Rate คืออะไร?
A: เปอร์เซ็นต์ของคนที่เข้าชม Capture Page
   แล้วกรอกฟอร์มลงทะเบียน
   (ค่าเฉลี่ยที่ดี = 20-30%)
```

---

## Quality Checklist

### Content Quality
- [ ] Covers all key concepts
- [ ] Questions are clear and specific
- [ ] Answers are concise
- [ ] Information is accurate

### Learning Design
- [ ] Mix of card types
- [ ] Difficulty is appropriate
- [ ] Answers are memorable
- [ ] Examples are helpful

### Format
- [ ] 10-20 cards per source
- [ ] Consistent Q/A format
- [ ] Thai language is correct
- [ ] No typos

### Usability
- [ ] Ready for Anki/Quizlet import
- [ ] Can be studied standalone
- [ ] Builds on previous knowledge
- [ ] Practical value

---

## QC Scoring (ปลัดซัน)

| Criteria | Weight | Score (1-5) | Notes |
|----------|--------|-------------|-------|
| Content Coverage | 25% | | |
| Question Clarity | 25% | | |
| Answer Quality | 25% | | |
| Learning Value | 25% | | |
| **Total** | 100% | | |

**Pass Threshold:** 70% (3.5/5 average)

---

## Export Formats

- Anki deck (.apkg)
- Quizlet set
- CSV (Q,A format)
- Markdown

---

## Tags

`#flashcards` `#memorization` `#notebooklm` `#learning` `#anki`

---

> *Pink Castle Foundation Kit v1.0*
