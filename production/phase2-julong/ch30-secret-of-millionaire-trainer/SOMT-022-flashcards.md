# ทดสอบระบบ Affiliate — SOMT-022
> **Format:** Flashcards (15 Cards)
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 22
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18
> **Duration:** 0:46:41

---

=== CARD 1 ===
Q: Affiliate Signup Test ต้องเช็คอะไรบ้าง?
A: **5 สิ่งที่ต้องเช็ค**: 1) **ฟอร์มกรอกได้ครบทุกช่อง** ไม่มี Bug 2) **Error Messages** แสดงเมื่อกรอกผิด 3) **Approval Process** ทำงานตามที่ตั้ง (Auto/Manual) 4) **Welcome Email** ส่งอัตโนมัติ เนื้อหาถูกต้อง 5) **Dashboard** แสดงข้อมูลเริ่มต้นเป็น 0 ทั้งหมด

---

=== CARD 2 ===
Q: Link Generation Test ทดสอบอะไร?
A: ทดสอบว่า **Tracking Link** ที่สร้างจาก Dashboard มี **Affiliate ID** ถูกต้อง เมื่อคลิกแล้ว **Redirect** ไปหน้าสินค้าถูก **Cookie ฝังบนเบราว์เซอร์** ถูกต้อง รวมถึงทดสอบ **Sub-tracking** สร้างลิงก์แยกตามช่องทาง (Facebook, Email) ดูว่า Dashboard แยกข้อมูลได้ถูกต้อง

---

=== CARD 3 ===
Q: Cookie Duration Test ทดสอบอย่างไร?
A: **ขั้นตอน**: 1) คลิก Affiliate Link วันนี้ 2) ปิดเบราว์เซอร์ 3) เปิดใหม่อีก 1 วัน 4) ตรวจว่า **Cookie ยังอยู่ไหม** ถ้าตั้ง Cookie 60 วัน ต้องยังอยู่ ทดสอบหลายเบราว์เซอร์ (Chrome, Safari, Firefox) และบนมือถือด้วย เพราะแต่ละเบราว์เซอร์จัดการ Cookie ต่างกัน

---

=== CARD 4 ===
Q: "Last Click Wins" คืออะไร? ทดสอบอย่างไร?
A: **Last Click Wins** = Attribution Model ที่ให้ Commission กับ Affiliate **คนสุดท้ายที่คลิก** ก่อนซื้อ **ทดสอบ**: คลิกลิงก์ Affiliate A ก่อน → คลิกลิงก์ Affiliate B ทีหลัง → ซื้อสินค้า → **Commission ต้องไปหา B** ไม่ใช่ A เพราะ B เป็น Last Click

---

=== CARD 5 ===
Q: Test Purchase ทำอย่างไร? ต้องเช็คอะไร?
A: **วิธีทำ**: สร้าง Test Account ใช้ **บัตรเครดิตทดสอบ** หรือ **Coupon 100% Discount** แล้วซื้อผ่าน Affiliate Link **สิ่งที่เช็ค**: 1) Order สร้างถูกต้อง 2) ระบุ Affiliate ที่แนะนำ 3) Commission คำนวณถูก 4) Commission แสดงใน Dashboard 5) สถานะเป็น **"Pending"** ทดสอบทั้ง One-time และ Subscription

---

=== CARD 6 ===
Q: Commission Calculation ต้องทดสอบกี่ Cases? อะไรบ้าง?
A: **6 Cases**: 1) **Percentage** — 30% x 5,000 = 1,500 ถูกไหม 2) **Fixed Amount** — 500 บาท/ขาย ถูกไหม 3) **Tiered** — ชิ้นที่ 11 เปลี่ยนจาก 20% เป็น 30% ถูกไหม 4) **Recurring** — เดือนที่ 2+ ได้ Commission ด้วยไหม 5) **Refund** — Commission ยกเลิกอัตโนมัติไหม 6) **Upsell** — Main + Upsell คำนวณถูกไหม **ทุก Case ต้อง Pass ครบ**

---

=== CARD 7 ===
Q: Tiered Commission คืออะไร? ทดสอบอย่างไร?
A: **Tiered Commission** = โครงสร้าง Commission ที่เปลี่ยนตามยอดขาย เช่น ขาย 1-10 ชิ้น ได้ 20% | ขาย 11+ ชิ้น ได้ 30% **ทดสอบ**: จำลองให้ Affiliate ขายถึง **จุดเปลี่ยน Tier** (ชิ้นที่ 11) ดูว่า Commission **ขยับขึ้นอัตโนมัติ** จาก 20% เป็น 30% ถูกต้องไหม

---

=== CARD 8 ===
Q: Recurring Commission ทดสอบอย่างไร?
A: ทดสอบด้วยการสร้าง **Subscription Purchase** ผ่าน Affiliate Link แล้วจำลองการ **จ่ายค่าสมาชิกเดือนที่ 2** ดูว่า Affiliate ได้ **Commission เดือนที่ 2 ด้วยไหม** ถ้าตั้งไว้ว่า Recurring Commission ต้องจ่าย ระบบต้องคำนวณและแสดงใน Dashboard อัตโนมัติ

---

=== CARD 9 ===
Q: Payment Testing ต้องเช็ค 4 ขั้นตอนอะไร?
A: 1) **ตรวจ Pending Commission** — ยอดสะสมถูกต้องไหม 2) **จำลอง Payout Process** — คำนวณ Payout Amount ถูก หักค่าธรรมเนียมถูกไหม 3) **ทดสอบ Minimum Payout Threshold** — ยอดยังไม่ถึงเกณฑ์ ระบบต้องแสดง "ยังไม่ถึงเกณฑ์ขั้นต่ำ" 4) **ทดสอบ Refund Clawback** — จ่าย Commission ไปแล้ว ลูกค้า Refund ระบบหัก Commission คืน

---

=== CARD 10 ===
Q: Refund Clawback คืออะไร? ทำงานอย่างไร?
A: **Refund Clawback** = การเรียก Commission คืนเมื่อลูกค้า Refund **กลไก**: ถ้าจ่าย Commission ไปแล้ว 1,500 บาท แล้วลูกค้าขอ Refund ระบบต้อง **หักยอด 1,500 บาทคืน** จาก Pending Commission ของ **งวดถัดไป** ไม่ใช่เรียกเงินคืนจาก Affiliate โดยตรง ทดสอบว่ายอด Pending ลดลงถูกต้อง

---

=== CARD 11 ===
Q: ปัญหา Cookie Not Tracking สาเหตุและวิธีแก้คืออะไร?
A: **สาเหตุ**: 1) **Ad Blocker** บล็อก Tracking Script 2) **Privacy Settings** ของเบราว์เซอร์ที่ตั้งไว้สูง (เช่น Safari ITP) 3) **Incognito Mode** ที่ลบ Cookie ทุกครั้งที่ปิด **วิธีแก้**: แนะนำให้ Affiliate บอกคนให้ **ปิด Ad Blocker** หรือใช้ **Direct Links** ที่ไม่ต้องพึ่ง Cookie (เช่น Coupon Code Tracking)

---

=== CARD 12 ===
Q: QA Checklist 10 ข้อก่อน Launch มีอะไรบ้าง?
A: 1) **Signup Flow** ทำงานครบ 2) **Link Generation** ถูกต้อง 3) **Cookie Tracking** ทำงาน 4) **Purchase Tracking** ถูก 5) **Commission Calculation** ถูกทุก Case 6) **Dashboard** แสดงข้อมูลถูก 7) **Payment Process** ถูกต้อง 8) **Refund Clawback** ทำงาน 9) **Anti-Fraud** ตรวจจับได้ 10) **Email Notifications** ส่งถูก **ต้อง Pass ครบทั้ง 10 ข้อ**

---

=== CARD 13 ===
Q: Launch Readiness Assessment มีเกณฑ์อย่างไร?
A: **3 ระดับ**: 1) **QA ผ่านครบ 10 ข้อ** → พร้อม Launch ทันที 2) **ผ่าน 8-9 ข้อ** → แก้ไขข้อที่ไม่ผ่านก่อน แล้ว Launch 3) **ผ่านต่ำกว่า 8 ข้อ** → **อย่าเพิ่ง Launch** ต้องแก้ให้ครบก่อน เพราะมีจุดเสี่ยงมากเกินไป

---

=== CARD 14 ===
Q: Post-launch Monitoring ควรทำอย่างไร?
A: **ช่วง Intensive (สัปดาห์ที่ 1-2)**: ดู Dashboard **ทุกวัน** ตรวจ Commission ทุกรายการ ตอบคำถาม Affiliate ทันที **ช่วงปรับลด (สัปดาห์ที่ 3-4)**: Monitor ทุก 2-3 วัน **ช่วงปกติ (หลัง 1 เดือน)**: Monitor สัปดาห์ละครั้ง พร้อมตั้ง **Alert อัตโนมัติ** สำหรับ Anomalies เช่น Commission สูงผิดปกติ

---

=== CARD 15 ===
Q: ทำไมการทดสอบระบบ Affiliate ก่อน Launch จึงสำคัญที่สุด?
A: เพราะระบบ Affiliate เกี่ยวข้องกับ **เงินจริง** ถ้า Commission คำนวณผิดแม้ 1 บาท Affiliate จะ **ไม่เชื่อมั่น** ในระบบ ถ้า Tracking ไม่ทำงาน Affiliate จะ **เสียรายได้** ถ้า Payment ผิดพลาด เกิด **ข้อพิพาททางกฎหมาย** การทดสอบ End-to-End ทุก Scenario คือ **การลงทุนที่คุ้มค่าที่สุด** ก่อนเปิดตัว ป้องกันปัญหาที่แก้ไขยากมากเมื่อมี Affiliate จริงในระบบแล้ว

---

*Flashcard count: 15 | Focus: Affiliate System End-to-End Testing*
