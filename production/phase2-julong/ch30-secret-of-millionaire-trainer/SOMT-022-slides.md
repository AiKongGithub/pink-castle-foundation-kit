# ทดสอบระบบ Affiliate — SOMT-022
> **Format:** Slide Deck (15 slides)
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 22
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

### SLIDE 1: หน้าปก
# ทดสอบระบบ Affiliate
## ด่านสุดท้ายก่อน Launch
**SWP3 บทที่ 30 ตอนที่ 22 (46:41 นาที)**
PinkCastle Academy

---

### SLIDE 2: ทำไมต้องทดสอบก่อน Launch?
## ข้ามขั้นตอนนี้ = เสี่ยงหนัก
| ถ้าไม่ทดสอบ | ผลกระทบ |
|-------------|---------|
| Commission คำนวณผิด | Affiliate ไม่เชื่อมั่น ออกจาก Program |
| Tracking ไม่ทำงาน | Affiliate เสียรายได้ ฟ้องร้อง |
| Payment ผิดพลาด | ข้อพิพาททางกฎหมาย |
| Cookie ไม่ฝัง | ยอดขาย = 0 |

> *"ระบบ Affiliate เกี่ยวกับเงินจริง — ผิดแม้ 1 บาท = เสียความเชื่อมั่น"*

---

### SLIDE 3: 6 Test Scenarios ที่ต้องผ่านทั้งหมด
## End-to-End Testing Roadmap
```
Scenario 1: Signup Test
    ↓
Scenario 2: Link Generation Test
    ↓
Scenario 3: Tracking Test (Cookie)
    ↓
Scenario 4: Test Purchase
    ↓
Scenario 5: Commission Calculation
    ↓
Scenario 6: Payment Testing
```

---

### SLIDE 4: Scenario 1 — Affiliate Signup Test
## ทดสอบการสมัคร Affiliate
| สิ่งที่เช็ค | ผลที่ต้องได้ |
|------------|-------------|
| ฟอร์มกรอกข้อมูล | ทุกช่องกรอกได้ครบ |
| Error Messages | แสดงเมื่อกรอกผิด |
| Approval Process | Auto/Manual ทำงานตามที่ตั้ง |
| Welcome Email | ส่งอัตโนมัติ เนื้อหาถูก |
| Dashboard เริ่มต้น | แสดงข้อมูล 0 ทั้งหมด |

> *สมมติตัวเองเป็น Affiliate ใหม่ ลองสมัครจริง*

---

### SLIDE 5: Scenario 2 — Link Generation Test
## ทดสอบการสร้าง Tracking Link
**ขั้นตอน:**
1. เข้า Dashboard → สร้าง Tracking Link
2. ตรวจว่าลิงก์มี **Affiliate ID** ถูกต้อง
3. คลิกลิงก์ → **Redirect** ไปหน้าสินค้าถูก
4. ตรวจว่า **Cookie ฝังเบราว์เซอร์** ถูกต้อง

**Sub-tracking Test:**
- สร้างลิงก์แยก Facebook / Email
- Dashboard แยกข้อมูลตามช่องทางได้

---

### SLIDE 6: Scenario 3 — Tracking Test (Cookie)
## ทดสอบ Cookie Duration + Attribution
**Cookie Duration:**
1. คลิก Affiliate Link วันนี้
2. ปิดเบราว์เซอร์
3. เปิดใหม่อีก 1 วัน
4. Cookie ยังอยู่ไหม?

**Last Click Wins:**
1. คลิกลิงก์ **Affiliate A** ก่อน
2. คลิกลิงก์ **Affiliate B** ทีหลัง
3. ซื้อสินค้า
4. Commission ต้องไปหา **B** (Last Click)

---

### SLIDE 7: Scenario 4 — Test Purchase
## ทดสอบการซื้อผ่าน Affiliate Link
**วิธีทำ:**
- สร้าง Test Account
- ใช้บัตรเครดิตทดสอบ / Coupon 100% Discount
- ซื้อผ่าน Affiliate Link

**เช็ค 2 แบบ:**
| ประเภท | สิ่งที่เช็ค |
|--------|-----------|
| One-time Purchase | Order สร้างถูก, ระบุ Affiliate |
| Subscription | Order ถูก + Recurring Attribution |

> *Commission ต้องแสดงใน Dashboard สถานะ "Pending"*

---

### SLIDE 8: Scenario 5 — Commission Calculation (Cases 1-3)
## ทดสอบ 3 Cases แรก
| Case | รายละเอียด | ผลที่ถูกต้อง |
|------|-----------|-------------|
| 1. Percentage | 30% x 5,000 | = **1,500 บาท** |
| 2. Fixed Amount | 500 บาท/ขาย | = **500 บาท** |
| 3. Tiered | ชิ้นที่ 11 (20%→30%) | Commission **ขยับขึ้น** |

> *ทดสอบด้วยตัวเลขที่คำนวณง่าย ตรวจสอบได้ทันที*

---

### SLIDE 9: Scenario 5 — Commission Calculation (Cases 4-6)
## ทดสอบ 3 Cases ที่เหลือ
| Case | รายละเอียด | ผลที่ถูกต้อง |
|------|-----------|-------------|
| 4. Recurring | สมาชิกจ่ายเดือนที่ 2 | Affiliate ได้ Commission **เดือน 2** ด้วย |
| 5. Refund | ลูกค้าขอ Refund | Commission **ยกเลิกอัตโนมัติ** |
| 6. Upsell | ซื้อ Main + Upsell | Commission คำนวณ **ถูกทั้ง 2 รายการ** |

> *ทุก Case ต้อง Pass ครบ — ถ้ามี Case ไหนไม่ Pass ต้องแก้ก่อน Launch*

---

### SLIDE 10: Scenario 6 — Payment Testing
## ทดสอบระบบจ่ายเงินให้ Affiliate
| ขั้นตอน | สิ่งที่ทดสอบ |
|---------|-----------|
| 1. Pending Balance | ยอดสะสมถูกต้อง |
| 2. Payout Process | คำนวณ Payout + หักค่าธรรมเนียมถูก |
| 3. Min Threshold | ยอดไม่ถึงเกณฑ์ = แสดง "ยังไม่ถึงขั้นต่ำ" |
| 4. Refund Clawback | จ่ายไปแล้ว + Refund = หัก Commission คืน |

> *เกี่ยวกับเงินจริง — ต้องละเอียดที่สุด*

---

### SLIDE 11: Common Issues — 3 ปัญหาที่เจอบ่อย
## รู้ก่อน แก้ก่อน
| ปัญหา | สาเหตุ | วิธีแก้ |
|-------|--------|--------|
| Cookie Not Tracking | Ad Blocker / Privacy Settings | ปิด Ad Blocker หรือใช้ Direct Links |
| Commission Not Showing | ลิงก์ไม่มี Parameter / Cookie หมดอายุ | ตรวจสอบลิงก์ทุกครั้ง |
| Duplicate Commission | ซื้อผ่านหลาย Affiliate | ใช้ **Last Click Attribution** |

---

### SLIDE 12: QA Checklist — 10 ข้อก่อน Launch
## ต้อง Pass ทั้งหมด
1. Signup Flow ทำงานครบ
2. Link Generation ถูกต้อง
3. Cookie Tracking ทำงาน
4. Purchase Tracking ถูก
5. Commission Calculation ถูกทุก Case
6. Dashboard แสดงข้อมูลถูก
7. Payment Process ถูกต้อง
8. Refund Clawback ทำงาน
9. Anti-Fraud ตรวจจับได้
10. Email Notifications ส่งถูก

---

### SLIDE 13: Launch Readiness Assessment
## กี่ข้อถึงพร้อม Launch?
| QA Score | การตัดสินใจ |
|----------|-----------|
| **10/10** | พร้อม Launch ทันที |
| **8-9/10** | แก้ไขข้อที่ไม่ผ่าน → แล้ว Launch |
| **ต่ำกว่า 8/10** | **อย่าเพิ่ง Launch** — ต้องแก้ให้ครบก่อน |

> *ยิ่งแก้ก่อน Launch = ยิ่งลดปัญหาหลัง Launch*

---

### SLIDE 14: Post-launch Monitoring Plan
## Monitor อย่างเป็นระบบ
```
สัปดาห์ที่ 1-2:  Monitor ทุกวัน
                  ├── ดู Dashboard ทุกวัน
                  ├── ตรวจ Commission ทุกรายการ
                  └── ตอบคำถาม Affiliate ทันที

สัปดาห์ที่ 3-4:  Monitor ทุก 2-3 วัน
                  ├── ตรวจสอบยอดรวม
                  └── ดู Anomalies

หลัง 1 เดือน:    Monitor สัปดาห์ละครั้ง
                  ├── รายงานสรุป
                  └── Alert อัตโนมัติ
```

---

### SLIDE 15: สรุป — ด่านสุดท้ายก่อน Launch
## ทดสอบครบ = Launch อย่างมั่นใจ
1. ผ่าน **6 Test Scenarios** ครบ
2. ผ่าน **6 Commission Cases** ครบ
3. ผ่าน **QA Checklist 10 ข้อ** ครบ
4. มี **Monitoring Plan** หลัง Launch
5. รู้ **Common Issues** และวิธีแก้

> *"ตอนที่ 22 นี้คือด่านสุดท้าย ทดสอบทุก Scenario ทำ QA Checklist ให้ครบ แล้ว Monitor หลัง Launch อย่างใกล้ชิด — ขอบคุณทุกคนที่ติดตามมาตลอด 22 ตอน"*

---

*Slide count: 15 | Presentation time: 20-25 minutes*
