# Quiz Template

> **Format:** Quiz (แบบทดสอบ)
> **Tool:** NotebookLM + Google Forms/Typeform
> **Output:** Interactive assessment
> **Quantity:** 10 questions per source

---

## Purpose

Create assessment quizzes that test understanding of source content, providing immediate feedback and reinforcing learning.

---

## Template Structure

### Quiz Header
```
# [Topic] Quiz

**Source:** [Content name]
**Questions:** 10
**Passing Score:** 70%
**Time Limit:** 15 minutes (optional)
```

### Question Types

#### 1. Multiple Choice (50-60%)
```
Q1. [Question text]
   a) [Option A]
   b) [Option B]
   c) [Option C]
   d) [Option D]

Correct: [Letter]
Explanation: [Why this is correct]
```

#### 2. True/False (20-30%)
```
Q2. [Statement]
   a) True / ถูก
   b) False / ผิด

Correct: [Answer]
Explanation: [Clarification]
```

#### 3. Fill in the Blank (10-20%)
```
Q3. _______ คือกลยุทธ์ที่ใช้เพื่อ [purpose]

Correct: [Answer]
Acceptable variations: [Alt 1, Alt 2]
```

---

## NotebookLM Prompt

```
Create a quiz from this content that:
1. Has exactly 10 questions
2. Uses 60% multiple choice, 30% true/false, 10% fill-in
3. Tests key concepts and applications
4. Includes explanations for each answer
5. Has clear, unambiguous questions
6. Is in Thai language
7. Covers easy, medium, and hard difficulty
```

---

## Example Output

**Source:** บทที่ 10: Youtube Marketing Mastery ตอนที่ 1

```markdown
# Youtube Marketing Mastery Quiz

**Source:** SWP3 บทที่ 10
**Questions:** 10
**Passing Score:** 70%

---

## Questions

**Q1. (Multiple Choice - Easy)**
Youtube Algorithm ให้ความสำคัญกับอะไรมากที่สุด?

a) จำนวน Views
b) จำนวน Subscribers
c) Watch Time
d) จำนวน Likes

**Correct:** c) Watch Time
**Explanation:** Youtube ต้องการให้คนอยู่บนแพลตฟอร์มนานที่สุด
จึงให้ความสำคัญกับ Watch Time มากกว่า metrics อื่น

---

**Q2. (True/False - Easy)**
การอัพโหลดวิดีโอทุกวันสำคัญกว่าคุณภาพของวิดีโอ

a) ถูก
b) ผิด

**Correct:** b) ผิด
**Explanation:** คุณภาพสำคัญกว่าปริมาณ วิดีโอที่ดี 1 ชิ้น
ดีกว่าวิดีโอธรรมดา 7 ชิ้น ในแง่ของ Watch Time

---

**Q3. (Multiple Choice - Medium)**
CTR (Click-Through Rate) ที่ดีสำหรับ Youtube คือเท่าไหร่?

a) 1-2%
b) 3-5%
c) 5-10%
d) 10-15%

**Correct:** c) 5-10%
**Explanation:** CTR 5-10% ถือว่าดี โดย Youtube จะส่งเสริม
วิดีโอที่มี CTR สูงกว่าค่าเฉลี่ยของช่อง

---

**Q4. (Fill in the Blank - Medium)**
_______ คือ 3 วินาทีแรกของวิดีโอที่ต้องดึงดูดความสนใจคนดู

**Correct:** Hook
**Acceptable:** Hook, ฮุค, Opening Hook

---

**Q5. (Multiple Choice - Medium)**
Thumbnail ที่ดีควรมีลักษณะอย่างไร?

a) ใส่ข้อความเยอะๆ เพื่อให้ข้อมูลครบ
b) ใช้สีเข้มๆ และหน้าคนที่มีอารมณ์ชัดเจน
c) ใช้ภาพจากวิดีโอโดยไม่ต้องแก้ไข
d) ทำให้เหมือนกับช่องอื่นที่ประสบความสำเร็จ

**Correct:** b) ใช้สีเข้มๆ และหน้าคนที่มีอารมณ์ชัดเจน
**Explanation:** สีที่โดดเด่นและอารมณ์บนใบหน้าดึงดูดสายตา
และทำให้คน click มากกว่า

---

**Q6. (True/False - Medium)**
ควรใส่ Keywords ไว้ในตอนต้นของ Title เสมอ

a) ถูก
b) ผิด

**Correct:** a) ถูก
**Explanation:** Youtube ให้น้ำหนักกับ Keywords
ที่อยู่ตอนต้นของ Title มากกว่าตอนท้าย

---

**Q7. (Multiple Choice - Hard)**
End Screen ควรปรากฏตอนไหนของวิดีโอ?

a) ตั้งแต่วินาทีแรก
b) 30 วินาทีสุดท้าย
c) 20 วินาทีสุดท้าย
d) 10 วินาทีสุดท้าย

**Correct:** c) 20 วินาทีสุดท้าย
**Explanation:** End Screen สามารถใส่ได้ใน 5-20 วินาทีสุดท้าย
แต่ 20 วินาทีให้พื้นที่มากที่สุดในการ promote content อื่น

---

**Q8. (Multiple Choice - Hard)**
การใส่ Chapters ในวิดีโอช่วยเรื่องอะไรมากที่สุด?

a) เพิ่ม Watch Time
b) ช่วยให้คนดูหาเนื้อหาที่ต้องการได้ง่าย
c) ทำให้ได้ Suggested Videos มากขึ้น
d) ถูกทุกข้อ

**Correct:** d) ถูกทุกข้อ
**Explanation:** Chapters ช่วยทั้ง user experience และ SEO
Youtube ชอบวิดีโอที่มี Chapters เพราะช่วยให้คนดูหาข้อมูลได้ง่าย

---

**Q9. (Fill in the Blank - Hard)**
_______ คือตัวเลขที่บอกว่ากี่เปอร์เซ็นต์ของคนที่ดูวิดีโอ
แล้วดูจนจบ

**Correct:** Audience Retention
**Acceptable:** Retention, Retention Rate

---

**Q10. (True/False - Hard)**
วิดีโอที่มีความยาวมากกว่า 10 นาที จะได้รับการส่งเสริม
จาก Algorithm มากกว่าวิดีโอสั้น

a) ถูก
b) ผิด

**Correct:** b) ผิด
**Explanation:** ไม่ใช่ความยาว แต่เป็น Watch Time %
วิดีโอสั้นที่คนดูจนจบ ดีกว่าวิดีโอยาวที่คนปิดกลางทาง

---

## Answer Key

| Q# | Answer | Difficulty |
|----|--------|------------|
| 1 | C | Easy |
| 2 | B | Easy |
| 3 | C | Medium |
| 4 | Hook | Medium |
| 5 | B | Medium |
| 6 | A | Medium |
| 7 | C | Hard |
| 8 | D | Hard |
| 9 | Audience Retention | Hard |
| 10 | B | Hard |

**Passing Score:** 7/10 (70%)
```

---

## Quality Checklist

### Content Quality
- [ ] Tests key concepts from source
- [ ] Questions are clear
- [ ] Answers are unambiguous
- [ ] Distractors are plausible

### Learning Design
- [ ] Mix of difficulty levels (Easy 30%, Medium 40%, Hard 30%)
- [ ] Mix of question types
- [ ] Explanations are educational
- [ ] Tests application not just recall

### Format
- [ ] 10 questions per quiz
- [ ] Consistent format
- [ ] Thai language is correct
- [ ] Ready for import

### Usability
- [ ] Can be taken online
- [ ] Immediate feedback
- [ ] Clear passing criteria
- [ ] Retakeable

---

## QC Scoring (ปลัดซัน)

| Criteria | Weight | Score (1-5) | Notes |
|----------|--------|-------------|-------|
| Content Coverage | 25% | | |
| Question Clarity | 25% | | |
| Answer Accuracy | 25% | | |
| Learning Value | 25% | | |
| **Total** | 100% | | |

**Pass Threshold:** 70% (3.5/5 average)

---

## Export Formats

- Google Forms
- Typeform
- Kahoot
- CSV/JSON

---

## Tags

`#quiz` `#assessment` `#notebooklm` `#testing` `#learning`

---

> *Pink Castle Foundation Kit v1.0*
