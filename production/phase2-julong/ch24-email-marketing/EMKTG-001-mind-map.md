# Email Marketing ตอนที่ 1 — EMKTG-001 Mind Map
> **Format:** Mind Map (Text Structure + Mermaid)
> **Source:** SWP3 Ch24 Email Marketing Mastery ตอนที่ 1
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 2:31:44

---

## Part 1: Mind Map — โครงสร้างข้อความ (Text Structure)

```
Email Marketing Mastery ตอนที่ 1
│
├── 1. ทำไม Email Marketing ยังสำคัญ
│   ├── ROI สูงสุด 36-42 เท่า
│   ├── Owned Media
│   │   └── เป็นเจ้าของ List จริงๆ
│   ├── ไม่ขึ้นกับ Algorithm
│   │   └── Facebook เปลี่ยน → Reach ตก
│   ├── Inbox = พื้นที่ส่วนตัว
│   │   └── คนยอมให้เข้า = สนใจจริง
│   └── Conversion Rate
│       └── สูงกว่า Social Media 3-5 เท่า
│
├── 2. การสร้าง Email List ตั้งแต่ศูนย์
│   ├── Lead Magnet (กุญแจสำคัญ)
│   │   ├── ต้องแก้ปัญหาเฉพาะเจาะจง
│   │   └── 5 รูปแบบ
│   │       ├── ebook
│   │       ├── Checklist
│   │       ├── Template
│   │       ├── Video Series
│   │       └── Free Tool
│   └── Opt-in Form (จุดเก็บอีเมล)
│       ├── Homepage
│       ├── Blog Post
│       ├── Pop-up
│       └── Dedicated Landing Page
│
├── 3. Opt-in Strategies + Welcome Sequence
│   ├── Single Opt-in
│   │   └── กรอกปุ๊บ เข้า List เลย
│   ├── Double Opt-in (แนะนำ)
│   │   └── ยืนยันอีเมลก่อน → List สะอาด
│   └── Welcome Sequence (5 ฉบับ)
│       ├── ฉบับ 1: ส่ง Lead Magnet + แนะนำตัว
│       ├── ฉบับ 2: เล่าเรื่องราว Origin Story
│       ├── ฉบับ 3: ให้คุณค่าเพิ่มเติม
│       ├── ฉบับ 4: ถามปัญหา/สำรวจ
│       └── ฉบับ 5: แนะนำสินค้า Soft Sell
│
├── 4. List Hygiene + Deliverability
│   ├── List Hygiene
│   │   ├── ทำทุก 3-6 เดือน
│   │   ├── ไม่เปิดอ่าน 90 วัน → Re-engagement
│   │   └── ยังเงียบ → ลบออก
│   └── Deliverability (4 ปัจจัย)
│       ├── Sender Reputation
│       ├── Authentication (SPF/DKIM/DMARC)
│       ├── Engagement Rate
│       └── Bounce Rate
│
└── 5. เลือก Email Platform
    ├── Mailchimp
    │   ├── ฟรี 500 คน
    │   ├── UI สวย ใช้ง่าย
    │   └── เหมาะกับมือใหม่
    ├── GetResponse
    │   ├── ~$15/เดือน
    │   ├── Landing Page ในตัว
    │   └── เหมาะกับเริ่มจริงจัง
    └── ActiveCampaign
        ├── ~$29/เดือน
        ├── Automation ยอดเยี่ยม
        └── เหมาะกับมืออาชีพ
```

---

## Part 2: Mind Map — Mermaid Diagram

```mermaid
mindmap
  root((Email Marketing<br/>Mastery ตอนที่ 1))
    ทำไมยังสำคัญ
      ROI 36-42x<br/>สูงสุดทุกช่องทาง
      Owned Media<br/>เป็นเจ้าของ List จริง
      ไม่ขึ้นกับ Algorithm
      Conversion Rate<br/>สูงกว่า Social 3-5x
    สร้าง Email List
      Lead Magnet<br/>แก้ปัญหาเฉพาะเจาะจง
      5 รูปแบบ<br/>ebook Checklist Template<br/>Video Tool
      Opt-in Form<br/>Homepage Blog Pop-up<br/>Landing Page
    Opt-in + Welcome
      Single Opt-in<br/>เข้า List ทันที
      Double Opt-in<br/>ยืนยันก่อน List สะอาด
      Welcome Sequence<br/>5 ฉบับอัตโนมัติ
    List Hygiene
      ทำทุก 3-6 เดือน
      90 วันไม่เปิด<br/>ส่ง Re-engagement
      ยังเงียบ ลบออก
    Deliverability
      Sender Reputation
      SPF DKIM DMARC
      Engagement Rate
      Bounce Rate
    เลือก Platform
      Mailchimp<br/>มือใหม่ ฟรี 500
      GetResponse<br/>จริงจัง $15 ต่อเดือน
      ActiveCampaign<br/>มืออาชีพ $29 ต่อเดือน
```

---

## Part 3: Flowchart — Email List Building Journey

```mermaid
graph LR
    A["สร้าง Lead Magnet<br/>(ebook/Checklist/Template)"] --> B["วาง Opt-in Form<br/>(Homepage/Blog/Pop-up)"]
    B --> C{"เลือกแบบ Opt-in"}
    C -->|Single| D["เข้า List ทันที<br/>List โตเร็ว"]
    C -->|Double| E["ยืนยันทางอีเมล<br/>List สะอาด"]
    D --> F["Welcome Sequence<br/>5 ฉบับอัตโนมัติ"]
    E --> F
    F --> G["สร้างความสัมพันธ์<br/>ให้คุณค่าก่อนขาย"]
    G --> H["Soft Sell<br/>แนะนำสินค้า/บริการ"]

    style A fill:#FF69B4,stroke:#FF1493,color:#fff
    style F fill:#FFD700,stroke:#FFA500,color:#000
    style H fill:#4CAF50,stroke:#388E3C,color:#fff
```

---

## Part 4: Flowchart — Welcome Sequence Timeline

```mermaid
graph TB
    T0["สมัครเข้า List"] --> E1["อีเมล 1<br/>ส่ง Lead Magnet<br/>+ แนะนำตัว<br/>ส่งทันที"]
    E1 --> E2["อีเมล 2<br/>Origin Story<br/>สร้าง Connection<br/>วันที่ 2"]
    E2 --> E3["อีเมล 3<br/>ให้คุณค่าเพิ่ม<br/>Tips/Insights<br/>วันที่ 4"]
    E3 --> E4["อีเมล 4<br/>ถามปัญหา<br/>เข้าใจ Audience<br/>วันที่ 6"]
    E4 --> E5["อีเมล 5<br/>Soft Sell<br/>แนะนำสินค้า<br/>วันที่ 8"]
    E5 --> NEXT["เข้าสู่ Regular Email<br/>จดหมายข่าวรายสัปดาห์"]

    style T0 fill:#FF69B4,stroke:#FF1493,color:#fff
    style E1 fill:#FFB6C1,stroke:#FF69B4
    style E2 fill:#FFB6C1,stroke:#FF69B4
    style E3 fill:#FFB6C1,stroke:#FF69B4
    style E4 fill:#FFB6C1,stroke:#FF69B4
    style E5 fill:#FFD700,stroke:#FFA500,color:#000
    style NEXT fill:#4CAF50,stroke:#388E3C,color:#fff
```

---

## Part 5: Flowchart — List Hygiene Process

```mermaid
graph TD
    START["ตรวจ Email List<br/>ทุก 3-6 เดือน"] --> CHECK{"สมาชิกเปิดอ่าน<br/>ใน 90 วันไหม?"}
    CHECK -->|เปิดอ่าน| ACTIVE["Active Subscriber<br/>ส่งเนื้อหาตามปกติ"]
    CHECK -->|ไม่เปิด| REENGAGE["ส่ง Re-engagement<br/>Email"]
    REENGAGE --> RESPOND{"ตอบกลับ<br/>หรือเปิดอ่านไหม?"}
    RESPOND -->|ตอบ| ACTIVE
    RESPOND -->|เงียบ| REMOVE["ลบออกจาก List"]
    REMOVE --> CLEAN["List สะอาดขึ้น<br/>Deliverability ดีขึ้น"]

    style START fill:#FF69B4,stroke:#FF1493,color:#fff
    style ACTIVE fill:#4CAF50,stroke:#388E3C,color:#fff
    style REMOVE fill:#FF6B6B,stroke:#FF1493,color:#fff
    style CLEAN fill:#FFD700,stroke:#FFA500,color:#000
```

---

## Part 6: เปรียบเทียบ — Email Marketing vs Social Media

| ด้าน | Email Marketing | Social Media |
|-----|----------------|-------------|
| **ความเป็นเจ้าของ** | Owned Media (เราเป็นเจ้าของ) | Rented Media (ยืมพื้นที่) |
| **ROI** | 36-42x | 5-10x |
| **Algorithm** | ไม่มีผลกระทบ | เปลี่ยนตลอด Reach ตกได้ |
| **Conversion** | สูงกว่า 3-5 เท่า | ต่ำกว่า |
| **ความเป็นส่วนตัว** | Inbox ส่วนตัว | Feed สาธารณะ |
| **ต้นทุน** | ต่ำ-ปานกลาง | ค่า Ads สูงขึ้นเรื่อยๆ |
| **สรุป** | สินทรัพย์ระยะยาว | เครื่องมือเสริม |

---

## Part 7: สรุปโครงสร้าง Mind Map

| กิ่งหลัก | จำนวนกิ่งย่อย | ประเด็นสำคัญ |
|---------|-------------|-------------|
| ทำไมยังสำคัญ | 5 | ROI 36-42x, Owned Media, ไม่ขึ้น Algorithm, Inbox ส่วนตัว, Conversion สูง |
| สร้าง Email List | 7 | Lead Magnet 5 แบบ + Opt-in Form 4 จุด |
| Opt-in + Welcome | 8 | Single/Double Opt-in + Welcome Sequence 5 ฉบับ |
| List Hygiene | 4 | ทุก 3-6 เดือน, 90 วัน threshold, Re-engagement, ลบออก |
| Deliverability | 4 | Sender Reputation, SPF/DKIM/DMARC, Engagement, Bounce Rate |
| เลือก Platform | 6 | Mailchimp (มือใหม่) / GetResponse (จริงจัง) / ActiveCampaign (มืออาชีพ) |

**จำนวน node ทั้งหมด:** 41 nodes (6 กิ่งหลัก + 35 กิ่งย่อย)

---

> **หมายเหตุ:** Mermaid mindmap สามารถ render ได้ใน GitHub, Notion (embed), VS Code (Mermaid Preview extension)
> Flowchart แบบทางเลือกใช้ได้ในกรณีที่ platform ไม่รองรับ mindmap syntax

---

> ทบทวนต่อ: **EMKTG-002** — Email Marketing ตอนที่ 2
> Series: SWP3 Ch24 Email Marketing Mastery
> PinkCastle Academy © 2026
