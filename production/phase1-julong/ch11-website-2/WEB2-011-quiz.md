# Quiz: วิธีติดตั้ง Google Analytics — WEB2-011
> **Format:** Multiple Choice Quiz (10 Questions)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 11
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## คำชี้แจง
- ข้อ 1-6: เลือกคำตอบที่ถูกต้องที่สุดเพียงข้อเดียว (Multiple Choice)
- ข้อ 7-9: ตอบ ถูก (True) หรือ ผิด (False)
- ข้อ 10: เติมคำตอบ (Fill in the blank)

---

### ข้อ 1: ในการสร้าง Google Analytics Account สำหรับเว็บไซต์ในประเทศไทย ควรตั้ง Time Zone และ Currency เป็นอะไร?

A) Time Zone: UTC+0 / Currency: USD
B) Time Zone: (GMT+07:00) Bangkok / Currency: Thai Baht (THB)
C) Time Zone: (GMT+08:00) Singapore / Currency: Thai Baht (THB)
D) Time Zone: (GMT+07:00) Bangkok / Currency: US Dollar (USD)

---

### ข้อ 2: Measurement ID ของ Google Analytics GA4 มีรูปแบบอย่างไร?

A) UA-XXXXXXXXX-X
B) AW-XXXXXXXXXX
C) G-XXXXXXXXXX
D) GT-XXXXXXXXXX

---

### ข้อ 3: วิธีใดง่ายที่สุดในการติดตั้ง Google Analytics บน WordPress?

A) แก้ไขไฟล์ functions.php โดยตรง
B) ใช้ Google Tag Manager
C) ใส่โค้ด gtag.js ในส่วน header.php ด้วยตนเอง
D) ใช้ปลั๊กอิน Site Kit by Google

---

### ข้อ 4: ถ้าเว็บไซต์มีผู้เข้าชม 1 คนเข้ามา 5 ครั้งในวันเดียว จะนับเป็นเท่าไรใน Analytics?

A) 5 Users, 5 Sessions
B) 1 User, 1 Session
C) 1 User, 5 Sessions
D) 5 Users, 1 Session

---

### ข้อ 5: Bounce Rate ที่ถือว่า "ต้องปรับปรุง" คือเท่าไร?

A) ต่ำกว่า 20%
B) 26-40%
C) 41-55%
D) มากกว่า 70%

---

### ข้อ 6: ข้อใดไม่ใช่ตัวอย่างของ Conversion Tracking?

A) การซื้อสินค้าสำเร็จ
B) การกรอกฟอร์มติดต่อ
C) จำนวน Impressions ในผลค้นหา
D) การสมัครสมาชิกจดหมายข่าว

---

### ข้อ 7: (True/False) Google Tag Manager เหมาะสำหรับเว็บไซต์ที่ต้องติดตั้ง tag หลายตัว เช่น Analytics, Facebook Pixel และ Google Ads Conversion Tag

---

### ข้อ 8: (True/False) การแก้ไข Time Zone ของ Google Analytics Property จะส่งผลย้อนหลังกับข้อมูลที่เก็บไปแล้ว

---

### ข้อ 9: (True/False) ตามกฎหมาย PDPA เว็บไซต์ที่ติดตั้ง Google Analytics ต้องมี Cookie Consent Banner เพื่อขอความยินยอมจากผู้ใช้

---

### ข้อ 10: (Fill in the blank) ตัวเลขสำคัญ 4 ตัวใน Google Analytics ที่ต้องติดตาม ได้แก่ Users, Sessions, ________ และ Pages per Session

---

## เฉลย (Answer Key)

| ข้อ | คำตอบ | คำอธิบาย |
|-----|-------|----------|
| 1 | **B** | เว็บไซต์ไทยต้องตั้ง Time Zone เป็น Bangkok (GMT+07:00) และ Currency เป็น THB เพื่อให้รายงานถูกต้อง |
| 2 | **C** | GA4 ใช้ Measurement ID รูปแบบ G-XXXXXXXXXX ส่วน UA- เป็นของ Universal Analytics เวอร์ชันเก่า |
| 3 | **D** | Site Kit by Google เป็นวิธีง่ายที่สุด ไม่ต้องแก้โค้ด แค่เชื่อมต่อ Google Account |
| 4 | **C** | 1 คนนับเป็น 1 User เสมอ แต่เข้า 5 ครั้งนับเป็น 5 Sessions |
| 5 | **D** | Bounce Rate มากกว่า 70% ถือว่าต้องปรับปรุง 26-40% ถือว่าดี 41-55% เป็นค่าเฉลี่ย |
| 6 | **C** | Impressions เป็นข้อมูลของ Search Console ไม่ใช่ Conversion Tracking ซึ่งวัดเป้าหมายทางธุรกิจ |
| 7 | **True** | GTM ช่วยจัดการ tag ทุกประเภทจากที่เดียว ติดตั้ง GTM ครั้งเดียว แล้วเพิ่ม tag ผ่าน interface |
| 8 | **False** | การแก้ไข Time Zone จะมีผลเฉพาะข้อมูลใหม่ตั้งแต่วันที่แก้ ไม่ย้อนหลังข้อมูลเก่า |
| 9 | **True** | PDPA กำหนดให้ต้องแจ้งและขอความยินยอมก่อนเก็บ Cookie โทษปรับสูงสุด 5 ล้านบาท |
| 10 | **Bounce Rate** | 4 ตัวเลขหลักคือ Users, Sessions, Bounce Rate และ Pages per Session |

---

**เกณฑ์การประเมิน:**
| คะแนน | ระดับ | คำแนะนำ |
|--------|-------|---------|
| 9-10 | ดีเยี่ยม | พร้อมไปตอนถัดไป |
| 7-8 | ดี | ทบทวนจุดที่พลาดเล็กน้อย |
| 5-6 | พอใช้ | ควรทบทวนเนื้อหาอีกครั้ง |
| ต่ำกว่า 5 | ต้องปรับปรุง | แนะนำให้ดูวิดีโอซ้ำและอ่าน Executive Summary |
