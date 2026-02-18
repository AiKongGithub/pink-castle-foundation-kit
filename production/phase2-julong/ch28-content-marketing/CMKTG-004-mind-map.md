# TOFU & MOFU — CMKTG-004 Mind Map
> **Format:** Mind Map (Text Structure + Mermaid)
> **Source:** SWP3 Ch28 Content Marketing Mastery ตอนที่ 4
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:20:10

---

## Part 1: Mind Map — โครงสร้างข้อความ (Text Structure)

```
TOFU & MOFU
│
├── 1. TOFU (Top of Funnel)
│   ├── เป้าหมาย: สร้าง Awareness
│   ├── กลุ่มเป้าหมาย: คนที่ยังไม่รู้จักเรา
│   ├── หลักการ: ให้คุณค่า ไม่ใช่ขายของ (96% ยังไม่พร้อมซื้อ)
│   └── เครื่องมือ 4 ตัวหลัก
│       ├── Blog + SEO — ดึง traffic จาก Google 24/7
│       ├── Social Media — Facebook, IG, TikTok, YouTube, X
│       ├── Video Content — How-to, Tutorial (engagement +1,200%)
│       └── Infographic — แปลงข้อมูลซับซ้อนเป็นภาพ
│
├── 2. MOFU (Middle of Funnel)
│   ├── เป้าหมาย: สร้างความเชื่อมั่น (Trust & Consideration)
│   ├── กลุ่มเป้าหมาย: คนที่รู้จักเราแล้ว กำลังเปรียบเทียบ
│   ├── หลักการ: แสดงความเชี่ยวชาญ + หลักฐานจริง
│   └── เครื่องมือ 4 ตัวหลัก
│       ├── Case Study — Before/Solution/After + ตัวเลข
│       ├── Webinar — ความรู้เชิงลึก + เก็บ email (73% B2B ยืนยัน)
│       ├── E-book / Lead Magnet — เนื้อหาเชิงลึกแลก email
│       └── Email Sequence — 5-7 ฉบับ, ROI $36/$1
│
├── 3. TOFU KPI (วัด Awareness)
│   ├── Website Traffic — จำนวนคนเข้าเว็บ
│   ├── Social Media Reach — จำนวนคนเห็นโพสต์
│   ├── Impressions — จำนวนครั้งที่เนื้อหาถูกแสดง
│   ├── Video Views — จำนวนคนดูวิดีโอ
│   └── Brand Mentions — จำนวนครั้งที่คนพูดถึงแบรนด์
│
├── 4. MOFU KPI (วัด Engagement & Leads)
│   ├── Email Subscribers — จำนวนคนสมัครรับอีเมล
│   ├── Lead Magnet Downloads — จำนวนดาวน์โหลด
│   ├── Webinar Registrations — จำนวนลงทะเบียน
│   ├── Email Open Rate — เป้า 20%+
│   └── Time on Page — ยิ่งนาน = ยิ่งมีคุณค่า
│
├── 5. Conversion Rate
│   ├── TOFU → MOFU = 2-5%
│   ├── Traffic 10,000 → Leads 200-500
│   └── TOFU ต้องสร้าง traffic มากพอ
│
├── 6. เครื่องมือวัดผล
│   ├── TOFU: GA4, Google Search Console, Social Analytics
│   ├── MOFU: Email Platform, CRM, Webinar Platform
│   └── เทคนิค: UTM Parameters + Content Scoring
│
└── 7. หลักการสำคัญ
    ├── TOFU เน้นปริมาณ, MOFU เน้นคุณภาพ
    ├── ทำทั้งสองชั้นให้สมดุล
    └── ขาดชั้นใดชั้นหนึ่ง Funnel จะรั่ว
```

---

## Part 2: Mind Map — Mermaid Diagram

```mermaid
mindmap
  root((TOFU & MOFU))
    TOFU - Top of Funnel
      เป้าหมาย: Awareness
      96% ยังไม่พร้อมซื้อ
      Blog + SEO
      Social Media
      Video Content
      Infographic
    MOFU - Middle of Funnel
      เป้าหมาย: Trust
      แสดงความเชี่ยวชาญ
      Case Study
      Webinar
      E-book / Lead Magnet
      Email Sequence
    TOFU KPI
      Website Traffic
      Social Reach
      Impressions
      Video Views
      Brand Mentions
    MOFU KPI
      Email Subscribers
      Lead Downloads
      Webinar Registrations
      Open Rate 20%+
      Time on Page
    Conversion
      TOFU to MOFU: 2-5%
      10,000 traffic = 200-500 leads
    วัดผล
      GA4 + GSC
      Email Platform + CRM
      UTM Parameters
      Content Scoring
```

---

## Part 3: Flowchart — Content Marketing Funnel (TOFU → MOFU → BOFU)

```mermaid
graph TB
    TOFU["TOFU<br/>Top of Funnel<br/>สร้าง Awareness"]
    MOFU["MOFU<br/>Middle of Funnel<br/>สร้างความเชื่อมั่น"]
    BOFU["BOFU<br/>Bottom of Funnel<br/>ปิดการขาย"]

    TOFU --> |"Conversion 2-5%"| MOFU
    MOFU --> BOFU

    subgraph "TOFU เครื่องมือ"
        T1["Blog + SEO<br/>ดึง traffic 24/7"]
        T2["Social Media<br/>Reels, TikTok"]
        T3["Video Content<br/>YouTube How-to"]
        T4["Infographic<br/>ข้อมูลเป็นภาพ"]
    end

    subgraph "MOFU เครื่องมือ"
        M1["Case Study<br/>Before/Solution/After"]
        M2["Webinar<br/>ความรู้เชิงลึก"]
        M3["E-book<br/>Lead Magnet"]
        M4["Email Sequence<br/>5-7 ฉบับ"]
    end

    T1 --> TOFU
    T2 --> TOFU
    T3 --> TOFU
    T4 --> TOFU

    M1 --> MOFU
    M2 --> MOFU
    M3 --> MOFU
    M4 --> MOFU

    style TOFU fill:#87CEEB,stroke:#4682B4,color:#000,stroke-width:3px
    style MOFU fill:#FFD700,stroke:#FFA500,color:#000,stroke-width:3px
    style BOFU fill:#FF69B4,stroke:#FF1493,color:#fff,stroke-width:3px
    style T1 fill:#E3F2FD,stroke:#64B5F6
    style T2 fill:#E3F2FD,stroke:#64B5F6
    style T3 fill:#E3F2FD,stroke:#64B5F6
    style T4 fill:#E3F2FD,stroke:#64B5F6
    style M1 fill:#FFF8E1,stroke:#FFD54F
    style M2 fill:#FFF8E1,stroke:#FFD54F
    style M3 fill:#FFF8E1,stroke:#FFD54F
    style M4 fill:#FFF8E1,stroke:#FFD54F
```

---

## Part 4: Flowchart — TOFU Content Journey

```mermaid
graph LR
    STRANGER["คนแปลกหน้า<br/>(ยังไม่รู้จักเรา)"]

    STRANGER --> |"ค้นหาใน Google"| BLOG["Blog + SEO<br/>บทความตอบคำถาม"]
    STRANGER --> |"เลื่อน feed"| SOCIAL["Social Media<br/>โพสต์ educational"]
    STRANGER --> |"ดู YouTube"| VIDEO["Video<br/>How-to / Tutorial"]
    STRANGER --> |"เห็นถูก share"| INFO["Infographic<br/>ข้อมูลเป็นภาพ"]

    BLOG --> AWARE["รู้จักแบรนด์<br/>(Awareness)"]
    SOCIAL --> AWARE
    VIDEO --> AWARE
    INFO --> AWARE

    AWARE --> |"สนใจเพิ่ม"| MOFU["เข้าสู่ MOFU<br/>2-5% ของ traffic"]

    style STRANGER fill:#E0E0E0,stroke:#9E9E9E,color:#000
    style BLOG fill:#E3F2FD,stroke:#64B5F6
    style SOCIAL fill:#E3F2FD,stroke:#64B5F6
    style VIDEO fill:#E3F2FD,stroke:#64B5F6
    style INFO fill:#E3F2FD,stroke:#64B5F6
    style AWARE fill:#87CEEB,stroke:#4682B4,color:#000
    style MOFU fill:#FFD700,stroke:#FFA500,color:#000
```

---

## Part 5: Flowchart — MOFU Nurturing Journey

```mermaid
graph LR
    LEAD["ผู้สนใจ<br/>(รู้จักเราแล้ว)"]

    LEAD --> |"อ่านเรื่องจริง"| CASE["Case Study<br/>Before/Solution/After"]
    LEAD --> |"ลงทะเบียน"| WEBINAR["Webinar<br/>สัมมนาออนไลน์"]
    LEAD --> |"ดาวน์โหลดแลก email"| EBOOK["E-book<br/>Lead Magnet"]

    CASE --> TRUST["เชื่อมั่น<br/>(Trust)"]
    WEBINAR --> TRUST
    EBOOK --> EMAIL["Email Sequence<br/>5-7 ฉบับ<br/>Nurturing"]
    EMAIL --> TRUST

    TRUST --> |"พร้อมซื้อ"| BOFU["เข้าสู่ BOFU<br/>(ปิดการขาย)"]

    style LEAD fill:#FFF8E1,stroke:#FFD54F
    style CASE fill:#FFF3E0,stroke:#FFB74D
    style WEBINAR fill:#FFF3E0,stroke:#FFB74D
    style EBOOK fill:#FFF3E0,stroke:#FFB74D
    style EMAIL fill:#FFF3E0,stroke:#FFB74D
    style TRUST fill:#FFD700,stroke:#FFA500,color:#000
    style BOFU fill:#FF69B4,stroke:#FF1493,color:#fff
```

---

## Part 6: Comparison Diagram — TOFU vs MOFU

```mermaid
graph TB
    subgraph "TOFU — Top of Funnel"
        TE["เป้าหมาย: Awareness"]
        TG["กลุ่ม: คนแปลกหน้า"]
        TT["เครื่องมือ: Blog, Social<br/>Video, Infographic"]
        TK["KPI: Traffic, Reach<br/>Views, Impressions"]
        TF["เน้น: ปริมาณ (Quantity)"]
    end

    subgraph "MOFU — Middle of Funnel"
        ME["เป้าหมาย: Trust & Consideration"]
        MG["กลุ่ม: คนที่รู้จักแล้ว"]
        MT["เครื่องมือ: Case Study, Webinar<br/>E-book, Email Sequence"]
        MK["KPI: Leads, Subscribers<br/>Open Rate, Time on Page"]
        MF["เน้น: คุณภาพ (Quality)"]
    end

    TE --- ME
    TG --- MG
    TT --- MT
    TK --- MK
    TF --- MF

    style TE fill:#E3F2FD,stroke:#64B5F6
    style TG fill:#E3F2FD,stroke:#64B5F6
    style TT fill:#E3F2FD,stroke:#64B5F6
    style TK fill:#E3F2FD,stroke:#64B5F6
    style TF fill:#E3F2FD,stroke:#64B5F6
    style ME fill:#FFF8E1,stroke:#FFD54F
    style MG fill:#FFF8E1,stroke:#FFD54F
    style MT fill:#FFF8E1,stroke:#FFD54F
    style MK fill:#FFF8E1,stroke:#FFD54F
    style MF fill:#FFF8E1,stroke:#FFD54F
```

---

## Part 7: Summary Box

```
+==============================================================+
|                    สรุป TOFU & MOFU                           |
+==============================================================+
|                                                              |
|   TOFU (Top of Funnel) — สร้าง Awareness                    |
|   +--------------------+----------------------------+        |
|   | Blog + SEO         | ดึง traffic 24/7 จาก Google|        |
|   | Social Media       | Reels, TikTok, เข้าถึงเร็ว |        |
|   | Video Content      | engagement +1,200%         |        |
|   | Infographic        | ข้อมูลเป็นภาพ ถูก share สูง |        |
|   +--------------------+----------------------------+        |
|                                                              |
|   MOFU (Middle of Funnel) — สร้างความเชื่อมั่น               |
|   +--------------------+----------------------------+        |
|   | Case Study         | Before/Solution/After      |        |
|   | Webinar            | 73% B2B บอกดีที่สุด        |        |
|   | E-book/Lead Magnet | แลก email ด้วยคุณค่า        |        |
|   | Email Sequence     | ROI $36/$1 สูงที่สุด!      |        |
|   +--------------------+----------------------------+        |
|                                                              |
|   Conversion Rate: TOFU → MOFU = 2-5%                       |
|   (10,000 traffic → 200-500 leads)                           |
|                                                              |
|   3 หลักการสำคัญ:                                            |
|   1. TOFU = ให้คุณค่า ไม่ใช่ขายของ (96% ยังไม่พร้อมซื้อ)    |
|   2. MOFU = สร้างความเชื่อมั่นด้วยหลักฐานจริง               |
|   3. ทำทั้งสองชั้นให้สมดุล ขาดชั้นใดชั้นหนึ่ง Funnel รั่ว!  |
|                                                              |
+==============================================================+
```

---

## สรุปโครงสร้าง Mind Map

| กิ่งหลัก | จำนวนกิ่งย่อย | ประเด็นสำคัญ |
|---------|-------------|-------------|
| TOFU (Top of Funnel) | 7 | Awareness, Blog, Social, Video, Infographic |
| MOFU (Middle of Funnel) | 7 | Trust, Case Study, Webinar, E-book, Email |
| TOFU KPI | 5 | Traffic, Reach, Impressions, Views, Mentions |
| MOFU KPI | 5 | Subscribers, Downloads, Registrations, Open Rate, Time |
| Conversion Rate | 3 | 2-5%, 10K→200-500 leads |
| เครื่องมือวัดผล | 4 | GA4, GSC, Email Platform, UTM |
| หลักการสำคัญ | 3 | ปริมาณ/คุณภาพ, สมดุล, Funnel ห้ามรั่ว |

**จำนวน nodes ทั้งหมด:** 41 nodes

---

> **หมายเหตุ:** Mermaid mindmap สามารถ render ได้ใน GitHub, Notion (embed), VS Code (Mermaid Preview extension)
> Flowchart แบบทางเลือกใช้ได้ในกรณีที่ platform ไม่รองรับ mindmap syntax

---

> ทบทวนต่อ: **CMKTG-005** — BOFU
> Series: SWP3 Ch28 Content Marketing Mastery
> PinkCastle Academy © 2026
