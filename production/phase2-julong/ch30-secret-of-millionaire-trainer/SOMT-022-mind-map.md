# ทดสอบระบบ Affiliate — SOMT-022
> **Format:** Mind Map (Text + Mermaid)
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 22
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18
> **Duration:** 0:46:41

---

## Text Mind Map (30+ Nodes)

```
ทดสอบระบบ Affiliate (End-to-End Testing)
│
├── 1. Scenario 1: Signup Test
│   ├── กรอกฟอร์มสมัคร
│   │   ├── ทุกช่องกรอกได้ครบ
│   │   ├── Error Messages แสดงเมื่อกรอกผิด
│   │   └── T&C Checkbox ทำงาน
│   ├── Approval Process
│   │   ├── Auto-approve ทำงานตามที่ตั้ง
│   │   └── Manual Review ทำงานตามที่ตั้ง
│   ├── Welcome Email
│   │   ├── ส่งอัตโนมัติ
│   │   └── เนื้อหาถูกต้อง
│   └── Dashboard เริ่มต้น
│       └── แสดงข้อมูล 0 ทั้งหมด
│
├── 2. Scenario 2: Link Generation Test
│   ├── สร้าง Tracking Link
│   │   ├── ลิงก์มี Affiliate ID
│   │   └── Redirect ไปหน้าสินค้าถูก
│   ├── Sub-tracking
│   │   ├── ลิงก์สำหรับ Facebook
│   │   ├── ลิงก์สำหรับ Email
│   │   └── Dashboard แยกข้อมูลได้
│   └── Cookie ฝังเบราว์เซอร์
│       └── ตรวจสอบ Cookie Parameters
│
├── 3. Scenario 3: Tracking Test
│   ├── Cookie Duration
│   │   ├── คลิกวันนี้ → ปิดเบราว์เซอร์
│   │   ├── เปิดใหม่อีก 1 วัน
│   │   └── Cookie ยังอยู่ไหม?
│   ├── Last Click Wins
│   │   ├── คลิก Affiliate A ก่อน
│   │   ├── คลิก Affiliate B ทีหลัง
│   │   └── Commission ไปหา B ถูกต้อง
│   └── Cross-browser Testing
│       ├── Chrome
│       ├── Safari
│       └── Firefox
│
├── 4. Scenario 4: Test Purchase
│   ├── สร้าง Test Account
│   ├── ใช้บัตรเครดิตทดสอบ / Coupon 100%
│   ├── One-time Purchase
│   │   ├── Order สร้างถูก
│   │   └── ระบุ Affiliate ถูก
│   ├── Subscription Purchase
│   │   ├── Order สร้างถูก
│   │   └── Recurring Attribution
│   └── Commission แสดงใน Dashboard
│       └── สถานะ "Pending"
│
├── 5. Scenario 5: Commission Calculation
│   ├── Case 1: Percentage
│   │   └── 30% x 5,000 = 1,500
│   ├── Case 2: Fixed Amount
│   │   └── 500 บาท/ขาย
│   ├── Case 3: Tiered Commission
│   │   └── ชิ้นที่ 11 → 20% เป็น 30%
│   ├── Case 4: Recurring
│   │   └── เดือนที่ 2+ ได้ Commission
│   ├── Case 5: Refund
│   │   └── Commission ยกเลิกอัตโนมัติ
│   └── Case 6: Upsell
│       └── Main + Upsell คำนวณถูก
│
├── 6. Scenario 6: Payment Testing
│   ├── Pending Commission ยอดสะสมถูก
│   ├── Payout Process
│   │   ├── Payout Amount ถูก
│   │   └── หักค่าธรรมเนียมถูก
│   ├── Minimum Payout Threshold
│   │   └── ยังไม่ถึงเกณฑ์ = ไม่ให้ถอน
│   └── Refund Clawback
│       └── หัก Commission คืนจาก Pending งวดถัดไป
│
├── 7. Common Issues
│   ├── Cookie Not Tracking
│   │   ├── Ad Blocker
│   │   └── Privacy Settings
│   ├── Commission Not Showing
│   │   ├── ลิงก์ไม่มี Parameter
│   │   └── Cookie หมดอายุ
│   └── Duplicate Commission
│       └── ใช้ Last Click Attribution
│
├── 8. QA Checklist (10 ข้อ)
│   ├── 1. Signup Flow ✓
│   ├── 2. Link Generation ✓
│   ├── 3. Cookie Tracking ✓
│   ├── 4. Purchase Tracking ✓
│   ├── 5. Commission Calculation ✓
│   ├── 6. Dashboard Display ✓
│   ├── 7. Payment Process ✓
│   ├── 8. Refund Clawback ✓
│   ├── 9. Anti-Fraud Detection ✓
│   └── 10. Email Notifications ✓
│
└── 9. Launch Readiness & Monitoring
    ├── Pass 10/10 → พร้อม Launch
    ├── Pass 8-9/10 → แก้ก่อน Launch
    ├── ต่ำกว่า 8/10 → อย่าเพิ่ง Launch
    └── Post-launch Monitor
        ├── สัปดาห์ที่ 1: ดูทุกวัน
        ├── สัปดาห์ที่ 2: ดูทุกวัน
        └── หลัง 2 สัปดาห์: สัปดาห์ละครั้ง
```

---

## Mermaid Mind Map

```mermaid
mindmap
  root((ทดสอบระบบ Affiliate))
    Scenario 1: Signup
      กรอกฟอร์ม
        ทุกช่องครบ
        Error Messages
      Approval Process
        Auto-approve
        Manual Review
      Welcome Email
      Dashboard เริ่มต้น
    Scenario 2: Link Generation
      Tracking Link
        Affiliate ID
        Redirect ถูก
      Sub-tracking
        Facebook
        Email
      Cookie ฝังเบราว์เซอร์
    Scenario 3: Tracking
      Cookie Duration
        ปิด-เปิดเบราว์เซอร์
      Last Click Wins
        A ก่อน B ทีหลัง
      Cross-browser
    Scenario 4: Test Purchase
      Test Account
      One-time Purchase
      Subscription
      Commission Pending
    Scenario 5: Commission
      Percentage 30%
      Fixed Amount
      Tiered Commission
      Recurring
      Refund Cancel
      Upsell
    Scenario 6: Payment
      Pending Balance
      Payout Process
      Minimum Threshold
      Refund Clawback
    Common Issues
      Cookie Not Tracking
      Commission Not Showing
      Duplicate Commission
    QA Checklist 10 ข้อ
      Pass 10 = Launch
      Pass 8-9 = แก้ก่อน
      ต่ำกว่า 8 = ห้าม Launch
    Post-launch Monitor
      สัปดาห์ 1-2 ทุกวัน
      หลัง 2 สัปดาห์ ลดลง
```

---

## Mermaid Flowchart — End-to-End Testing Process

```mermaid
flowchart TD
    START([เริ่มทดสอบระบบ Affiliate]) --> S1

    subgraph S1 [Scenario 1: Signup Test]
        S1A[กรอกฟอร์มสมัคร] --> S1B[ตรวจ Error Messages]
        S1B --> S1C{Approval ทำงาน?}
        S1C -->|Yes| S1D[ตรวจ Welcome Email]
        S1D --> S1E[ตรวจ Dashboard เริ่มต้น]
    end

    S1E --> S2

    subgraph S2 [Scenario 2: Link Generation]
        S2A[สร้าง Tracking Link] --> S2B[ตรวจ Affiliate ID]
        S2B --> S2C[ทดสอบ Redirect]
        S2C --> S2D[ทดสอบ Sub-tracking]
    end

    S2D --> S3

    subgraph S3 [Scenario 3: Tracking Test]
        S3A[ทดสอบ Cookie Duration] --> S3B[ทดสอบ Last Click Wins]
        S3B --> S3C[Cross-browser Testing]
    end

    S3C --> S4

    subgraph S4 [Scenario 4: Test Purchase]
        S4A[สร้าง Test Account] --> S4B[ซื้อผ่าน Affiliate Link]
        S4B --> S4C[ตรวจ Order Attribution]
        S4C --> S4D[ตรวจ Commission Pending]
    end

    S4D --> S5

    subgraph S5 [Scenario 5: Commission Calculation]
        S5A[Case 1: Percentage] --> S5B[Case 2: Fixed]
        S5B --> S5C[Case 3: Tiered]
        S5C --> S5D[Case 4: Recurring]
        S5D --> S5E[Case 5: Refund]
        S5E --> S5F[Case 6: Upsell]
    end

    S5F --> S6

    subgraph S6 [Scenario 6: Payment Testing]
        S6A[ตรวจ Pending Balance] --> S6B[จำลอง Payout]
        S6B --> S6C[ทดสอบ Minimum Threshold]
        S6C --> S6D[ทดสอบ Refund Clawback]
    end

    S6D --> QA

    subgraph QA [QA Checklist]
        QA1[ตรวจ 10 ข้อ] --> QA2{ผ่านกี่ข้อ?}
        QA2 -->|10/10| LAUNCH[พร้อม Launch!]
        QA2 -->|8-9/10| FIX[แก้ไขก่อน Launch]
        QA2 -->|ต่ำกว่า 8| STOP[อย่าเพิ่ง Launch]
        FIX --> LAUNCH
        STOP --> S1A
    end

    LAUNCH --> MONITOR

    subgraph MONITOR [Post-launch Monitoring]
        M1[สัปดาห์ 1-2: Monitor ทุกวัน] --> M2[สัปดาห์ 3-4: Monitor ทุก 2-3 วัน]
        M2 --> M3[หลัง 1 เดือน: สัปดาห์ละครั้ง]
    end

    S1C -->|No| S1FIX[แก้ไข Approval] --> S1A

    style START fill:#FF6B6B,color:#fff
    style LAUNCH fill:#51CF66,color:#fff
    style STOP fill:#FF6B6B,color:#fff
    style FIX fill:#FFD43B,color:#333
```

---

*Node count: 65+ | Diagrams: 3 (Text Tree + Mermaid Mind Map + Flowchart)*
