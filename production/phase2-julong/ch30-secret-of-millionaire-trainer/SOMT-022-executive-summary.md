# ทดสอบระบบ Affiliate — SOMT-022
> **Format:** Executive Summary
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 22
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18
> **Duration:** 0:46:41

---

## Executive Summary

ตอนที่ 22 เป็นตอนสุดท้ายของ Secret Of Millionaire Trainer ว่าด้วยการทดสอบระบบ Affiliate แบบ End-to-End ก่อนเปิดตัวจริง ครอบคลุม 6 Test Scenarios หลัก ตั้งแต่ Signup, Link Generation, Cookie Tracking, Test Purchase, Commission Calculation ไปจนถึง Payment Testing พร้อม QA Checklist 10 ข้อที่ต้อง Pass ครบก่อน Launch และแนวทาง Monitor หลังเปิดตัว

---

## Key Findings

### 1. End-to-End Testing คือด่านสุดท้ายที่ข้ามไม่ได้
การทดสอบทุก Scenario ตั้งแต่ต้นจนจบเป็นสิ่งจำเป็นก่อน Launch ถ้าข้ามไปโดยไม่ทดสอบ อาจเจอปัญหาร้ายแรงเมื่อ Affiliate จริงเริ่มขาย ทั้ง Commission คำนวณผิด Tracking ไม่ทำงาน หรือ Payment ผิดพลาด ซึ่งทำลายความเชื่อมั่นของ Affiliate ทันที

### 2. 6 Test Scenarios ครอบคลุมทุกจุดเสี่ยง
| Scenario | สิ่งที่ทดสอบ | ความสำคัญ |
|----------|-------------|-----------|
| 1. Signup Test | ฟอร์มสมัคร, Approval, Welcome Email, Dashboard | สูง |
| 2. Link Generation | Tracking Link, Affiliate ID, Sub-tracking | สูง |
| 3. Tracking Test | Cookie Duration, Last Click Wins, Cross-browser | สูงมาก |
| 4. Test Purchase | Order Creation, Affiliate Attribution, One-time + Subscription | สูงมาก |
| 5. Commission Calculation | Percentage, Fixed, Tiered, Recurring, Refund, Upsell | สูงมาก |
| 6. Payment Testing | Pending Balance, Payout Process, Minimum Threshold, Refund Clawback | สูงมาก |

### 3. Commission Calculation ต้องทดสอบ 6 Cases
Case 1: Percentage Commission (30% x 5,000 = 1,500) — Case 2: Fixed Amount (500 บาท/ขาย) — Case 3: Tiered Commission (ชิ้นที่ 11 ขยับจาก 20% เป็น 30%) — Case 4: Recurring Commission (เดือนที่ 2+) — Case 5: Refund Clawback (ยกเลิก Commission อัตโนมัติ) — Case 6: Upsell Commission (Main + Upsell Product) ทุก Case ต้อง Pass ก่อน Launch

### 4. Common Issues 3 ข้อที่พบบ่อยที่สุด
| ปัญหา | สาเหตุ | วิธีแก้ |
|-------|--------|--------|
| Cookie Not Tracking | Ad Blocker, Privacy Settings | แนะนำปิด Ad Blocker หรือใช้ Direct Links |
| Commission Not Showing | ลิงก์ไม่มี Affiliate Parameter, Cookie หมดอายุ | ตรวจสอบลิงก์ทุกครั้งที่สร้าง |
| Duplicate Commission | ซื้อผ่านหลาย Affiliate | ใช้ Last Click Attribution |

### 5. QA Checklist 10 ข้อ กำหนด Launch Readiness
ผ่านครบ 10 ข้อ = พร้อม Launch ทันที | ผ่าน 8-9 ข้อ = แก้ไขก่อนแล้ว Launch | ต่ำกว่า 8 ข้อ = อย่าเพิ่ง Launch ต้องแก้ให้ครบ หลัง Launch ต้อง Monitor อย่างใกล้ชิดสัปดาห์แรก ดู Dashboard ทุกวัน ตรวจ Commission ทุกรายการ ตอบคำถาม Affiliate ทันที

---

## Data Highlights

| Metric | Value |
|--------|-------|
| Test Scenarios ทั้งหมด | 6 Scenarios |
| Commission Cases ที่ต้องทดสอบ | 6 Cases |
| QA Checklist Items | 10 ข้อ |
| Common Issues | 3 ปัญหาหลัก |
| Minimum Pass Rate สำหรับ Launch | 8/10 ข้อ (80%) |
| Post-launch Intensive Monitor | 2 สัปดาห์แรก |
| Cookie Duration ที่ต้องทดสอบ | ตาม Setting (30-90 วัน) |
| Attribution Model | Last Click Wins |

---

## Recommendations

### 1. สร้าง Test Environment แยกจาก Production
ใช้ Test Account และบัตรเครดิตทดสอบ หรือ Coupon 100% Discount เพื่อจำลองการซื้อจริงโดยไม่กระทบข้อมูล Production ทดสอบทั้ง One-time Purchase และ Subscription

### 2. ทดสอบ Cross-browser และ Cross-device
อย่าทดสอบแค่เบราว์เซอร์เดียว ต้องทดสอบ Cookie Tracking บน Chrome, Safari, Firefox และบนมือถือด้วย เพราะแต่ละเบราว์เซอร์มี Privacy Settings ต่างกัน

### 3. จำลอง Edge Cases ทุกตัว
ทดสอบ Refund Clawback, Tiered Commission ที่จุดเปลี่ยน Tier, Recurring Commission เดือนที่ 2+, Duplicate Click จากหลาย Affiliate เพื่อให้มั่นใจว่าทุก Case ทำงานถูกต้อง

### 4. สร้าง Automated Test Script ถ้าเป็นไปได้
เมื่อทดสอบ Manual ผ่านแล้ว ควรสร้าง Automated Test Script สำหรับ Commission Calculation เพื่อให้สามารถ Re-test ได้เร็วเมื่อมีการอัปเดตระบบ

### 5. วางแผน Post-launch Monitoring อย่างเป็นระบบ
สัปดาห์ที่ 1-2: Monitor ทุกวัน ตรวจ Commission ทุกรายการ | สัปดาห์ที่ 3-4: Monitor ทุก 2-3 วัน | หลัง 1 เดือน: Monitor สัปดาห์ละครั้ง พร้อมตั้ง Alert สำหรับ Anomalies

---

*Word count: ~650 | Reading time: 3-4 minutes*
