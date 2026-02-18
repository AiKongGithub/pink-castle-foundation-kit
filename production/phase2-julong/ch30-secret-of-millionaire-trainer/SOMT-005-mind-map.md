# วิธี Deploy Membership System — SOMT-005
> **Format:** Mind Map
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 5
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

## Text Tree Mind Map

```
Deploy Membership System บน Kartra
│
├── 1. สร้าง Membership Portal
│   ├── เข้า Kartra Dashboard → Memberships → New
│   ├── ตั้งชื่อ Membership
│   ├── เลือก Template
│   │   ├── Modern
│   │   ├── Classic
│   │   └── Sidebar Navigation
│   ├── ใส่ Description
│   └── ใส่ Welcome Message
│
├── 2. ตั้งค่า Membership Levels
│   ├── Add Level: Silver
│   │   ├── Access: Category 1-5 เท่านั้น
│   │   ├── Content Dripping: สัปดาห์ละ 1 Module
│   │   └── ราคา: 990 บาท/เดือน
│   ├── Add Level: Gold
│   │   ├── Access: ทุก Category
│   │   ├── Content Dripping: สัปดาห์ละ 1 Module
│   │   └── ราคา: 2,990 บาท/เดือน
│   └── Access Rules
│       ├── Level-based access
│       ├── Time-based dripping
│       └── Locked Content → "Upgrade" page
│
├── 3. Domain Configuration
│   ├── Custom Domain (แนะนำ)
│   │   ├── เพิ่ม Domain ใน "My Domains"
│   │   ├── ตั้ง DNS: CNAME → Kartra
│   │   └── ตัวอย่าง: members.yourbrand.com
│   └── Kartra Subdomain (ง่าย)
│       ├── ใช้งานได้ทันที
│       └── ตัวอย่าง: yourbrand.kartra.com
│
├── 4. SSL Setup
│   ├── Kartra ให้ SSL ฟรี
│   ├── เข้า Domain Settings → Enable SSL
│   ├── รอ Provision ไม่เกิน 24 ชม.
│   └── ผลลัพธ์: HTTPS (กุญแจล็อค)
│       ├── ความปลอดภัย
│       ├── ความน่าเชื่อถือ
│       └── จำเป็นสำหรับ Payment
│
├── 5. Payment Setup
│   ├── เชื่อมต่อ Payment Gateway
│   │   ├── Stripe (Credit/Debit Card)
│   │   └── PayPal
│   ├── สร้าง Products
│   │   ├── Silver Product: 990 บาท/เดือน
│   │   └── Gold Product: 2,990 บาท/เดือน
│   ├── เชื่อม Product ↔ Membership Level
│   ├── ตั้ง Recurring Billing
│   └── ทดสอบด้วย Test Mode
│
├── 6. ทดสอบ & Go Live
│   ├── Testing Checklist
│   │   ├── Signup Flow ✓
│   │   ├── Payment (Test Card) ✓
│   │   ├── Access Control ✓
│   │   ├── Content Dripping ✓
│   │   ├── Welcome Email ✓
│   │   └── Cancellation Flow ✓
│   ├── Soft Launch (5-10 Beta Members)
│   ├── เก็บ Feedback + แก้ไข
│   └── Public Launch! 🚀
│
└── 7. สรุปซีรีส์ 5 ตอน
    ├── ตอน 1: Identity & Mindset
    ├── ตอน 2: Revenue Strategies
    ├── ตอน 3: Empire Model
    ├── ตอน 4: Membership System
    └── ตอน 5: Deploy (ตอนนี้)
```

---

## Mermaid Mind Map

```mermaid
mindmap
  root((Deploy Membership<br/>SOMT-005))
    สร้าง Portal
      ตั้งชื่อ
      เลือก Template
      Description
      Welcome Message
    ตั้งค่า Levels
      Silver
        Access จำกัด
        990 บาท/เดือน
      Gold
        Access ทั้งหมด
        2990 บาท/เดือน
      Access Rules
    Domain Config
      Custom Domain
        CNAME DNS
      Kartra Subdomain
        ใช้ทันที
    SSL Setup
      ฟรีจาก Kartra
      Enable SSL
      รอ 24 ชม
    Payment Setup
      Stripe PayPal
      สร้าง Products
      Recurring Billing
      Test Mode
    Testing & Go Live
      Signup Flow
      Payment Test
      Access Control
      Content Dripping
      Welcome Email
      Soft Launch
```

---

## Deployment Flow Diagram

```mermaid
graph TD
    A[1. สร้าง Portal<br/>+ เลือก Template] --> B[2. ตั้งค่า Levels<br/>Silver & Gold]
    B --> C[3. Domain Config<br/>Custom หรือ Subdomain]
    C --> D[4. SSL Setup<br/>Enable HTTPS]
    D --> E[5. Payment Setup<br/>Stripe/PayPal]
    E --> F[6. Testing<br/>6-point checklist]
    F --> G{ทดสอบ<br/>ผ่านหมด?}
    G -->|ผ่าน| H[Soft Launch<br/>5-10 Beta Members]
    G -->|ไม่ผ่าน| I[แก้ไข] --> F
    H --> J[เก็บ Feedback]
    J --> K[Public Launch!]

    style A fill:#E8F5E9
    style B fill:#E3F2FD
    style C fill:#FFF3E0
    style D fill:#F3E5F5
    style E fill:#FFEBEE
    style K fill:#C8E6C9
```

---

## Series Journey Map

```mermaid
graph LR
    A[SOMT-001<br/>Identity & Mindset] --> B[SOMT-002<br/>Revenue Strategies]
    B --> C[SOMT-003<br/>Empire Model]
    C --> D[SOMT-004<br/>Membership System]
    D --> E[SOMT-005<br/>Deploy!]

    A -.->|"รู้จักตัวเอง"| B
    B -.->|"รู้วิธีสร้างรายได้"| C
    C -.->|"มี Framework"| D
    D -.->|"มี System Design"| E

    style E fill:#FFD700,stroke:#B8860B,stroke-width:3px
```

---

*สิ้นสุด Mind Map — SOMT-005*
