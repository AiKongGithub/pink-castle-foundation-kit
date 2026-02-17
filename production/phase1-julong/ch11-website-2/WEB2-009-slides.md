# Slides: วิธีตั้งค่า Plugin Akismet — WEB2-009
> **Format:** Slide Outline (12 Slides)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 9
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## Slide 1: หน้าปก (Title Slide)

- **วิธีตั้งค่า Plugin Akismet**
- SWP3 บทที่ 11: สร้างเว็บไซต์ Part 2 — ตอนที่ 9
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## Slide 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- เข้าใจว่า Comment Spam คืออะไรและอันตรายอย่างไร
- รู้จักวิธีทำงานของ Akismet (cloud-based AI)
- ขอ API Key ฟรีและติดตั้ง Akismet
- ตั้งค่า Spam Filtering และจัดการ False Positives
- รู้จักทางเลือกอื่นและเหตุผลที่ห้ามปิด Anti-spam

---

## Slide 3: Comment Spam คืออะไร?

- คอมเมนต์ที่สร้างโดย **bot อัตโนมัติ**
- เป้าหมาย: ใส่ลิงก์โฆษณา / ลิงก์อันตราย
- เว็บที่ไม่กรองอาจได้ **หลายร้อยอัน/วัน**
- **ผลเสีย 3 ด้าน:**
  - SEO — Google ลงโทษเว็บที่มี spam links
  - ความปลอดภัย — นำผู้ใช้ไปเว็บ malware
  - ความน่าเชื่อถือ — ผู้ใช้จริงไม่อยากมีส่วนร่วม

---

## Slide 4: Akismet ทำงานอย่างไร?

- **Cloud-based AI** — ไม่ได้กรองบน server ของเรา
- เมื่อมีคอมเมนต์ใหม่ → ส่งไปตรวจสอบที่ Akismet server
- มีฐานข้อมูล spam จาก **เว็บไซต์หลายล้านแห่ง** ทั่วโลก
- ตรวจพบ spam → ย้ายไป spam queue (ไม่แสดงบนเว็บ)
- ความแม่นยำ **เกือบ 100%** เรียนรู้ตลอดเวลา

---

## Slide 5: การติดตั้ง — ง่ายมาก

- **ขั้นตอน 1:** ไปที่ Plugins > Activate Akismet (มากับ WordPress)
- **ขั้นตอน 2:** ไปที่ akismet.com เลือกแพลนฟรี
- **ขั้นตอน 3:** เลื่อน slider ราคาไปที่ **0 บาท**
- **ขั้นตอน 4:** ได้ API Key → กลับมาใส่ใน Akismet Settings
- **ขั้นตอน 5:** กด Connect → เสร็จ! กรอง spam อัตโนมัติ

---

## Slide 6: API Key — ฟรีสำหรับเว็บส่วนบุคคล

- ขอที่ **akismet.com** ต้องมีบัญชี WordPress.com
- **ฟรี** สำหรับเว็บส่วนบุคคล / บล็อกไม่ทำเงิน
- เลื่อน slider ราคาไปที่ 0 (ไม่ต้องจ่าย)
- เว็บธุรกิจ → ใช้แพลนเสียเงิน
- API Key ใช้ได้กับหลายเว็บไซต์

---

## Slide 7: ตั้งค่า Spam Filtering

- **ตัวเลือก 1:** ย้ายไป spam queue (แนะนำ)
- **ตัวเลือก 2:** ลบ spam ทิ้งอัตโนมัติ (ไม่แนะนำ)
- ทำไมเลือกตัวเลือก 1? → ป้องกัน **False Positives**
- False Positive = คอมเมนต์จริงที่ถูกจับเป็น spam
- ต้องเข้าตรวจสอบ spam queue เป็นประจำ

---

## Slide 8: จัดการ False Positives

- **False Positive** = คอมเมนต์จริง ถูก Akismet จับว่าเป็น spam
- สาเหตุ: มีลิงก์หลายอัน, มีคำคล้าย spam, IP น่าสงสัย
- **วิธีจัดการ:** ไปที่ Comments > Spam
- พบคอมเมนต์จริง → กด **"Not Spam"**
- Akismet จะ **เรียนรู้** และไม่จับผิดซ้ำ
- ตรวจสอบ **สัปดาห์ละ 1 ครั้ง**

---

## Slide 9: อย่าปิด Anti-spam เด็ดขาด!

- Bot ไม่สนว่าเว็บ **ใหญ่หรือเล็ก** — spam ทุกเว็บ
- ปิดแม้แค่ **1 วัน** อาจได้ spam หลายร้อยอัน
- Spam ที่ค้างอยู่ส่งผลเสียต่อ **SEO ทันที**
- ต้องเสียเวลามานั่งลบ spam ทีหลัง
- **ป้องกันตั้งแต่ต้นดีกว่าแก้ภายหลัง**

---

## Slide 10: ทางเลือกอื่นนอกจาก Akismet

| ปลั๊กอิน | ราคา | API Key | จุดเด่น |
|----------|------|:---:|---------|
| Akismet | ฟรี (ส่วนบุคคล) | ต้องใช้ | Cloud AI แม่นมาก |
| Antispam Bee | ฟรี 100% | ไม่ต้อง | Privacy-friendly GDPR |
| CleanTalk | เสียเงิน | ต้องใช้ | ครอบคลุม comment + form |

- เลือกตามความต้องการด้าน privacy และฟีเจอร์

---

## Slide 11: Akismet กับ Contact Forms

- Akismet ทำงานร่วมกับ Contact Form ได้ด้วย
- รองรับ: **Contact Form 7, WPForms, Gravity Forms**
- กรอง spam submission จากฟอร์มติดต่อ
- ไม่ใช่แค่คอมเมนต์ — ป้องกัน spam **ทุกช่องทาง**
- ตรวจสอบว่าปลั๊กอิน form ที่ใช้รองรับ Akismet

---

## Slide 12: สรุปและก้าวต่อไป (Summary & Next Steps)

- Comment spam อันตราย — ต้องป้องกันตั้งแต่วันแรก
- Akismet: cloud AI แม่นเกือบ 100%, API Key ฟรี
- ตั้งค่า: ย้ายไป spam queue, ตรวจ False Positives สัปดาห์ละครั้ง
- อย่าปิด Anti-spam เด็ดขาด
- **สรุป Ch11:** ครบทุกเรื่อง Blog Settings, Performance, Social Media, Jetpack, Akismet

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
