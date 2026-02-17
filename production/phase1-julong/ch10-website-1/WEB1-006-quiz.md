# Quiz: แนะนำ cPanel และติดตั้ง WordPress — WEB1-006
> **Format:** Multiple Choice Quiz (10 Questions)
> **Source:** SWP3 Ch10 สร้างเว็บไซต์ Part 1 ตอนที่ 6
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## คำชี้แจง
เลือกคำตอบที่ถูกต้องที่สุด (Multiple Choice 6 ข้อ / True-False 3 ข้อ / Fill-in-Blank 1 ข้อ)

---

### ข้อ 1: (Multiple Choice) cPanel คืออะไร?

A) โปรแกรมสำหรับเขียนโค้ดเว็บไซต์
B) แผงควบคุมเว็บโฮสติ้งแบบกราฟิกที่ใช้จัดการไฟล์ ฐานข้อมูล โดเมน และอื่นๆ
C) ระบบจัดการเนื้อหาเว็บไซต์ (CMS) เหมือน WordPress
D) เครื่องมือสำหรับออกแบบหน้าตาเว็บไซต์

---

### ข้อ 2: (Multiple Choice) เข้า cPanel ได้โดยพิมพ์ URL อะไร?

A) yourdomain.com/cpanel
B) yourdomain.com:2083
C) yourdomain.com/admin
D) yourdomain.com:8080

---

### ข้อ 3: (True/False) Softaculous คือเครื่องมือสำหรับเขียนโค้ด WordPress

A) True — Softaculous ใช้เขียนโค้ด WordPress
B) False — Softaculous คือ Auto Installer ที่ช่วยติดตั้ง WordPress แบบ one-click โดยไม่ต้องเขียนโค้ด

---

### ข้อ 4: (Multiple Choice) ถ้าต้องการให้ WordPress เป็นหน้าหลักของเว็บไซต์ ช่อง "In Directory" ต้องกรอกอย่างไร?

A) พิมพ์ "wp" ลงไป
B) พิมพ์ "wordpress" ลงไป
C) เว้นว่างไว้ (ลบค่าเริ่มต้นออก)
D) พิมพ์ชื่อโดเมนลงไป

---

### ข้อ 5: (Multiple Choice) ทำไมไม่ควรใช้ "admin" เป็น Admin Username?

A) เพราะ WordPress ไม่อนุญาตให้ใช้ชื่อนี้
B) เพราะจะทำให้ระบบทำงานช้าลง
C) เพราะเป็นชื่อที่แฮกเกอร์ลองโจมตีเป็นอันดับแรก
D) เพราะชื่อนี้ถูกสงวนไว้สำหรับผู้ดูแลระบบโฮสติ้ง

---

### ข้อ 6: (True/False) Table Prefix ค่าเริ่มต้นคือ wp_ ซึ่งแนะนำให้เปลี่ยนเป็นค่าอื่นเพื่อความปลอดภัย

A) True — เปลี่ยน Table Prefix ช่วยป้องกันการโจมตีฐานข้อมูล
B) False — ค่า wp_ ปลอดภัยเพียงพอแล้ว ไม่จำเป็นต้องเปลี่ยน

---

### ข้อ 7: (Multiple Choice) หลังติดตั้ง WordPress สำเร็จ เข้า Admin Dashboard ผ่าน URL ใด?

A) yourdomain.com/dashboard
B) yourdomain.com/admin
C) yourdomain.com/wp-admin
D) yourdomain.com/login

---

### ข้อ 8: (Multiple Choice) Permalink Structure ที่แนะนำให้ตั้งคือแบบใด?

A) Plain (?p=123)
B) Day and Name (/2026/02/17/post-name/)
C) Post Name (/post-name/)
D) Numeric (/archives/123)

---

### ข้อ 9: (True/False) WordPress ไม่รองรับภาษาไทย ต้องติดตั้ง Plugin แปลภาษาเพิ่ม

A) True — WordPress รองรับเฉพาะภาษาอังกฤษ ต้องใช้ Plugin แปลภาษา
B) False — WordPress รองรับภาษาไทยอย่างสมบูรณ์ เลือกได้ตั้งแต่ตอนติดตั้ง

---

### ข้อ 10: (Fill-in-Blank) เมนู __________ ใน WordPress Dashboard ใช้สำหรับเปลี่ยนธีมและออกแบบหน้าตาของเว็บไซต์

---

## เฉลย (Answer Key)

| ข้อ | ประเภท | คำตอบ | คำอธิบายสั้น |
|-----|--------|-------|-------------|
| 1 | MC | **B** | cPanel = แผงควบคุมโฮสติ้งแบบ GUI |
| 2 | MC | **B** | เข้า cPanel ผ่าน domain:2083 |
| 3 | T/F | **B (False)** | Softaculous = Auto Installer ไม่ใช่เครื่องมือเขียนโค้ด |
| 4 | MC | **C** | In Directory ว่าง = WordPress เป็นหน้าหลัก |
| 5 | MC | **C** | "admin" เป็นเป้าหมายแรกของ Brute Force Attack |
| 6 | T/F | **A (True)** | เปลี่ยน Table Prefix เพิ่มความปลอดภัยฐานข้อมูล |
| 7 | MC | **C** | Admin Dashboard เข้าผ่าน /wp-admin |
| 8 | MC | **C** | Post Name ให้ URL อ่านง่ายและดีต่อ SEO |
| 9 | T/F | **B (False)** | WordPress รองรับภาษาไทยสมบูรณ์ในตัว |
| 10 | Fill | **Appearance** | Appearance ใช้เปลี่ยนธีมและดีไซน์ |

---

**สัดส่วนข้อสอบ:** MC 60% (6 ข้อ) | T/F 30% (3 ข้อ) | Fill-in-Blank 10% (1 ข้อ)

**เกณฑ์การประเมิน:**
| คะแนน | ระดับ | คำแนะนำ |
|--------|-------|---------|
| 9-10 | ดีเยี่ยม | พร้อมไปตอนถัดไป |
| 7-8 | ดี | ทบทวนจุดที่พลาดเล็กน้อย |
| 5-6 | พอใช้ | ควรทบทวนเนื้อหาอีกครั้ง |
| ต่ำกว่า 5 | ต้องปรับปรุง | แนะนำให้ดูวิดีโอซ้ำและอ่าน Executive Summary |
