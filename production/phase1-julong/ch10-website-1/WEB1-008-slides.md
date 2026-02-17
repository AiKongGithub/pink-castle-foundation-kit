# Slides: วิธีการติดตั้ง Plugin ตอนที่ 1 — WEB1-008
> **Format:** Slide Outline (12 Slides)
> **Source:** SWP3 Ch10 สร้างเว็บไซต์ Part 1 ตอนที่ 8
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## SLIDE 1: หน้าปก (Title Slide)
─────────────────

- **วิธีการติดตั้ง Plugin ตอนที่ 1**
- SWP3 บทที่ 10: สร้างเว็บไซต์ Part 1 — ตอนที่ 8
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)
─────────────────

- เข้าใจว่า Plugin คืออะไร และทำไมถึงสำคัญ
- รู้วิธีค้นหาและติดตั้ง Plugin จากคลัง WordPress
- สามารถประเมินคุณภาพ Plugin ก่อนติดตั้งได้
- รู้จัก Plugin 5 ประเภทที่ทุกเว็บไซต์ต้องมี
- เลือก Plugin ที่เหมาะสมได้อย่างมั่นใจ

---

## SLIDE 3: Plugin คืออะไร? (What is a Plugin?)
─────────────────

- **Plugin** = ส่วนเสริมที่เพิ่มความสามารถให้ WordPress
- เปรียบเหมือน **แอปในมือถือ**
- WordPress เปล่า = โทร + ส่งข้อความ
- WordPress + Plugin = ทำได้ทุกอย่าง
- คลัง WordPress.org มี **60,000+ Plugin**
- ทุกความต้องการมี Plugin รองรับ

---

## SLIDE 4: วิธีติดตั้ง Plugin (How to Install)
─────────────────

1. เข้าหน้า Admin → **Plugins** → **Add New**
2. พิมพ์ค้นหาชื่อ Plugin ในช่อง Search
3. กด **Install Now** → รอการติดตั้ง
4. กด **Activate** → เปิดใช้งาน

- ง่ายเพียง 4 ขั้นตอน
- แต่... **ต้องประเมินคุณภาพก่อนกด Install!**

---

## SLIDE 5: การประเมินคุณภาพ Plugin (Quality Check)
─────────────────

| เกณฑ์ | สิ่งที่ต้องดู |
|-------|-------------|
| Rating | คะแนน 4+ ดาว จาก 5 |
| Active Installations | จำนวนผู้ใช้งาน (ยิ่งมากยิ่งดี) |
| Last Updated | อัปเดตล่าสุดไม่เกิน 3-6 เดือน |
| Tested up to | รองรับ WordPress เวอร์ชันล่าสุด |

- Plugin ที่ไม่อัปเดตนาน = **อันตราย**
- อาจมีช่องโหว่ด้านความปลอดภัย

---

## SLIDE 6: Must-Have #1 — Security Plugin
─────────────────

- **Wordfence Security**
  - Firewall ป้องกันการโจมตี
  - สแกนมัลแวร์
  - บล็อก IP ที่น่าสงสัย

- **iThemes Security**
  - Brute Force Protection
  - ป้องกันการเดารหัสผ่าน

- **สำคัญ:** เลือก 1 ตัว ห้ามลงทั้ง 2 ตัวพร้อมกัน

---

## SLIDE 7: Must-Have #2 — SEO Plugin
─────────────────

- **Yoast SEO**
  - ผู้ใช้มากที่สุดในโลก
  - เสถียร ใช้ง่าย เหมาะมือใหม่

- **RankMath**
  - ฟีเจอร์ฟรีเยอะกว่า
  - Schema Markup + Keyword Tracking

- ทั้งสองช่วย: Title, Meta Description, Sitemap
- ทำให้ Google หาเว็บไซต์เจอ

---

## SLIDE 8: Must-Have #3 — Contact Form
─────────────────

- **WPForms** — Plugin สร้างฟอร์มยอดนิยม
- ระบบ **ลากวาง** (Drag & Drop)
- เทมเพลตฟอร์มหลากหลาย
- สร้างได้: ฟอร์มติดต่อ / สมัครสมาชิก / แบบสอบถาม
- **ทุกเว็บไซต์ธุรกิจต้องมี Contact Form**
- ทำให้ลูกค้าติดต่อได้ง่าย สะดวก

---

## SLIDE 9: Must-Have #4 — Analytics
─────────────────

- **MonsterInsights** หรือ **Site Kit by Google**
- เชื่อมต่อ Google Analytics กับ WordPress
- ดูสถิติจาก Dashboard ได้เลย:
  - จำนวนผู้เข้าชม
  - แหล่งที่มาของ Traffic
  - หน้าที่ได้รับความนิยมสูงสุด
  - พฤติกรรมผู้ใช้บนเว็บ
- **ข้อมูลคือพลัง** — ตัดสินใจด้วย Data ไม่ใช่การเดา

---

## SLIDE 10: Must-Have #5 — Backup
─────────────────

- **UpdraftPlus** — Plugin สำรองข้อมูลอันดับ 1
- ตั้งค่าสำรองอัตโนมัติ: รายวัน / รายสัปดาห์
- ส่งไฟล์ไปเก็บ: **Google Drive** / **Dropbox**
- กู้คืนได้ในไม่กี่คลิก
- **"ไม่มี Backup ก็เหมือนไม่มีเว็บ"**
- ถ้าถูกแฮก/ข้อมูลหาย = ต้องทำใหม่ทั้งหมด

---

## SLIDE 11: คำเตือนสำคัญ (Important Warnings)
─────────────────

- **อย่าลง Plugin ซ้ำประเภท** — จะเกิด Conflict
  - Wordfence + iThemes = ขัดกัน
  - Yoast + RankMath = ขัดกัน
- **อย่าลง Plugin มากเกินไป** — เว็บจะช้า
  - แนะนำไม่เกิน 15-20 Plugin
- **ลบ Plugin ที่ไม่ใช้** — Deactivate อย่างเดียวไม่พอ
- ตรวจสอบอัปเดต Plugin เป็นประจำ

---

## SLIDE 12: สรุปและก้าวต่อไป (Summary & Next Steps)
─────────────────

- **Plugin 5 ประเภทที่ต้องมี:**
  1. Security (Wordfence / iThemes)
  2. SEO (Yoast / RankMath)
  3. Contact Form (WPForms)
  4. Analytics (MonsterInsights / Site Kit)
  5. Backup (UpdraftPlus)

- ประเมินคุณภาพก่อนติดตั้งเสมอ
- **ขั้นตอนถัดไป:** Plugin ขั้นสูง — Performance, Social, Page Builder

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
