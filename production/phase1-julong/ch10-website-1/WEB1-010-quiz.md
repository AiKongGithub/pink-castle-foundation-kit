# Quiz: วิธีติดตั้ง WP-Rocket Plugin — WEB1-010
> **Format:** Multiple Choice Quiz (10 Questions)
> **Source:** SWP3 Ch10 สร้างเว็บไซต์ Part 1 ตอนที่ 10
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## คำชี้แจง
- ข้อ 1-6: เลือกคำตอบที่ถูกต้องที่สุดเพียงข้อเดียว (A, B, C หรือ D)
- ข้อ 7-9: ตอบ "ถูก" หรือ "ผิด"
- ข้อ 10: เติมคำในช่องว่าง

---

### ข้อ 1: ถ้าเว็บไซต์โหลดนานเกินกี่วินาที ผู้เยี่ยมชมกว่าครึ่งจะกดปิดหน้าเว็บ?

A) 1 วินาที
B) 3 วินาที
C) 5 วินาที
D) 10 วินาที

---

### ข้อ 2: WP-Rocket จัดอยู่ในประเภท Plugin ใด?

A) Security Plugin
B) SEO Plugin
C) Caching Plugin
D) Backup Plugin

---

### ข้อ 3: Lazy Loading ทำงานอย่างไร?

A) โหลดรูปภาพทั้งหมดในหน้าเว็บพร้อมกันตั้งแต่เปิด
B) บีบอัดรูปภาพให้มีขนาดเล็กลงก่อนแสดงผล
C) โหลดรูปภาพเฉพาะเมื่อผู้ใช้เลื่อนหน้าจอลงไปถึงตำแหน่งนั้น
D) แปลงรูปภาพทั้งหมดเป็นรูปแบบ WebP อัตโนมัติ

---

### ข้อ 4: ข้อใดเป็นข้อจำกัดของ LiteSpeed Cache เมื่อเทียบกับ WP-Rocket?

A) ไม่มี Page Caching
B) ต้องใช้กับ LiteSpeed Web Server จึงจะใช้งานได้เต็มประสิทธิภาพ
C) เป็น Plugin ที่ต้องเสียเงินซื้อ
D) ไม่รองรับ WordPress เวอร์ชันใหม่

---

### ข้อ 5: ฟีเจอร์ใดของ WP-Rocket ที่ช่วยล้างข้อมูลไม่จำเป็นออกจากฐานข้อมูล?

A) Page Caching
B) Browser Caching
C) Database Optimization
D) GZIP Compression

---

### ข้อ 6: ควรใช้เครื่องมือใดในการทดสอบความเร็วเว็บไซต์?

A) Google Analytics และ Facebook Pixel
B) Google PageSpeed Insights และ GTmetrix
C) Google Search Console และ Yoast SEO
D) WordPress Health Check และ phpMyAdmin

---

### ข้อ 7: (ถูก/ผิด) WP-Rocket เป็น Plugin ฟรีที่สามารถดาวน์โหลดจาก WordPress Plugin Directory ได้

---

### ข้อ 8: (ถูก/ผิด) การเปิด Minify CSS/JS อาจทำให้ CSS หรือ JavaScript บางตัวทำงานผิดปกติได้ จึงต้องทดสอบหลังเปิดใช้งาน

---

### ข้อ 9: (ถูก/ผิด) การติดตั้ง Caching Plugin เพียงตัวเดียวเพียงพอแล้วสำหรับการทำให้เว็บไซต์เร็วที่สุด

---

### ข้อ 10: (เติมคำ) GZIP Compression ทำหน้าที่ ____________ ไฟล์ของเว็บไซต์ให้มีขนาดเล็กลงก่อนส่งไปยังเบราว์เซอร์ของผู้ใช้

---

## เฉลย (Answer Key)

| ข้อ | คำตอบ | คำอธิบายสั้น |
|-----|-------|-------------|
| 1 | **B** | เว็บโหลดเกิน 3 วินาที ผู้เยี่ยมชมกว่าครึ่งจะออกจากเว็บทันที |
| 2 | **C** | WP-Rocket เป็น Premium Caching Plugin สำหรับ WordPress |
| 3 | **C** | Lazy Loading โหลดรูปเฉพาะเมื่อผู้ใช้เลื่อนลงไปถึงตำแหน่งนั้น |
| 4 | **B** | LiteSpeed Cache ต้องใช้กับ LiteSpeed Server จึงจะเต็มประสิทธิภาพ |
| 5 | **C** | Database Optimization ล้าง Post Revisions, Spam Comments ฯลฯ |
| 6 | **B** | Google PageSpeed Insights และ GTmetrix ใช้วัดความเร็วเว็บไซต์ |
| 7 | **ผิด** | WP-Rocket เป็น Premium Plugin ต้องซื้อ License จาก wp-rocket.me |
| 8 | **ถูก** | Minify อาจทำให้โค้ดบางตัวทำงานผิดปกติ ต้องทดสอบทุกครั้ง |
| 9 | **ผิด** | ต้อง Optimize เรื่องอื่นด้วย เช่น ขนาดรูปภาพ คุณภาพ Hosting จำนวน Plugin |
| 10 | **บีบอัด** | GZIP Compression บีบอัดไฟล์ให้เล็กลงก่อนส่งให้ผู้ใช้ |

---

**เกณฑ์การประเมิน:**
| คะแนน | ระดับ | คำแนะนำ |
|--------|-------|---------|
| 9-10 | ดีเยี่ยม | พร้อมไปตอนถัดไป |
| 7-8 | ดี | ทบทวนจุดที่พลาดเล็กน้อย |
| 5-6 | พอใช้ | ควรทบทวนเนื้อหาอีกครั้ง |
| ต่ำกว่า 5 | ต้องปรับปรุง | แนะนำให้ดูวิดีโอซ้ำและอ่าน Executive Summary |
