# วิธี Deploy Membership System — SOMT-005
> **Format:** Quiz (10 Questions)
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 5
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

## คำแนะนำ
- ทำข้อสอบด้วยตัวเองก่อนดูเฉลย
- ข้อ 1-6: ปรนัย (Multiple Choice)
- ข้อ 7-9: ถูก/ผิด (True/False)
- ข้อ 10: เติมคำ (Fill-in-the-blank)

---

### ข้อ 1 (Multiple Choice)
ขั้นตอนแรกในการ Deploy Membership บน Kartra คืออะไร?

- A) ตั้งค่า SSL
- B) เชื่อมต่อ Stripe
- C) สร้าง Membership Portal (ตั้งชื่อ + เลือก Template)
- D) ตั้งค่า Domain

---

### ข้อ 2 (Multiple Choice)
ข้อใดเป็นข้อดีของการใช้ Custom Domain เมื่อเทียบกับ Kartra Subdomain?

- A) ใช้งานได้ทันทีโดยไม่ต้องตั้งค่า DNS
- B) ดู Professional และ Brand เป็นของตัวเอง
- C) ราคาถูกกว่า Kartra Subdomain
- D) ไม่ต้องมี SSL Certificate

---

### ข้อ 3 (Multiple Choice)
SSL ที่ Kartra ให้ใช้ฟรี ใช้เวลา Provision นานสูงสุดเท่าไหร่?

- A) 1 ชั่วโมง
- B) 6 ชั่วโมง
- C) 24 ชั่วโมง
- D) 7 วัน

---

### ข้อ 4 (Multiple Choice)
ข้อใด **ไม่ใช่** รายการใน Testing Checklist ก่อน Go Live?

- A) ทดสอบ Signup Flow
- B) ทดสอบ SEO Ranking
- C) ทดสอบ Access Control (Silver vs Gold)
- D) ทดสอบ Welcome Email

---

### ข้อ 5 (Multiple Choice)
ในการตั้งค่า Payment ต้องสร้าง Products สำหรับอะไร?

- A) เพื่อแสดงในหน้า Landing Page
- B) เพื่อเชื่อมต่อ Product กับ Membership Level และตั้ง Recurring Billing
- C) เพื่อส่งสินค้าทางไปรษณีย์
- D) เพื่อสร้าง Affiliate Program

---

### ข้อ 6 (Multiple Choice)
ลำดับที่ถูกต้องของซีรีส์ Secret Of Millionaire Trainer คือข้อใด?

- A) Revenue → Identity → Deploy → Empire → Membership
- B) Identity → Revenue → Empire → Membership → Deploy
- C) Empire → Membership → Revenue → Identity → Deploy
- D) Deploy → Membership → Empire → Revenue → Identity

---

### ข้อ 7 (True/False)
**คำกล่าว:** "ควร Go Live ทันทีหลังตั้งค่า Payment โดยไม่ต้องทดสอบ เพราะ Kartra เป็น Platform ที่เสถียร"

- True
- False

---

### ข้อ 8 (True/False)
**คำกล่าว:** "SSL จำเป็นสำหรับ Membership ที่รับ Payment เพราะ Stripe และ PayPal บังคับใช้ HTTPS"

- True
- False

---

### ข้อ 9 (True/False)
**คำกล่าว:** "ควร Soft Launch กับ Beta Members 5-10 คนก่อน แล้วค่อย Public Launch เพื่อเก็บ Feedback และแก้ไขปัญหา"

- True
- False

---

### ข้อ 10 (Fill-in-the-blank)
การ Deploy Membership บน Kartra มีทั้งหมด _______ ขั้นตอนหลัก

---

## เฉลยและคำอธิบาย

### ข้อ 1: **C** — สร้าง Membership Portal (ตั้งชื่อ + เลือก Template)
> ขั้นแรกคือสร้าง Portal ก่อน ตั้งชื่อ เลือก Template ใส่ Description แล้วค่อยตั้งค่า Levels, Domain, SSL, Payment ตามลำดับ

### ข้อ 2: **B** — ดู Professional และ Brand เป็นของตัวเอง
> Custom Domain (members.yourbrand.com) สร้างความน่าเชื่อถือมากกว่า Kartra Subdomain แม้จะต้องตั้ง DNS เพิ่มเติม

### ข้อ 3: **C** — 24 ชั่วโมง
> Kartra ให้ SSL ฟรี กด Enable SSL แล้วรอ Provision ไม่เกิน 24 ชั่วโมง ระบบจัดการ Certificate ให้อัตโนมัติ

### ข้อ 4: **B** — ทดสอบ SEO Ranking
> Testing Checklist ก่อน Go Live ครอบคลุม: Signup Flow, Payment (Test Card), Access Control, Content Dripping, Welcome Email, Cancellation Flow ไม่มี SEO Ranking

### ข้อ 5: **B** — เพื่อเชื่อมต่อ Product กับ Membership Level และตั้ง Recurring Billing
> ต้องสร้าง Product (Silver 990/เดือน, Gold 2,990/เดือน) แล้วเชื่อมกับ Membership Level เพื่อให้ระบบรู้ว่าใครจ่ายอะไรได้เข้าถึง Level ไหน

### ข้อ 6: **B** — Identity → Revenue → Empire → Membership → Deploy
> ลำดับ: ตอน 1 Identity → ตอน 2 Revenue → ตอน 3 Empire → ตอน 4 Membership → ตอน 5 Deploy

### ข้อ 7: **False**
> ต้องทดสอบทุกอย่างก่อน Go Live เสมอ! Testing Checklist 6 ข้อต้องผ่านทั้งหมด ถ้าลูกค้าคนแรกเจอปัญหาจะเสียความน่าเชื่อถือที่กู้คืนได้ยาก

### ข้อ 8: **True**
> SSL (HTTPS) จำเป็นสำหรับ Payment Processing ทั้ง Stripe และ PayPal บังคับใช้ HTTPS นอกจากนี้ยังสร้างความน่าเชื่อถือให้ลูกค้า

### ข้อ 9: **True**
> Soft Launch ช่วยทดสอบกับผู้ใช้จริง เก็บ Feedback แก้ไขปัญหา และสร้าง Testimonials แรกก่อน Public Launch

### ข้อ 10: **6** ขั้นตอน
> 6 ขั้นตอน: (1) สร้าง Portal (2) ตั้งค่า Levels (3) Domain (4) SSL (5) Payment (6) ทดสอบ + Go Live

---

## สรุปคะแนน

| คะแนน | ระดับ | คำแนะนำ |
|-------|-------|---------|
| 9-10 | ยอดเยี่ยม | พร้อม Deploy Membership ของตัวเอง! |
| 7-8 | ดี | ทบทวน Testing Checklist |
| 5-6 | ปานกลาง | กลับไปอ่าน Executive Summary |
| 0-4 | ต้องปรับปรุง | ฟัง Audio Script ซ้ำทั้งหมด |

---

*สิ้นสุด Quiz — SOMT-005 | 10 ข้อ (6 ปรนัย + 3 ถูก/ผิด + 1 เติมคำ)*
