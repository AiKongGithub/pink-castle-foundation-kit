# Slides: วิธีปรับแต่ง WordPress Admin Panel — WEB1-011
> **Format:** Slide Outline (13 Slides)
> **Source:** SWP3 Ch10 สร้างเว็บไซต์ Part 1 ตอนที่ 11
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## Slide 1: หน้าปก (Title Slide)

- **วิธีปรับแต่ง WordPress Admin Panel**
- SWP3 บทที่ 10: วิธีการสร้างเว็บไซต์ Part 1 — ตอนที่ 11
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

─────────────────

## Slide 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- จัดการ Dashboard Widgets ให้เป็นระเบียบ
- เข้าใจ User Roles ทั้ง 5 บทบาทและการให้สิทธิ์ที่เหมาะสม
- ตั้งค่า Settings สำคัญ (Writing, Permalinks, Reading, Discussion, Media, Privacy)
- ทำ Security Hardening เบื้องต้นเพื่อป้องกันภัยคุกคาม
- ปรับแต่ง Admin Menu ให้ใช้งานสะดวก

─────────────────

## Slide 3: Dashboard Widgets Management

- **Dashboard** = หน้าแรกของ Admin Panel
- Widget หลัก: At a Glance, Quick Draft, Activity, Events & News
- **Screen Options** (มุมขวาบน) — เลือกเปิด/ปิด Widget
- ลาก Widget เพื่อจัดลำดับใหม่ได้
- ปิด Widget ที่ไม่ใช้ → Dashboard สะอาด โฟกัสข้อมูลสำคัญ

─────────────────

## Slide 4: User Roles — 5 บทบาทหลัก

| บทบาท | สิทธิ์ |
|-------|-------|
| **Administrator** | สิทธิ์เต็มทุกอย่าง (ลบ Plugin/Theme/เว็บ) |
| **Editor** | จัดการเนื้อหาทั้งหมด รวมถึงโพสต์คนอื่น |
| **Author** | เขียนและเผยแพร่โพสต์ตัวเองได้ |
| **Contributor** | เขียนได้แต่ไม่สามารถเผยแพร่เอง |
| **Subscriber** | อ่านได้อย่างเดียว |

─────────────────

## Slide 5: หลักการกำหนด User Roles

- **หลักทอง: ให้สิทธิ์เท่าที่จำเป็นเท่านั้น**
- อย่าให้ทุกคนเป็น Administrator
- นักเขียน → กำหนดเป็น **Author**
- คนส่งบทความมาตรวจ → กำหนดเป็น **Contributor**
- ทบทวน User Roles เป็นประจำ ลบบัญชีที่ไม่ใช้แล้ว

─────────────────

## Slide 6: Writing Settings & Permalinks

- **Writing Settings** (Settings > Writing)
  - Default Post Category
  - Default Post Format
- **Permalinks** (Settings > Permalinks)
  - แนะนำ: **Post name** (yoursite.com/sample-post/)
  - ดีต่อ SEO — URL อ่านง่ายและมีคำสำคัญ
  - ตั้งตั้งแต่วันแรก — เปลี่ยนภายหลังเสีย SEO

─────────────────

## Slide 7: Reading Settings

- เข้าที่ **Settings > Reading**
- **Your latest posts** — หน้าแรกแสดงบทความล่าสุด
  - เหมาะกับเว็บ Blog
- **A static page** — เลือกหน้าเฉพาะเป็น Homepage
  - เหมาะกับเว็บธุรกิจ
- ตั้งค่า Posts page สำหรับหน้า Blog แยก
- กำหนดจำนวนบทความต่อหน้าได้

─────────────────

## Slide 8: Discussion Settings (Comments)

- เข้าที่ **Settings > Discussion**
- ตัวเลือกสำคัญ:
  - เปิดหรือปิด Comments ทั้งเว็บ
  - ตั้ง **Manual Approval** ก่อนแสดง Comment
  - จำกัดลิงก์ใน Comment เพื่อลด Spam
- เว็บธุรกิจ: พิจารณา **ปิด Comments** เพื่อลดภาระดูแล
- ถ้าเปิด: ใช้ **Akismet** กรอง Spam

─────────────────

## Slide 9: Media Settings

- เข้าที่ **Settings > Media**
- WordPress สร้างรูป **3 ขนาด** อัตโนมัติเมื่ออัปโหลด:
  - **Thumbnail** — รูปย่อ (เช่น 150x150 px)
  - **Medium** — ขนาดกลาง (เช่น 300x300 px)
  - **Large** — ขนาดใหญ่ (เช่น 1024x1024 px)
- ขนาดที่ไม่ต้องการ → ตั้งเป็น **0** เพื่อประหยัดพื้นที่

─────────────────

## Slide 10: Privacy Settings

- เข้าที่ **Settings > Privacy**
- สร้าง **Privacy Policy Page** จากเทมเพลตที่มีให้
- **ข้อบังคับทางกฎหมาย**: GDPR (EU), PDPA (ไทย)
- เว็บที่เก็บข้อมูลส่วนบุคคล **ต้องมี** Privacy Policy
- ปรับเนื้อหาให้ตรงกับข้อมูลที่เว็บเก็บจริง

─────────────────

## Slide 11: Security Hardening

- **เปลี่ยน Username** จาก "admin" เป็นชื่ออื่น
- **รหัสผ่านแข็งแกร่ง** — 12+ ตัวอักษร ผสมตัวพิมพ์เล็ก-ใหญ่ ตัวเลข สัญลักษณ์
- **จำกัด Login attempts** — 3-5 ครั้ง แล้วล็อค
- **อัปเดตสม่ำเสมอ** — WordPress, Theme, Plugin ทุกตัว
- สำรองข้อมูล (Backup) ก่อนอัปเดตทุกครั้ง

─────────────────

## Slide 12: Admin Menu Customization

- เมนูด้านซ้ายของ Admin Panel
- ใช้ Plugin: **Admin Menu Editor**
  - ซ่อนเมนูที่ไม่ได้ใช้
  - เปลี่ยนชื่อเมนู
  - จัดลำดับเมนูใหม่
  - กำหนดสิทธิ์เข้าถึงตาม User Role
- เมนูเรียบง่าย → ทำงานได้เร็วขึ้น

─────────────────

## Slide 13: สรุปและก้าวต่อไป (Summary & Next Steps)

- WordPress Admin Panel คือ **ศูนย์บัญชาการ** ของเว็บไซต์
- ตั้งค่า **Permalinks** และ **Security** ตั้งแต่วันแรก
- ให้ **User Roles** เท่าที่จำเป็น — ไม่ให้ทุกคนเป็น Admin
- จัดการ **Dashboard, Settings, Privacy** ให้ครบถ้วน
- **Action Item:** กลับไปตรวจสอบ Settings ของเว็บคุณวันนี้

---

*จำนวน Slides ทั้งหมด: 13 สไลด์*
