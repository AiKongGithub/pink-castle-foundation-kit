# Quiz: วิธีปรับแต่ง WordPress Admin Panel — WEB1-011
> **Format:** Multiple Choice Quiz (10 Questions)
> **Source:** SWP3 Ch10 สร้างเว็บไซต์ Part 1 ตอนที่ 11
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## คำชี้แจง
- ข้อ 1-6: เลือกคำตอบที่ถูกต้องที่สุดเพียงข้อเดียว (A, B, C หรือ D)
- ข้อ 7-9: ตอบ "ถูก" หรือ "ผิด"
- ข้อ 10: เติมคำในช่องว่าง

---

### ข้อ 1: WordPress มี User Roles ทั้งหมดกี่บทบาท?

A) 3 บทบาท (Admin, Editor, Subscriber)
B) 4 บทบาท (Admin, Editor, Author, Subscriber)
C) 5 บทบาท (Administrator, Editor, Author, Contributor, Subscriber)
D) 6 บทบาท (Super Admin, Admin, Editor, Author, Contributor, Subscriber)

---

### ข้อ 2: Permalinks ควรตั้งค่าแบบใดเพื่อ SEO ที่ดี?

A) Plain (?p=123)
B) Day and name (/2026/02/17/sample-post/)
C) Post name (/sample-post/)
D) Numeric (/archives/123)

---

### ข้อ 3: Reading Settings ตัวเลือก "A static page" เหมาะกับเว็บไซต์ประเภทใด?

A) เว็บ Blog ส่วนตัว
B) เว็บธุรกิจที่ต้องการ Homepage สวยงาม
C) เว็บ Forum สำหรับชุมชน
D) เว็บข่าวที่อัปเดตบทความทุกวัน

---

### ข้อ 4: ข้อใดเป็นมาตรการ Security Hardening ที่ควรทำ?

A) ใช้ Username เป็น "admin" เพื่อจำง่าย
B) ติดตั้ง Plugin ให้มากที่สุดเพื่อเพิ่มฟีเจอร์
C) เปลี่ยน Username จาก admin + ใช้รหัสผ่านแข็งแกร่ง + จำกัด Login attempts
D) ปิดการอัปเดตอัตโนมัติเพื่อป้องกัน Plugin เสีย

---

### ข้อ 5: Dashboard Widgets จัดการได้ผ่านเมนูใด?

A) Settings > General
B) Appearance > Customize
C) Screen Options (มุมขวาบนของ Dashboard)
D) Plugins > Installed Plugins

---

### ข้อ 6: Media Settings ใน WordPress สร้างรูปภาพอัตโนมัติกี่ขนาดเมื่ออัปโหลด?

A) 1 ขนาด (Original)
B) 2 ขนาด (Thumbnail, Full)
C) 3 ขนาด (Thumbnail, Medium, Large)
D) 4 ขนาด (Thumbnail, Small, Medium, Large)

---

### ข้อ 7: (ถูก/ผิด) Contributor สามารถเขียนและเผยแพร่บทความได้ด้วยตนเอง

---

### ข้อ 8: (ถูก/ผิด) การเปลี่ยน Permalinks หลังจากเว็บถูก Index ใน Search Engine แล้ว อาจทำให้ URL เดิมกลายเป็น 404 Not Found และเสียอันดับ SEO

---

### ข้อ 9: (ถูก/ผิด) เว็บไซต์ที่เก็บข้อมูลส่วนบุคคลของผู้ใช้ไม่จำเป็นต้องมีหน้า Privacy Policy

---

### ข้อ 10: (เติมคำ) WordPress มี 5 User Roles เรียงจากสิทธิ์สูงสุดไปต่ำสุด ได้แก่ Administrator, Editor, Author, ____________ และ Subscriber

---

## เฉลย (Answer Key)

| ข้อ | คำตอบ | คำอธิบายสั้น |
|-----|-------|-------------|
| 1 | **C** | WordPress มี 5 บทบาท: Administrator, Editor, Author, Contributor, Subscriber |
| 2 | **C** | Post name (/sample-post/) อ่านง่ายและดีต่อ SEO ที่สุด |
| 3 | **B** | Static page เหมาะกับเว็บธุรกิจที่ต้องการ Homepage ออกแบบเฉพาะ |
| 4 | **C** | เปลี่ยน Username + รหัสผ่านแข็งแกร่ง + จำกัด Login attempts คือมาตรการพื้นฐาน |
| 5 | **C** | Screen Options อยู่มุมขวาบนของ Dashboard ใช้จัดการ Widgets |
| 6 | **C** | WordPress สร้างรูป 3 ขนาดอัตโนมัติ: Thumbnail, Medium, Large |
| 7 | **ผิด** | Contributor เขียนได้แต่ไม่สามารถเผยแพร่เอง ต้องรอ Editor/Admin อนุมัติ |
| 8 | **ถูก** | URL เดิมจะเป็น 404 ถ้าไม่ทำ Redirect ส่งผลเสียต่อ SEO อย่างมาก |
| 9 | **ผิด** | กฎหมาย GDPR/PDPA กำหนดให้ต้องมี Privacy Policy สำหรับเว็บที่เก็บข้อมูลส่วนบุคคล |
| 10 | **Contributor** | เรียงจากสิทธิ์สูงไปต่ำ: Administrator > Editor > Author > Contributor > Subscriber |

---

**เกณฑ์การประเมิน:**
| คะแนน | ระดับ | คำแนะนำ |
|--------|-------|---------|
| 9-10 | ดีเยี่ยม | พร้อมไปตอนถัดไป |
| 7-8 | ดี | ทบทวนจุดที่พลาดเล็กน้อย |
| 5-6 | พอใช้ | ควรทบทวนเนื้อหาอีกครั้ง |
| ต่ำกว่า 5 | ต้องปรับปรุง | แนะนำให้ดูวิดีโอซ้ำและอ่าน Executive Summary |
