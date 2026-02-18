# วิธีตั้งค่า Membership System — SOMT-006
> **Format:** Slide Deck (12 slides)
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 6
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

### SLIDE 1: หน้าปก
# วิธีตั้งค่า Membership System
## Configuration ระบบสมาชิกให้พร้อมรับสมาชิก
**SWP3 บทที่ 30 — ตอนที่ 6 (6:27 นาที)**
PinkCastle Academy

---

### SLIDE 2: ทำไมต้องตั้งค่าให้ดี?
## First Impression ตัดสินทุกอย่าง
- สมาชิกตัดสินใจอยู่หรือไป **ภายใน 5 นาทีแรก**
- ระบบที่ดูไม่มืออาชีพ = ขาดความน่าเชื่อถือ
- Configuration ที่ดี **ลดภาระ Support 50%+**
- ลงทุน 2-3 ชั่วโมง ประหยัดเวลาหลายสิบชั่วโมง

> *"ตั้งค่าครั้งเดียว ใช้ได้ตลอดชีวิตระบบ"*

---

### SLIDE 3: Branding Settings
## สร้าง Brand Consistency ทั้งระบบ
| รายการ | รายละเอียด |
|--------|-----------|
| **โลโก้** | PNG + SVG สำหรับ Web |
| **Color Scheme** | Primary, Secondary, Accent |
| **Favicon** | ไอคอนบน Browser Tab |
| **Custom Domain** | members.yourbrand.com |
| **Font** | สอดคล้องกับแบรนด์ |

> สมาชิกต้องรู้สึกว่าอยู่ **แบรนด์เดียวกัน** ทุกหน้า

---

### SLIDE 4: Email Notifications — 4 ประเภท
## อีเมลที่ต้อง Customize ทุกฉบับ
```
1. Welcome Email      → ต้อนรับ + Next Steps + Login Info
2. New Content Alert   → แจ้งเมื่อมีบทเรียนใหม่
3. Payment Reminder    → แจ้งก่อนเรียกเก็บเงิน
4. Failed Payment      → แจ้งเมื่อชำระไม่สำเร็จ
```

**สำคัญ:** อย่าใช้ Default ภาษาอังกฤษ ถ้ากลุ่มเป้าหมายเป็นคนไทย!

---

### SLIDE 5: Welcome Email — อีเมลที่สำคัญที่สุด
## 3 หน้าที่ของ Welcome Email
1. **ต้อนรับ** — ทำให้รู้สึกตื่นเต้นที่เข้ามา
2. **Next Steps** — บอกชัดเจนว่าต้องทำอะไร
3. **Login Info** — ลิงก์และวิธีเข้าสู่ระบบ

### เป้าหมาย:
> สมาชิกต้อง Login และเริ่มเรียน **ภายใน 24 ชั่วโมงแรก**

---

### SLIDE 6: Member Dashboard Layout
## 3-Click Rule — ทุกอย่างหาเจอใน 3 คลิก
| ส่วน | แสดงอะไร | ทำไมสำคัญ |
|------|----------|----------|
| **บทเรียน** | รายการหลักสูตรทั้งหมด | สมาชิกรู้ว่ามีอะไรบ้าง |
| **Progress** | แถบ % ที่เรียนไปแล้ว | สร้างแรงจูงใจเรียนต่อ |
| **ใหม่** | ไฮไลท์เนื้อหาล่าสุด | ดึงให้กลับมาเรียน |

---

### SLIDE 7: Login Page Customization
## ไม่ใช่แค่ฟอร์ม Username/Password
- **โลโก้แบรนด์** ชัดเจน
- **Welcome Message** สร้างความรู้สึกดี
- **ภาพสร้างแรงบันดาลใจ** ทำให้ตื่นเต้น
- **ฟอร์ม Login** เรียบง่าย ใช้ง่าย

> Login Page ที่ดี = สมาชิก **ตื่นเต้นทุกครั้ง** ที่เข้าเรียน

---

### SLIDE 8: Security Settings
## ป้องกัน Account Sharing
| Setting | ค่าที่แนะนำ | ผลลัพธ์ |
|---------|------------|---------|
| **Password** | 8+ ตัว + ตัวพิเศษ | รหัสแข็งแรง |
| **Session Timeout** | 30-60 นาที | ป้องกันลืม Logout |
| **Device Limit** | 2-3 เครื่อง | ยืดหยุ่นแต่ปลอดภัย |
| **IP Restriction** | เปิดเฉพาะคอร์สแพง | ป้องกันสูงสุด |

---

### SLIDE 9: Mobile Responsiveness
## 60-70% ของสมาชิกเข้าผ่านมือถือ
### ต้องทดสอบ:
- Login Page บนมือถือ
- Dashboard บนมือถือ
- บทเรียน/วิดีโอ บนมือถือ

### ต้องทดสอบบน:
- iOS (Safari)
- Android (Chrome)
- **มือถือจริง** ไม่ใช่แค่ Responsive Mode

> Mobile ใช้ยาก = สมาชิกเลิกเข้าเรียน **ภายใน 1 สัปดาห์**

---

### SLIDE 10: Best Practice — Test Account
## ลอง Login เป็นสมาชิกเอง
1. สร้าง Test Account ด้วยอีเมลทดสอบ
2. ลอง Login → ดู Welcome Email
3. ดู Dashboard → หาบทเรียน
4. ลองเรียน 1-2 บทเรียน
5. ลองบนมือถือ

> **ถ้าตัวเองยังงง = สมาชิกจริงจะงงมากกว่า**

---

### SLIDE 11: Configuration Checklist
## 6 ข้อก่อนเปิดระบบ
1. Branding ครบถ้วน (โลโก้ สี Font)
2. Email Notifications Customize แล้ว
3. Dashboard Layout ชัดเจน (3-Click Rule)
4. Login Page มีแบรนด์ชัดเจน
5. Security Settings เหมาะสม (Device Limit)
6. ทดสอบบน Mobile จริงแล้ว

> ครบ 6 ข้อ = **พร้อมต้อนรับสมาชิก!**

---

### SLIDE 12: สรุป — Next Step
## ระบบพร้อมแล้ว ต่อไปคืออะไร?
- Configuration เสร็จ = ระบบ **พร้อมใช้งาน**
- ตอนต่อไป: **สร้าง Product ใน Membership** (SOMT-007)
- Product = สิ่งที่สมาชิก **จ่ายเงินซื้อ**

> *"ตั้งค่าดี สมาชิกอยู่นาน รายได้ยั่งยืน"*

---

*Slide count: 12 | Presentation time: 12-15 minutes*
