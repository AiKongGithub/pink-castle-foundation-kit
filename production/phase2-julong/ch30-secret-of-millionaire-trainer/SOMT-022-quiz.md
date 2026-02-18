# ทดสอบระบบ Affiliate — SOMT-022
> **Format:** Quiz (10 ข้อ)
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 22
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

## คำชี้แจง
- ข้อสอบ 10 ข้อ (ปรนัย 6 ข้อ / ถูก-ผิด 3 ข้อ / เติมคำ 1 ข้อ)
- เฉลยพร้อมคำอธิบายอยู่ด้านล่าง

---

### ข้อ 1 (ปรนัย)
**End-to-End Testing ของระบบ Affiliate ต้องทดสอบกี่ Scenarios หลัก?**

A) 3 Scenarios
B) 4 Scenarios
C) 6 Scenarios
D) 10 Scenarios

---

### ข้อ 2 (ปรนัย)
**"Last Click Wins" หมายความว่าอะไร?**

A) Affiliate คนแรกที่แนะนำลูกค้าได้ Commission
B) Affiliate คนสุดท้ายที่ลูกค้าคลิกลิงก์ก่อนซื้อได้ Commission
C) Affiliate ทุกคนแบ่ง Commission เท่าๆ กัน
D) Commission ไปหาเจ้าของสินค้าเสมอ

---

### ข้อ 3 (ปรนัย)
**Commission Calculation ต้องทดสอบกี่ Cases?**

A) 3 Cases
B) 4 Cases
C) 6 Cases
D) 8 Cases

---

### ข้อ 4 (ปรนัย)
**Refund Clawback ทำงานอย่างไร?**

A) เรียกเงินคืนจาก Affiliate โดยตรง
B) หักยอด Commission คืนจาก Pending ของงวดถัดไป
C) ยกเลิก Account ของ Affiliate ทันที
D) ไม่ทำอะไร Commission จ่ายไปแล้วเรียกคืนไม่ได้

---

### ข้อ 5 (ปรนัย)
**QA Checklist ก่อน Launch มีทั้งหมดกี่ข้อ?**

A) 5 ข้อ
B) 8 ข้อ
C) 10 ข้อ
D) 15 ข้อ

---

### ข้อ 6 (ปรนัย)
**ถ้า QA Checklist ผ่านต่ำกว่า 8 ข้อ ควรทำอย่างไร?**

A) Launch ได้เลย แก้ทีหลัง
B) Launch แบบ Soft Launch กับกลุ่มเล็กๆ
C) อย่าเพิ่ง Launch ต้องแก้ให้ครบก่อน
D) ยกเลิก Affiliate Program ทั้งหมด

---

### ข้อ 7 (ถูก-ผิด)
**Cookie Duration Test ทดสอบโดยคลิกลิงก์ ปิดเบราว์เซอร์ เปิดใหม่อีก 1 วัน แล้วดูว่า Cookie ยังอยู่หรือไม่**

ถูก / ผิด

---

### ข้อ 8 (ถูก-ผิด)
**หลัง Launch ระบบ Affiliate แล้ว ไม่จำเป็นต้อง Monitor เพราะทุกอย่างทดสอบผ่านแล้ว**

ถูก / ผิด

---

### ข้อ 9 (ถูก-ผิด)
**ปัญหา Cookie Not Tracking มักเกิดจาก Ad Blocker หรือ Privacy Settings ของเบราว์เซอร์**

ถูก / ผิด

---

### ข้อ 10 (เติมคำ)
**Tiered Commission ทดสอบโดยจำลองให้ Affiliate ขายถึงจุดเปลี่ยน Tier เช่น ชิ้นที่ 11 Commission ต้องขยับจาก _______% เป็น _______% อัตโนมัติ**

---

---

## เฉลยพร้อมคำอธิบาย

### ข้อ 1: ✅ C) 6 Scenarios
> 6 Scenarios หลัก: 1) Signup Test 2) Link Generation Test 3) Tracking Test 4) Test Purchase 5) Commission Calculation Test 6) Payment Testing ทั้ง 6 ครอบคลุมทุกจุดเสี่ยงของระบบ Affiliate

### ข้อ 2: ✅ B) Affiliate คนสุดท้ายที่ลูกค้าคลิกลิงก์ก่อนซื้อได้ Commission
> Last Click Wins เป็น Attribution Model ที่นิยมใช้มากที่สุด ถ้าลูกค้าคลิกลิงก์ Affiliate A ก่อน แล้วคลิกลิงก์ Affiliate B ทีหลัง Commission จะไปหา B เพราะเป็น Click สุดท้าย

### ข้อ 3: ✅ C) 6 Cases
> 6 Cases: 1) Percentage Commission 2) Fixed Amount 3) Tiered Commission 4) Recurring Commission 5) Refund Cancel 6) Upsell Commission ทุก Case ต้อง Pass ครบก่อน Launch

### ข้อ 4: ✅ B) หักยอด Commission คืนจาก Pending ของงวดถัดไป
> Refund Clawback ไม่ได้เรียกเงินคืนจาก Affiliate โดยตรง แต่หักจากยอด Commission ที่ยังเป็น Pending ในงวดถัดไป เป็นวิธีที่ยุติธรรมและไม่สร้างปัญหากับ Affiliate

### ข้อ 5: ✅ C) 10 ข้อ
> QA Checklist 10 ข้อ: Signup Flow, Link Generation, Cookie Tracking, Purchase Tracking, Commission Calculation, Dashboard Display, Payment Process, Refund Clawback, Anti-Fraud Detection, Email Notifications

### ข้อ 6: ✅ C) อย่าเพิ่ง Launch ต้องแก้ให้ครบก่อน
> ถ้าผ่านต่ำกว่า 8 ข้อ หมายความว่ามีจุดเสี่ยงมากเกินไป ต้องแก้ให้ผ่านอย่างน้อย 8 ข้อก่อน (ผ่าน 8-9 ข้อ = แก้ก่อนแล้ว Launch, 10 ข้อ = พร้อม Launch ทันที)

### ข้อ 7: ✅ ถูก
> Cookie Duration Test ทดสอบตามขั้นตอนนี้เพื่อยืนยันว่า Cookie ยังคงอยู่ตามระยะเวลาที่ตั้งไว้ (เช่น 30, 60 หรือ 90 วัน) ควรทดสอบหลายเบราว์เซอร์ด้วย

### ข้อ 8: ✅ ผิด
> หลัง Launch ต้อง Monitor อย่างใกล้ชิด สัปดาห์แรก ดู Dashboard ทุกวัน ตรวจ Commission ทุกรายการ ตอบคำถาม Affiliate ทันที ผ่าน 2 สัปดาห์ค่อยลดเป็นสัปดาห์ละครั้ง

### ข้อ 9: ✅ ถูก
> Cookie Not Tracking มักเกิดจาก Ad Blocker ที่บล็อก Tracking Script หรือ Privacy Settings ที่ตั้งสูง (เช่น Safari ITP) วิธีแก้คือแนะนำให้ปิด Ad Blocker หรือใช้ Direct Links

### ข้อ 10: ✅ 20, 30
> Tiered Commission ตัวอย่างในบทเรียน: ขาย 1-10 ชิ้นได้ 20% เมื่อขายชิ้นที่ 11 Commission ขยับจาก 20% เป็น 30% อัตโนมัติ ต้องทดสอบว่าจุดเปลี่ยน Tier ทำงานถูกต้อง

---

### สรุปผลสอบ

| ระดับ | คะแนน | การประเมิน |
|-------|--------|-----------|
| ยอดเยี่ยม | 9-10 | พร้อม Launch ระบบ Affiliate ได้ด้วยตัวเอง |
| ดี | 7-8 | เข้าใจดี ทบทวนจุดที่พลาด |
| ปานกลาง | 5-6 | ควรศึกษาเพิ่มเรื่อง Testing Scenarios |
| ต้องปรับปรุง | < 5 | ควรดูเนื้อหาซ้ำทั้งหมด |

---

*Quiz count: 10 | Focus: Affiliate System End-to-End Testing*
