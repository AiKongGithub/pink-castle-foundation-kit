# Quiz: วิธีตั้งค่า Plugin Jetpack — WEB2-008
> **Format:** Multiple Choice Quiz (10 Questions)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 8
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## คำชี้แจง
เลือกคำตอบที่ถูกต้องที่สุด (Multiple Choice / True-False / Fill-in)

---

### ข้อ 1: Jetpack ถูกพัฒนาโดยบริษัทใด? (MC)

A) Google
B) Automattic (ทีมเดียวกับ WordPress.com)
C) Facebook
D) Microsoft

---

### ข้อ 2: สิ่งแรกที่ต้องทำหลังติดตั้ง Jetpack คืออะไร? (MC)

A) ซื้อแพลนเสียเงิน
B) เชื่อมต่อกับบัญชี WordPress.com
C) ปิด module ทั้งหมดก่อน
D) ติดตั้ง Akismet เพิ่ม

---

### ข้อ 3: จริงหรือไม่ — Brute Force Protection ใน Jetpack ป้องกันการสุ่มรหัสผ่านเพื่อเข้าสู่ระบบ (TF)

A) จริง
B) ไม่จริง

---

### ข้อ 4: Downtime Monitoring ตรวจสอบเว็บไซต์ทุกกี่นาที? (MC)

A) ทุก 1 นาที
B) ทุก 5 นาที
C) ทุก 30 นาที
D) ทุก 1 ชั่วโมง

---

### ข้อ 5: Site Accelerator ใน Jetpack ทำหน้าที่อะไร? (MC)

A) เร่งความเร็วในการเขียนบทความ
B) Serve รูปภาพและ Static Files ผ่าน CDN ของ WordPress.com
C) บีบอัดฐานข้อมูลให้เล็กลง
D) เร่งความเร็วในการ index ของ Google

---

### ข้อ 6: จริงหรือไม่ — Publicize ใน Jetpack คือฟีเจอร์ที่แชร์บทความไป Social Media อัตโนมัติเมื่อ publish (TF)

A) จริง
B) ไม่จริง

---

### ข้อ 7: ข้อใดเป็นฟีเจอร์ที่ต้องอัปเกรดเป็นแพลนเสียเงิน? (MC)

A) Brute Force Protection
B) Site Stats
C) Automated Backup และ Malware Scanning
D) Related Posts

---

### ข้อ 8: ทำไมควรปิด module ที่ไม่ได้ใช้ใน Jetpack? (MC)

A) เพราะ module ที่เปิดมากเกินไปจะทำให้ Jetpack หมดอายุเร็ว
B) เพราะแต่ละ module ใช้ทรัพยากร ทำให้เว็บหนักเปล่าๆ
C) เพราะ WordPress.com จะเก็บค่าบริการเพิ่มตาม module
D) เพราะ module จะทำให้เว็บถูก hack ง่ายขึ้น

---

### ข้อ 9: Jetpack มีฟีเจอร์หลัก 3 ด้าน ได้แก่ Security, _______ และ Traffic (Fill-in)

คำตอบ: _______

---

### ข้อ 10: จริงหรือไม่ — แพลนฟรีของ Jetpack เพียงพอสำหรับเว็บไซต์ทั่วไป (TF)

A) จริง
B) ไม่จริง

---

## เฉลย (Answer Key)

| ข้อ | คำตอบ | คำอธิบายสั้น |
|-----|-------|-------------|
| 1 | **B** | Jetpack พัฒนาโดย Automattic ซึ่งเป็นบริษัทเดียวกับ WordPress.com |
| 2 | **B** | ต้องเชื่อมต่อกับบัญชี WordPress.com ก่อน เพราะหลายฟีเจอร์ทำงานผ่าน cloud |
| 3 | **A** | Brute Force Protection บล็อก IP ที่พยายามสุ่มรหัสผ่านล็อกอินอัตโนมัติ |
| 4 | **B** | Downtime Monitoring ตรวจเว็บทุก 5 นาที แจ้งเตือน email ทันทีถ้าเว็บล่ม |
| 5 | **B** | Site Accelerator = CDN ฟรี serve รูปภาพและ Static Files ผ่านเครือข่าย WordPress.com |
| 6 | **A** | Publicize แชร์บทความไป Social Media อัตโนมัติทันทีที่กด publish |
| 7 | **C** | Automated Backup และ Malware Scanning เป็นฟีเจอร์ของแพลนเสียเงิน |
| 8 | **B** | module ที่เปิดแต่ไม่ได้ใช้จะใช้ทรัพยากรเปล่าๆ ทำให้เว็บหนักขึ้นโดยไม่จำเป็น |
| 9 | **Performance** | Jetpack มี 3 ด้านหลัก คือ Security, Performance และ Traffic |
| 10 | **A** | แพลนฟรีได้ Brute Force, Downtime, CDN, Lazy Images, Stats, Related Posts, Sharing ครบ |

---

**เกณฑ์การประเมิน:**
| คะแนน | ระดับ | คำแนะนำ |
|--------|-------|---------|
| 9-10 | ดีเยี่ยม | พร้อมไปตอนถัดไป |
| 7-8 | ดี | ทบทวนจุดที่พลาดเล็กน้อย |
| 5-6 | พอใช้ | ควรทบทวนเนื้อหาอีกครั้ง |
| ต่ำกว่า 5 | ต้องปรับปรุง | แนะนำให้ดูวิดีโอซ้ำและอ่าน Executive Summary |
