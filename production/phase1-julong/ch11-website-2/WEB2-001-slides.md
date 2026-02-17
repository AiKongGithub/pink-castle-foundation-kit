# Slides: วิธีการตั้งค่าต่างๆ ของ WordPress — WEB2-001
> **Format:** Slide Outline (12 Slides)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 1
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## SLIDE 1: หน้าปก (Title Slide)

- **วิธีการตั้งค่าต่างๆ ของ WordPress**
- SWP3 บทที่ 11: สร้างเว็บไซต์ Part 2 — ตอนที่ 1
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- เข้าใจ 6 หมวดการตั้งค่า WordPress
- รู้จักการตั้งค่า General, Writing และ Reading
- จัดการระบบคอมเมนต์ผ่าน Discussion Settings
- เลือกโครงสร้าง URL ที่เป็นมิตรกับ SEO

---

## SLIDE 3: ทำไมต้องตั้งค่า WordPress ก่อน? (Why Settings First?)

- เหมือนเดินสายไฟก่อนตกแต่งบ้าน
- ตั้งค่าพื้นฐานผิด → สะสมเป็นปัญหาใหญ่
- Permalink เปลี่ยนทีหลังได้ยากมาก
- Search Visibility ลืมปิด = เว็บหายจาก Google
- **ทำให้ถูกตั้งแต่ครั้งแรก ดีกว่าแก้ทีหลัง**

---

## SLIDE 4: General Settings — ตั้งค่าทั่วไป

- **Site Title** — ชื่อเว็บไซต์ (แสดงใน Google)
- **Tagline** — คำอธิบายสั้นๆ เกี่ยวกับเว็บ
- **Timezone** — Bangkok / UTC+7 สำหรับไทย
- **Date Format** — เลือกรูปแบบวันที่ที่ถนัด
- **Site Language** — เลือกภาษาไทยสำหรับเว็บไทย

---

## SLIDE 5: Writing Settings — ตั้งค่าการเขียน

- **Default Post Category** — หมวดหมู่เริ่มต้นเมื่อลืมเลือก
- **Post Format** — ส่วนใหญ่ใช้ Standard
- ตั้งค่าน้อย แต่ช่วยป้องกันบทความไม่มีหมวดหมู่
- แนะนำ: สร้างหมวดหมู่หลักก่อน แล้วตั้งเป็นค่าเริ่มต้น

---

## SLIDE 6: Reading Settings — ตั้งค่าหน้าแรก

- **Homepage Display มี 2 แบบ:**
  - Your latest posts → เหมาะบล็อก
  - A static page → เหมาะเว็บธุรกิจ / Landing Page
- **Blog pages show** — แนะนำ 10 โพสต์ต่อหน้า
- **Search Engine Visibility** — ระวัง! ติ๊กแล้วเว็บหายจาก Google

---

## SLIDE 7: Discussion Settings — จัดการคอมเมนต์

- **Comment Moderation** — แนะนำเปิด เพื่อกรองสแปม
- **Avatars** — แสดงรูปโปรไฟล์ผู้คอมเมนต์
- **Notifications** — รับอีเมลเมื่อมีคอมเมนต์ใหม่
- เว็บ WordPress โดนสแปมคอมเมนต์เป็นเรื่องปกติ
- พิจารณาติดตั้งปลั๊กอิน Akismet Anti-Spam เพิ่ม

---

## SLIDE 8: Media Settings — ตั้งค่ารูปภาพ

| ขนาด | ค่าเริ่มต้น |
|------|-----------|
| Thumbnail | 150 x 150 px |
| Medium | 300 x 300 px |
| Large | 1024 x 1024 px |

- WordPress สร้าง 3 สำเนาทุกครั้งที่อัปโหลด
- ค่าเริ่มต้นใช้ได้ดี ไม่ต้องเปลี่ยน
- แนะนำ optimize รูปก่อนอัปโหลด

---

## SLIDE 9: Permalink Settings — สำคัญที่สุด!

| รูปแบบ | ตัวอย่าง URL | แนะนำ |
|--------|------------|-------|
| Plain | ?p=123 | ไม่แนะนำ |
| Day and name | /2026/02/17/title | พอใช้ |
| Post name | /your-post-title | แนะนำมากที่สุด |

- Post name → URL สะอาด อ่านง่าย SEO ดี
- Google เข้าใจเนื้อหาจาก URL ได้ทันที
- Click-through rate สูงขึ้นเพราะ URL น่าเชื่อถือ

---

## SLIDE 10: คำเตือนสำคัญเรื่อง Permalink

- ต้องตั้งตั้งแต่วันแรก ก่อนเขียนบทความ
- เปลี่ยนทีหลัง → ลิงก์เก่าทั้งหมดพัง
- Google เสียอันดับ → ผู้เข้าชมเจอ 404
- ต้องทำ Redirect ซึ่งซับซ้อนมาก
- **สรุป: เลือก Post name → กดบันทึก → ทำวันแรก!**

---

## SLIDE 11: Checklist หลังติดตั้ง WordPress

- [ ] ตั้ง Permalink เป็น Post name (สำคัญที่สุด)
- [ ] ตั้ง Timezone เป็น Bangkok (UTC+7)
- [ ] ใส่ Site Title และ Tagline
- [ ] เปิด Comment Moderation
- [ ] ตรวจสอบ Homepage Display (Static page หรือ Latest posts)
- [ ] ตรวจสอบ Search Engine Visibility (เอาออกเมื่อพร้อม)

---

## SLIDE 12: สรุปและก้าวต่อไป (Summary & Next Steps)

- WordPress Settings มี 6 หมวด ทุกหมวดสำคัญ
- **Permalink = ตั้งก่อน เปลี่ยนทีหลังไม่ได้**
- Search Visibility = ลืมปิดเท่ากับเว็บไม่มีอยู่
- ทำตาม Checklist ให้ครบก่อนเริ่มสร้างเนื้อหา
- **ตอนหน้า:** วิธีการตั้ง Thrive Theme Plugin

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
