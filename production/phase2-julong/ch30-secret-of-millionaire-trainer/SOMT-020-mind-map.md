# ตั้งค่าระบบ Affiliate — SOMT-020 Mind Map
> **Format:** Mind Map (Text Tree + Mermaid)
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 20
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:27:08

---

## Part 1: Text Tree Mind Map

```
ตั้งค่าระบบ Affiliate (SOMT-020)
├── 📌 Central Concept
│   └── สร้างระบบ Affiliate ที่ Win-Win — จ่ายเมื่อขายได้จริง
│
├── 💰 Commission Structure
│   ├── Percentage Based
│   │   ├── 20-50% ของราคาสินค้า
│   │   └── เหมาะกับ Digital Product
│   ├── Fixed Amount
│   │   ├── จำนวนคงที่ต่อการขาย
│   │   └── เหมาะกับ Physical Product
│   ├── Tiered Commission
│   │   ├── ใหม่: 20%
│   │   ├── 10+ ชิ้น: 30%
│   │   └── 50+ ชิ้น: 40%
│   └── Recurring Commission
│       ├── จ่ายทุกเดือนตลอดที่สมาชิกอยู่
│       └── Affiliate มี Incentive รักษาสมาชิก
│
├── 🍪 Cookie Duration
│   ├── 30 วัน — สินค้าราคาต่ำ
│   ├── 60 วัน — สินค้าราคาปานกลาง (แนะนำ)
│   ├── 90 วัน — สินค้าราคาสูง
│   └── สั้นเกินไป = Affiliate ไม่ Happy
│
├── 💳 Payment Schedule
│   ├── Monthly Payment — ทุกสิ้นเดือน
│   ├── Bi-weekly — ทุก 2 สัปดาห์
│   ├── Net 30 — 30 วันหลัง Refund Period (แนะนำ)
│   └── Minimum Payout Threshold
│       ├── 500-1,000 บาท
│       └── ลดค่าธรรมเนียมโอน
│
├── 📊 Affiliate Dashboard
│   ├── Total Clicks
│   ├── Total Sales
│   ├── Conversion Rate
│   ├── Commission Earned
│   ├── Pending Payout
│   └── Sub-tracking (แยก Campaign)
│
├── 🔗 Tracking Links
│   ├── ลิงก์เฉพาะแต่ละ Affiliate
│   ├── Cookie ตามระยะที่ตั้ง
│   ├── คำนวณ Commission อัตโนมัติ
│   └── Real-time Data ใน Kartra
│
├── 📜 Terms & Conditions
│   ├── ห้ามทำ
│   │   ├── Paid Ads บนชื่อแบรนด์
│   │   ├── ส่ง Spam Email
│   │   ├── Cookie Stuffing
│   │   └── Misleading Claims
│   ├── ต้องทำ
│   │   └── เปิดเผยว่าเป็น Affiliate Link
│   └── บทลงโทษ
│       └── ยกเลิก Affiliate ทันที
│
└── 🛡️ Anti-Fraud Measures
    ├── Self-referral Detection
    │   └── บล็อค Cookie จาก Affiliate IP
    ├── IP Monitoring
    │   └── Alert เมื่อ Clicks ผิดปกติ
    ├── Manual Review
    │   └── ตรวจ Commission ก่อนจ่ายยอดใหญ่
    └── Minimum Payout
        └── ลด Incentive สำหรับ Small-scale Fraud
```

---

## Part 2: Mermaid Mind Map

```mermaid
mindmap
  root((ระบบ Affiliate))
    Commission Structure
      Percentage 20-50%
      Fixed Amount
      Tiered Commission
        20% 30% 40%
      Recurring Commission
    Cookie Duration
      30 วัน ราคาต่ำ
      60 วัน ปานกลาง
      90 วัน ราคาสูง
    Payment Schedule
      Monthly
      Net 30 แนะนำ
      Minimum Payout 500-1000
    Affiliate Dashboard
      Clicks Sales CVR
      Commission Earned
      Sub-tracking
    Tracking Links
      ลิงก์เฉพาะ
      Cookie อัตโนมัติ
      Real-time Data
    Terms and Conditions
      ห้าม Paid Ads
      ห้าม Spam
      เปิดเผย Affiliate Link
    Anti-Fraud
      Self-referral Detection
      IP Monitoring
      Manual Review
```

---

## Part 3: Mermaid Flowchart (Affiliate Sales Flow)

```mermaid
flowchart TD
    A[Affiliate ได้ Tracking Link] --> B[แชร์ลิงก์]
    B --> C[ผู้มุ่งหวังคลิกลิงก์]
    C --> D[ระบบฝัง Cookie]
    D --> E{ซื้อภายใน Cookie Period?}
    E -->|ซื้อ| F[ระบบคำนวณ Commission]
    E -->|ไม่ซื้อ| G[Cookie หมดอายุ]
    F --> H{ผ่าน Refund Period?}
    H -->|ผ่าน| I[Commission Approved]
    H -->|Refund| J[Commission Cancelled]
    I --> K{ถึง Minimum Payout?}
    K -->|ถึง| L[จ่ายเงิน Net 30]
    K -->|ยังไม่ถึง| M[สะสมต่อ]
    L --> N[Affiliate เห็นใน Dashboard]
```

---

## Part 4: Summary Statistics

| Metric | Value |
|--------|-------|
| Total Nodes | 48 |
| Primary Branches | 7 |
| Average Sub-nodes per Branch | 7 |
| Key Concepts | Commission, Cookie, Payment, Anti-Fraud |
| Platform | Kartra |
| Commission Range | 20-50% |

---

*Mind Map nodes: 48 | Focus: Affiliate System Setup on Kartra*
