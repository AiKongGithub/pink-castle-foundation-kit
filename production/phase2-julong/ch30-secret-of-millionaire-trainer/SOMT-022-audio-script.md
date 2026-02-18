# ทดสอบระบบ Affiliate — SOMT-022
> **Format:** Audio Script (Podcast-style)
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 22
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18
> **Duration:** 0:46:41

---

## SEGMENT 1: เปิดรายการ (00:00 - 03:00)

**Host A:** สวัสดีครับทุกคน มาถึงตอนสุดท้ายของ Secret Of Millionaire Trainer แล้วนะครับ ตอนที่ 22 ทดสอบระบบ Affiliate ก่อนเปิดตัวจริง ตอนนี้ยาวเกือบ 47 นาทีเลย เพราะต้องทดสอบทุกขั้นตอนอย่างละเอียด

**Host B:** ใช่ค่ะ ตอนนี้สำคัญมากเพราะเป็นขั้นตอนสุดท้ายก่อน Launch ถ้าข้ามไปโดยไม่ทดสอบ อาจเจอปัญหาหนักเมื่อ Affiliate จริงๆ เริ่มขาย ทั้ง Commission ไม่ถูก Tracking ไม่ทำงาน หรือ Payment ผิดพลาด

**Host A:** วันนี้เราจะครอบคลุม End-to-End Testing ทุก Scenario ตั้งแต่สมัคร สร้างลิงก์ ซื้อทดสอบ ตรวจ Commission ไปจนถึง QA Checklist ก่อน Launch ครับ

---

## SEGMENT 2: Test Scenario 1-3 — Signup, Link Generation, Tracking (03:00 - 15:00)

**Host B:** เริ่มจาก Scenario 1 Affiliate Signup Test ค่ะ สมมติตัวเองเป็น Affiliate ใหม่ เข้าหน้า Signup กรอกข้อมูล ยอมรับ T&C แล้วดูว่า Approval Process ทำงานถูกต้องไหม ได้ Welcome Email ไหม Dashboard เปิดได้ไหม

**Host A:** สิ่งที่ต้องเช็ค ฟอร์มกรอกได้ครบทุกช่อง Error Messages แสดงเมื่อกรอกผิด Auto-approve หรือ Manual ทำงานตามที่ตั้ง Welcome Email ส่งเนื้อหาถูก Dashboard แสดงข้อมูลเริ่มต้น 0 ทั้งหมดครับ

**Host B:** Scenario 2 Link Generation Test ค่ะ เข้า Dashboard สร้าง Tracking Link ดูว่าลิงก์ถูกต้อง มีพารามิเตอร์ Affiliate ID เมื่อคลิกลิงก์แล้ว Redirect ไปหน้าสินค้าถูก Cookie ฝังบนเบราว์เซอร์ถูกต้อง

**Host A:** ทดสอบ Sub-tracking ด้วยครับ สร้างลิงก์ 2 แบบ แบบสำหรับ Facebook แบบสำหรับ Email ดูว่า Dashboard แยกข้อมูลได้ถูกต้องไหม

**Host B:** Scenario 3 Tracking Test ค่ะ ทดสอบ Cookie Duration คลิกลิงก์วันนี้ ปิดเบราว์เซอร์ เปิดใหม่อีก 1 วัน ดูว่า Cookie ยังอยู่ไหม และทดสอบ "Last Click Wins" ถ้าคลิกลิงก์ Affiliate A แล้วคลิกลิงก์ Affiliate B ทีหลัง Commission ไปหา B ถูกต้องไหม

---

## SEGMENT 3: Test Scenario 4-5 — Purchase และ Commission Calculation (15:00 - 28:00)

**Host A:** Scenario 4 คือ Test Purchase ครับ สร้าง Test Account ใช้บัตรเครดิตทดสอบ หรือ Coupon 100% Discount แล้วซื้อสินค้าผ่าน Affiliate Link ทดสอบทั้ง One-time Purchase และ Subscription

**Host B:** สิ่งที่ต้องเช็คค่ะ Order สร้างถูกต้อง ระบุ Affiliate ที่แนะนำ Commission คำนวณถูก (ถ้า 30% ของ 5,000 = 1,500) Commission แสดงใน Dashboard ของ Affiliate สถานะเป็น "Pending" (รอจ่าย)

**Host A:** Scenario 5 Commission Calculation Test ครับ ทดสอบทุก Case ที่เป็นไปได้ Case 1 Percentage Commission 30% x 5,000 = 1,500 ถูกไหม Case 2 Fixed Amount 500 บาทต่อการขาย ถูกไหม Case 3 Tiered Commission ถ้า Affiliate ขายชิ้นที่ 11 Commission ขยับจาก 20% เป็น 30% ถูกไหม

**Host B:** Case 4 Recurring Commission ค่ะ ถ้าสมาชิกจ่ายค่าสมาชิกเดือนที่ 2 Affiliate ได้ Commission เดือนที่ 2 ด้วยไหม Case 5 ถ้าลูกค้าขอ Refund Commission ถูกยกเลิกอัตโนมัติไหม

**Host A:** Case 6 ถ้าซื้อผ่าน One-Click Upsell Commission คำนวณถูกสำหรับทั้ง Main Product และ Upsell Product ไหม ทุก Case ต้อง Pass ครบ ถ้ามี Case ไหนไม่ Pass ต้องแก้ก่อน Launch

---

## SEGMENT 4: Test Scenario 6 — Payment Testing (28:00 - 36:00)

**Host B:** Scenario 6 Payment Testing ค่ะ ทดสอบว่าระบบจ่ายเงินให้ Affiliate ถูกต้อง

**Host A:** ขั้นตอนที่ 1 ตรวจ Pending Commission ว่ายอดสะสมถูกต้อง ขั้นตอนที่ 2 จำลอง Payout Process ดูว่าระบบคำนวณ Payout Amount ถูก หักค่าธรรมเนียมถูก ขั้นตอนที่ 3 ทดสอบ Minimum Payout Threshold ถ้ายอดยังไม่ถึงเกณฑ์ ระบบต้องแสดง "ยังไม่ถึงเกณฑ์ขั้นต่ำ" ไม่ให้ถอน

**Host B:** ขั้นตอนที่ 4 ทดสอบ Refund Clawback ค่ะ ถ้าจ่าย Commission ไปแล้ว แล้วลูกค้าขอ Refund ระบบต้องหักยอด Commission คืนจาก Pending ของงวดถัดไป

**Host A:** Payment Testing ต้องทำอย่างละเอียดครับ เพราะเกี่ยวกับเงินจริง ถ้ามีข้อผิดพลาดจะสร้างความไม่พอใจให้ Affiliate ทันที

---

## SEGMENT 5: Common Issues, QA Checklist และ Launch Readiness (36:00 - 46:41)

**Host B:** มาดู Common Issues ที่มักเจอค่ะ ปัญหาแรก Cookie Not Tracking สาเหตุมักจาก Ad Blocker หรือ Privacy Settings วิธีแก้คือแนะนำให้ Affiliate บอกคนให้ปิด Ad Blocker หรือใช้ Direct Links

**Host A:** ปัญหาที่สอง Commission Not Showing เกิดจากลิงก์ไม่มี Affiliate Parameter หรือ Cookie หมดอายุ วิธีแก้คือตรวจสอบลิงก์ทุกครั้งที่สร้าง ปัญหาที่สาม Duplicate Commission เกิดจากลูกค้าซื้อผ่านหลาย Affiliate วิธีแก้คือใช้ Last Click Attribution

**Host B:** QA Checklist ก่อน Launch ค่ะ ต้อง Pass ทั้งหมด ข้อ 1 Signup Flow ทำงานครบ ข้อ 2 Link Generation ถูกต้อง ข้อ 3 Cookie Tracking ทำงาน ข้อ 4 Purchase Tracking ถูก ข้อ 5 Commission Calculation ถูกทุก Case ข้อ 6 Dashboard แสดงข้อมูลถูก ข้อ 7 Payment Process ถูกต้อง ข้อ 8 Refund Clawback ทำงาน ข้อ 9 Anti-Fraud ตรวจจับได้ ข้อ 10 Email Notifications ส่งถูก

**Host A:** Launch Readiness Assessment ครับ ถ้า QA Checklist ผ่านครบ 10 ข้อ พร้อม Launch ถ้าผ่าน 8-9 ข้อ แก้ไขก่อนแล้ว Launch ถ้าผ่านต่ำกว่า 8 ข้อ อย่าเพิ่ง Launch ต้องแก้ให้ครบก่อน

**Host B:** หลัง Launch ต้อง Monitor อย่างใกล้ชิดค่ะ สัปดาห์แรกดู Dashboard ทุกวัน ตรวจ Commission ทุกรายการ ตอบคำถาม Affiliate ทันที เมื่อผ่าน 2 สัปดาห์แล้วทุกอย่างราบรื่น ค่อยลดการ Monitor เป็นสัปดาห์ละครั้ง

**Host A:** สรุปครับ ตอนที่ 22 นี้คือด่านสุดท้ายก่อน Launch ทดสอบทุก Scenario ทำ QA Checklist ให้ครบ แล้ว Monitor หลัง Launch อย่างใกล้ชิด และนี่ก็คือตอนสุดท้ายของ Secret Of Millionaire Trainer ครับ ขอบคุณทุกคนที่ติดตามมาตลอด 22 ตอน สวัสดีครับ!

---

*Word count: ~1,200 | Audio duration estimate: 12-15 minutes*
