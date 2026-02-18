# ทดสอบระบบ Affiliate — SOMT-022
> **Format:** Insights Table
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 22
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

## ตาราง 12 Insights สำคัญ

| # | Insight | Detail | Application | Impact Level |
|---|---------|--------|-------------|--------------|
| 1 | End-to-End Testing คือด่านสุดท้ายที่ห้ามข้าม | ถ้าข้ามไปโดยไม่ทดสอบ อาจเจอปัญหาร้ายแรงเมื่อ Affiliate จริงเริ่มขาย Commission ผิด Tracking พัง Payment ล้มเหลว ทำลายความเชื่อมั่นทันที | วางแผนทดสอบ 6 Scenarios ครบก่อน Launch อย่าปล่อยให้ Affiliate เป็นคนเจอ Bug แทนเรา | สูงมาก |
| 2 | Signup Test ต้องจำลองเป็น Affiliate ใหม่จริงๆ | สมมติตัวเองเป็นคนที่ไม่เคยใช้ระบบ กรอกฟอร์ม ตรวจ Error Messages Approval Process Welcome Email และ Dashboard เริ่มต้น ทุกขั้นตอนต้องทำงานสมบูรณ์ | สร้าง Test Account ใหม่ ทดลองสมัครทั้ง Auto-approve และ Manual Review ตรวจ Email ทุกฉบับ | สูง |
| 3 | Sub-tracking แยกช่องทางป้องกันข้อมูลปะปน | สร้าง Tracking Link แยกสำหรับ Facebook และ Email ดูว่า Dashboard แยกข้อมูลได้ถูกต้อง ถ้าแยกไม่ได้ Affiliate ไม่รู้ว่าช่องทางไหนทำงาน | ทดสอบสร้างลิงก์อย่างน้อย 2 ช่องทาง ตรวจ Dashboard ว่าแสดงข้อมูลแยกตาม Campaign ถูกต้อง | สูง |
| 4 | Cookie Duration + Last Click Wins ต้องทดสอบคู่กัน | Cookie Duration ทดสอบด้วยการปิด-เปิดเบราว์เซอร์ Last Click Wins ทดสอบด้วยการคลิกลิงก์ 2 Affiliate ติดกัน สองอย่างนี้เป็นหัวใจของ Attribution | ทดสอบ Cookie หลายเบราว์เซอร์ (Chrome, Safari, Firefox) และทดสอบ Last Click จาก 2 Affiliate ตรวจว่า Commission ไปหาคนสุดท้าย | สูงมาก |
| 5 | Commission 6 Cases ต้อง Pass ครบไม่เว้นแม้แต่ Case เดียว | Percentage Fixed Tiered Recurring Refund Upsell ทุก Case เกี่ยวกับเงินจริง ถ้าผิดแม้ 1 Case Affiliate จะสูญเสียความเชื่อมั่น | สร้างตาราง Test Matrix 6 Cases ทดสอบทีละ Case บันทึกผล Pass/Fail ถ้ามี Fail ต้องแก้ก่อน Launch | สูงมาก |
| 6 | Tiered Commission ต้องทดสอบที่จุดเปลี่ยน Tier | จุดเปลี่ยน Tier (เช่น ชิ้นที่ 11) เป็น Edge Case ที่มักมี Bug ถ้าไม่ทดสอบอาจพบว่า Commission ไม่ขยับเมื่อถึง Tier ใหม่ หรือขยับผิด Tier | จำลองการขายให้ถึงจุดเปลี่ยน Tier พอดี (ชิ้นที่ 10 และ 11) ตรวจว่า Commission เปลี่ยนถูกต้อง | สูง |
| 7 | Refund Clawback เป็นกลไกป้องกันการสูญเสีย | เมื่อลูกค้า Refund ระบบต้องหัก Commission คืนจาก Pending ของงวดถัดไป ไม่ใช่เรียกเงินคืนจาก Affiliate โดยตรง กลไกนี้ยุติธรรมทั้งสองฝ่าย | ทดสอบโดยจำลอง Refund หลังจ่าย Commission แล้ว ตรวจว่ายอด Pending ของงวดถัดไปลดลงถูกต้อง | สูงมาก |
| 8 | Minimum Payout Threshold ป้องกัน Micro-withdrawals | ถ้าไม่มีเกณฑ์ขั้นต่ำ Affiliate จะถอนเงินทีละน้อยๆ สร้างค่าธรรมเนียมโอนสูง Threshold ป้องกันปัญหานี้ | ทดสอบด้วยยอดที่ต่ำกว่าเกณฑ์ ระบบต้องแสดง "ยังไม่ถึงเกณฑ์ขั้นต่ำ" และไม่ให้ถอน | ปานกลาง-สูง |
| 9 | Common Issues 3 ข้อที่ต้องรู้และเตรียมวิธีแก้ | Cookie Not Tracking (Ad Blocker) Commission Not Showing (ลิงก์ผิด) Duplicate Commission (หลาย Affiliate) ถ้ารู้ก่อน เตรียมแก้ได้ทันที | สร้าง FAQ หรือ Knowledge Base สำหรับ Affiliate ที่อธิบายวิธีแก้ปัญหาทั่วไป ลด Support Load | สูง |
| 10 | QA Checklist 10 ข้อเป็น Launch Gate ที่เข้มงวด | 10 ข้อครอบคลุมทุกมิติ: Signup Link Cookie Purchase Commission Dashboard Payment Refund Anti-Fraud Email ต้อง Pass ครบก่อน Launch | พิมพ์ Checklist ออกมา ทดสอบทีละข้อ ให้คนอื่นทดสอบด้วย (Fresh Eyes) เพื่อจับ Bug ที่ตัวเองมองไม่เห็น | สูงมาก |
| 11 | Launch Readiness มี 3 ระดับชัดเจน | 10/10 = Launch ได้ 8-9/10 = แก้แล้ว Launch ต่ำกว่า 8 = ห้าม Launch เกณฑ์ชัดเจนช่วยตัดสินใจไม่ลังเล ไม่มีพื้นที่สำหรับ "น่าจะ OK" | กำหนดเกณฑ์ Pass/Fail ชัดเจนก่อนเริ่มทดสอบ ไม่ปรับลดเกณฑ์เมื่อผลออกมาไม่ดี | สูง |
| 12 | Post-launch Monitoring ต้องทำอย่างเป็นระบบ | สัปดาห์ 1-2 Monitor ทุกวัน สัปดาห์ 3-4 ทุก 2-3 วัน หลัง 1 เดือน สัปดาห์ละครั้ง ค่อยๆ ลด Intensity เมื่อทุกอย่างราบรื่น | ตั้ง Calendar Alert สำหรับ Monitoring ทุกวันในสัปดาห์แรก ตั้ง Auto-alert สำหรับ Anomalies เช่น Commission สูงผิดปกติ | สูง |

---

### สรุป Impact Level

| Level | จำนวน Insights |
|-------|---------------|
| สูงมาก | 5 |
| สูง | 6 |
| ปานกลาง-สูง | 1 |
| ปานกลาง | 0 |

---

*Insights count: 12 | Focus: Affiliate System End-to-End Testing & Launch Readiness*
