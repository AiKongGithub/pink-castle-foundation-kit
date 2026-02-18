# วิธีตั้งค่า Membership System — SOMT-006
> **Format:** Quiz (10 ข้อ)
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 6
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

## คำชี้แจง
- ข้อสอบ 10 ข้อ (ปรนัย 6 ข้อ / ถูก-ผิด 3 ข้อ / เติมคำ 1 ข้อ)
- เฉลยพร้อมคำอธิบายอยู่ด้านล่าง

---

### ข้อ 1 (ปรนัย)
**Branding Settings ของ Membership System ประกอบด้วยข้อใดบ้าง?**

A) โลโก้, Color Scheme, Favicon, Custom Domain
B) โลโก้, ราคา, Payment Gateway, Coupon
C) Color Scheme, Video Player, Chat Widget, Footer
D) Font, Animation, Sound Effect, Background Video

---

### ข้อ 2 (ปรนัย)
**Welcome Email ต้องทำหน้าที่กี่อย่าง และอะไรบ้าง?**

A) 2 อย่าง: ต้อนรับ + ให้ Login Info
B) 3 อย่าง: ต้อนรับ + บอก Next Steps + ให้ Login Info
C) 4 อย่าง: ต้อนรับ + ขายสินค้า + ให้ Login Info + ขอ Review
D) 1 อย่าง: ให้ Login Info เท่านั้น

---

### ข้อ 3 (ปรนัย)
**หลักการ "3-Click Rule" หมายความว่าอย่างไร?**

A) สมาชิกต้องคลิก 3 ครั้งก่อน Login
B) สมาชิกต้องหาสิ่งที่ต้องการได้ภายใน 3 คลิก
C) ระบบต้องมี 3 เมนูหลักเท่านั้น
D) ทุกหน้าต้องมี 3 ปุ่ม CTA

---

### ข้อ 4 (ปรนัย)
**Email Notifications ที่ต้องตั้งค่ามีกี่ประเภท?**

A) 2 ประเภท: Welcome + Content Alert
B) 3 ประเภท: Welcome + Payment + Cancellation
C) 4 ประเภท: Welcome + Content Alert + Payment Reminder + Failed Payment
D) 5 ประเภท: Welcome + Content + Payment + Failed + Cancellation

---

### ข้อ 5 (ปรนัย)
**Device Limit ที่แนะนำสำหรับป้องกัน Account Sharing คือกี่เครื่อง?**

A) 1 เครื่องเท่านั้น
B) 2-3 เครื่อง (PC + มือถือ + Tablet)
C) 5 เครื่อง ไม่จำกัด
D) ไม่ต้องจำกัด เพราะทำให้สมาชิกอึดอัด

---

### ข้อ 6 (ปรนัย)
**ผู้ใช้งานกี่ % เข้าระบบ Membership ผ่านมือถือ?**

A) 20-30%
B) 40-50%
C) 60-70%
D) 80-90%

---

### ข้อ 7 (ถูก-ผิด)
**Login Page ของ Membership ควรเป็นฟอร์มธรรมดาที่มีแค่ช่อง Username และ Password ก็เพียงพอแล้ว**

ถูก / ผิด

---

### ข้อ 8 (ถูก-ผิด)
**การทดสอบ Mobile Responsiveness ด้วย Responsive Mode ใน Browser เพียงพอแล้ว ไม่ต้องทดสอบบนมือถือจริง**

ถูก / ผิด

---

### ข้อ 9 (ถูก-ผิด)
**ควรสร้าง Test Account และทดลอง Login ดูเองก่อนเปิดระบบจริง**

ถูก / ผิด

---

### ข้อ 10 (เติมคำ)
**สมาชิกที่หน้า Mobile ใช้ยาก จะมีแนวโน้มเลิกเข้าเรียนภายใน _______**

---

---

## เฉลยพร้อมคำอธิบาย

### ข้อ 1: ✅ A) โลโก้, Color Scheme, Favicon, Custom Domain
> Branding Settings ประกอบด้วยองค์ประกอบ Visual Identity ทั้งหมด ได้แก่ โลโก้ (PNG/SVG), Color Scheme (Primary/Secondary/Accent), Favicon (ไอคอน Browser Tab), Custom Domain และ Font Selection เพื่อสร้าง Brand Consistency ทั้งระบบ

### ข้อ 2: ✅ B) 3 อย่าง: ต้อนรับ + บอก Next Steps + ให้ Login Info
> Welcome Email ต้องทำ 3 หน้าที่สำคัญ: 1) ต้อนรับและสร้างความตื่นเต้น 2) บอก Next Steps ชัดเจนว่าต้องทำอะไร 3) ให้ข้อมูล Login ที่ชัดเจน เป้าหมายคือให้สมาชิกเข้าระบบและเริ่มเรียนภายใน 24 ชั่วโมง

### ข้อ 3: ✅ B) สมาชิกต้องหาสิ่งที่ต้องการได้ภายใน 3 คลิก
> 3-Click Rule คือหลักการออกแบบ UX ที่ว่าผู้ใช้ต้องเข้าถึงสิ่งที่ต้องการได้ภายใน 3 คลิก ไม่ว่าจะเป็นบทเรียน ความก้าวหน้า หรือเนื้อหาใหม่ ช่วยลดความสับสนและเพิ่มความพึงพอใจ

### ข้อ 4: ✅ C) 4 ประเภท: Welcome + Content Alert + Payment Reminder + Failed Payment
> ต้องตั้งค่าอีเมล 4 ประเภท: Welcome Email (ต้อนรับ), New Content Alert (แจ้งเนื้อหาใหม่), Payment Reminder (แจ้งก่อนเรียกเก็บเงิน), Failed Payment (แจ้งเมื่อชำระไม่สำเร็จ)

### ข้อ 5: ✅ B) 2-3 เครื่อง (PC + มือถือ + Tablet)
> 2-3 เครื่องเป็นจุดสมดุลระหว่างความสะดวก (สมาชิกใช้หลายอุปกรณ์จริง) กับความปลอดภัย (ป้องกัน Account Sharing) 1 เครื่องอึดอัดเกินไป ไม่จำกัดเลยเสี่ยงต่อการแชร์

### ข้อ 6: ✅ C) 60-70%
> ในยุคปัจจุบัน ผู้ใช้ 60-70% เข้าถึงเนื้อหาออนไลน์ผ่านมือถือ ทำให้ Mobile Responsiveness เป็นสิ่งจำเป็น ไม่ใช่ทางเลือก

### ข้อ 7: ✅ ผิด
> Login Page ไม่ควรเป็นแค่ฟอร์มธรรมดา ควรมีโลโก้แบรนด์, Welcome Message, ภาพสร้างแรงบันดาลใจ เพื่อสร้าง First Impression ที่ดีทุกครั้งที่สมาชิกเข้าเรียน

### ข้อ 8: ✅ ผิด
> ต้องทดสอบบนมือถือจริง (ทั้ง iOS และ Android) เพราะ Responsive Mode ใน Browser ไม่ได้จำลองประสบการณ์จริงได้ 100% เช่น Touch Interaction, Font Size, Loading Speed บนมือถือจริง

### ข้อ 9: ✅ ถูก
> ควรสร้าง Test Account และทดลองเป็นสมาชิกเอง ลอง Login, ดู Dashboard, ลองเรียนบทเรียน เพื่อประเมินประสบการณ์จริงก่อนเปิดให้สมาชิกจริงใช้งาน

### ข้อ 10: ✅ 1 สัปดาห์
> ถ้าหน้า Mobile ใช้ยาก สมาชิกจะเลิกเข้าเรียนภายใน 1 สัปดาห์ เพราะความไม่สะดวกทำให้ขาดแรงจูงใจในการเข้ามาซ้ำ

---

### สรุปผลสอบ

| ระดับ | คะแนน | การประเมิน |
|-------|--------|-----------|
| ยอดเยี่ยม | 9-10 | เข้าใจ Configuration ครบถ้วน พร้อมตั้งค่าเอง |
| ดี | 7-8 | เข้าใจดี ทบทวนจุดที่พลาด |
| ปานกลาง | 5-6 | ควรศึกษาเพิ่มเติมเรื่อง Settings |
| ต้องปรับปรุง | < 5 | ควรดูเนื้อหาซ้ำ |

---

*Quiz count: 10 | Focus: Membership System Configuration*
