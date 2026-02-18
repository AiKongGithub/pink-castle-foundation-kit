# BOFU — CMKTG-005 Mind Map
> **Format:** Mind Map (Text Structure + Mermaid)
> **Source:** SWP3 Ch28 Content Marketing Mastery ตอนที่ 5
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:08:10

---

## Part 1: Mind Map — โครงสร้างข้อความ (Text Structure)

```
BOFU (Bottom of Funnel)
│
├── 1. BOFU คืออะไร?
│   ├── เป้าหมาย: ปิดการขาย (Conversion)
│   ├── กลุ่มเป้าหมาย: คนที่พร้อมซื้อ (ผ่าน TOFU + MOFU แล้ว)
│   ├── Conversion Rate: 20-30% (เทียบ TOFU 1-2%)
│   └── หลักการ: ขจัดข้อกังวลสุดท้าย ทำให้มั่นใจ 100%
│
├── 2. เครื่องมือ BOFU — 7 ตัวหลัก
│   ├── [1] Free Trial — ทดลองใช้ฟรี (Conversion 15-25%)
│   ├── [2] Product Demo — สาธิตสินค้า เน้น Benefits (Personalized = 3x)
│   ├── [3] Testimonial — รีวิวจากลูกค้าจริง (92% อ่านก่อนซื้อ)
│   ├── [4] Comparison Chart — เปรียบเทียบคู่แข่งอย่างยุติธรรม
│   ├── [5] Case Study เชิงลึก — ROI + Timeline + ขั้นตอน implement
│   ├── [6] Guarantee/Warranty — คืนเงิน 30 วัน (+21% ยอดขาย)
│   └── [7] Pricing Page — แพ็กเกจ + Recommended + FAQ + CTA
│
├── 3. BOFU KPI (วัดการปิดการขาย)
│   ├── Conversion Rate — lead → ลูกค้า (20-30%)
│   ├── Revenue — รายได้จริง + AOV + CLV
│   └── CAC — ต้นทุนได้ลูกค้า 1 คน
│
├── 4. สูตรสำคัญ
│   ├── CAC = ค่าใช้จ่ายทั้งหมด / ลูกค้าใหม่
│   ├── CLV = AOV x ความถี่ซื้อ x อายุลูกค้า
│   └── CLV/CAC Ratio ≥ 3:1 (ต่ำกว่า = ต้องปรับปรุง)
│
├── 5. ความต่างจาก TOFU & MOFU
│   ├── TOFU: Awareness → Blog, Social, Video, Infographic
│   ├── MOFU: Trust → Case Study, Webinar, E-book, Email
│   └── BOFU: Conversion → Trial, Demo, Testimonial, Guarantee
│
├── 6. เทคนิคปิดการขาย
│   ├── ลดความเสี่ยง (Guarantee, Free Trial)
│   ├── สร้าง Social Proof (Testimonial, Case Study)
│   └── ทำให้ตัดสินใจง่าย (Comparison, Pricing, CTA)
│
└── 7. หลักการสำคัญ
    ├── BOFU leads คุณภาพสูง ต้อง nurture มาจาก TOFU + MOFU
    ├── ขจัดข้อกังวลสุดท้าย = ทำให้มั่นใจ 100%
    └── ทั้ง 3 ชั้นต้องทำงานร่วมกัน ขาดชั้นใด Funnel รั่ว
```

---

## Part 2: Mind Map — Mermaid Diagram

```mermaid
mindmap
  root((BOFU))
    คืออะไร
      Bottom of Funnel
      ชั้นล่างสุด ปิดการขาย
      Conversion Rate 20-30%
      ขจัดข้อกังวลสุดท้าย
    เครื่องมือ 7 ตัว
      Free Trial 15-25%
      Product Demo 3x personalized
      Testimonial 92% อ่านก่อนซื้อ
      Comparison Chart
      Case Study เชิงลึก
      Guarantee +21% ยอดขาย
      Pricing Page + CTA
    BOFU KPI
      Conversion Rate
      Revenue + AOV + CLV
      CAC ต้นทุนได้ลูกค้า
    สูตรสำคัญ
      CLV/CAC Ratio
      อย่างน้อย 3 ต่อ 1
      ต่ำกว่า 3 = ปรับปรุง
    เทคนิคปิดการขาย
      ลดความเสี่ยง
      สร้าง Social Proof
      ทำให้ตัดสินใจง่าย
```

---

## Part 3: Flowchart — Full Marketing Funnel (TOFU → MOFU → BOFU)

```mermaid
graph TB
    TOFU["TOFU<br/>Top of Funnel<br/>สร้าง Awareness"]
    MOFU["MOFU<br/>Middle of Funnel<br/>สร้างความเชื่อมั่น"]
    BOFU["BOFU<br/>Bottom of Funnel<br/>ปิดการขาย"]
    CUSTOMER["ลูกค้าจริง!<br/>Revenue + CLV"]

    TOFU --> |"Conversion 2-5%"| MOFU
    MOFU --> |"Nurturing"| BOFU
    BOFU --> |"Conversion 20-30%"| CUSTOMER

    subgraph "BOFU เครื่องมือ 7 ตัว"
        B1["Free Trial<br/>ทดลองใช้ฟรี<br/>Conv. 15-25%"]
        B2["Product Demo<br/>สาธิตสินค้า<br/>Personalized 3x"]
        B3["Testimonial<br/>รีวิวลูกค้าจริง<br/>92% อ่านก่อนซื้อ"]
        B4["Comparison Chart<br/>เปรียบเทียบคู่แข่ง"]
        B5["Case Study เชิงลึก<br/>ROI + Timeline"]
        B6["Guarantee<br/>คืนเงิน 30 วัน<br/>+21% ยอดขาย"]
        B7["Pricing Page<br/>แพ็กเกจ + CTA"]
    end

    B1 --> BOFU
    B2 --> BOFU
    B3 --> BOFU
    B4 --> BOFU
    B5 --> BOFU
    B6 --> BOFU
    B7 --> BOFU

    style TOFU fill:#87CEEB,stroke:#4682B4,color:#000,stroke-width:3px
    style MOFU fill:#FFD700,stroke:#FFA500,color:#000,stroke-width:3px
    style BOFU fill:#FF69B4,stroke:#FF1493,color:#fff,stroke-width:3px
    style CUSTOMER fill:#32CD32,stroke:#228B22,color:#fff,stroke-width:3px
    style B1 fill:#FCE4EC,stroke:#F48FB1
    style B2 fill:#FCE4EC,stroke:#F48FB1
    style B3 fill:#FCE4EC,stroke:#F48FB1
    style B4 fill:#FCE4EC,stroke:#F48FB1
    style B5 fill:#FCE4EC,stroke:#F48FB1
    style B6 fill:#FCE4EC,stroke:#F48FB1
    style B7 fill:#FCE4EC,stroke:#F48FB1
```

---

## Part 4: Flowchart — BOFU Decision Journey

```mermaid
graph LR
    LEAD["Lead ที่พร้อมซื้อ<br/>(ผ่าน TOFU + MOFU)"]

    LEAD --> |"ลองใช้ก่อน"| TRIAL["Free Trial<br/>ทดลอง 7-30 วัน"]
    LEAD --> |"ดูสาธิต"| DEMO["Product Demo<br/>เน้น Benefits"]
    LEAD --> |"ดูรีวิว"| TESTI["Testimonial<br/>Video + Text"]
    LEAD --> |"เปรียบเทียบ"| COMPARE["Comparison Chart<br/>เรา vs คู่แข่ง"]

    TRIAL --> CONFIDENT["มั่นใจ!"]
    DEMO --> CONFIDENT
    TESTI --> CONFIDENT
    COMPARE --> CONFIDENT

    CONFIDENT --> |"ดูราคา"| PRICING["Pricing Page<br/>+ Recommended Plan"]
    CONFIDENT --> |"ยังกังวล"| GUARANTEE["Guarantee<br/>คืนเงิน 30 วัน"]

    GUARANTEE --> PRICING
    PRICING --> |"กดปุ่มซื้อ!"| CUSTOMER["ลูกค้าจริง!"]

    style LEAD fill:#FFF8E1,stroke:#FFD54F
    style TRIAL fill:#FCE4EC,stroke:#F48FB1
    style DEMO fill:#FCE4EC,stroke:#F48FB1
    style TESTI fill:#FCE4EC,stroke:#F48FB1
    style COMPARE fill:#FCE4EC,stroke:#F48FB1
    style CONFIDENT fill:#FF69B4,stroke:#FF1493,color:#fff
    style GUARANTEE fill:#E8F5E9,stroke:#66BB6A
    style PRICING fill:#E8F5E9,stroke:#66BB6A
    style CUSTOMER fill:#32CD32,stroke:#228B22,color:#fff
```

---

## Part 5: Flowchart — BOFU KPI & Measurement

```mermaid
graph TB
    subgraph "BOFU KPI Dashboard"
        CR["Conversion Rate<br/>Lead → ลูกค้า<br/>เป้า: 20-30%"]
        REV["Revenue<br/>รายได้จริง<br/>AOV + CLV"]
        CAC_NODE["CAC<br/>ต้นทุนได้ลูกค้า 1 คน<br/>ค่าใช้จ่าย / ลูกค้าใหม่"]
    end

    subgraph "สูตรความยั่งยืน"
        RATIO["CLV / CAC Ratio"]
        GOOD["≥ 3:1<br/>ธุรกิจยั่งยืน"]
        BAD["< 3:1<br/>ต้นทุนสูงเกินไป!<br/>ปรับปรุง Funnel"]
    end

    CR --> RATIO
    REV --> RATIO
    CAC_NODE --> RATIO

    RATIO --> GOOD
    RATIO --> BAD

    style CR fill:#E3F2FD,stroke:#64B5F6
    style REV fill:#E8F5E9,stroke:#66BB6A
    style CAC_NODE fill:#FFF3E0,stroke:#FFB74D
    style RATIO fill:#FF69B4,stroke:#FF1493,color:#fff
    style GOOD fill:#32CD32,stroke:#228B22,color:#fff
    style BAD fill:#F44336,stroke:#D32F2F,color:#fff
```

---

## Part 6: Comparison Diagram — TOFU vs MOFU vs BOFU

```mermaid
graph TB
    subgraph "TOFU — Top of Funnel"
        TE["เป้าหมาย: Awareness"]
        TT["Blog, Social<br/>Video, Infographic"]
        TK["KPI: Traffic<br/>Reach, Views"]
    end

    subgraph "MOFU — Middle of Funnel"
        ME["เป้าหมาย: Trust"]
        MT["Case Study, Webinar<br/>E-book, Email Seq"]
        MK["KPI: Leads<br/>Subscribers, Open Rate"]
    end

    subgraph "BOFU — Bottom of Funnel"
        BE["เป้าหมาย: Conversion"]
        BT["Free Trial, Demo<br/>Testimonial, Guarantee<br/>Comparison, Pricing"]
        BK["KPI: Conv. Rate<br/>Revenue, CAC"]
    end

    TE --- ME
    ME --- BE
    TT --- MT
    MT --- BT
    TK --- MK
    MK --- BK

    style TE fill:#E3F2FD,stroke:#64B5F6
    style TT fill:#E3F2FD,stroke:#64B5F6
    style TK fill:#E3F2FD,stroke:#64B5F6
    style ME fill:#FFF8E1,stroke:#FFD54F
    style MT fill:#FFF8E1,stroke:#FFD54F
    style MK fill:#FFF8E1,stroke:#FFD54F
    style BE fill:#FCE4EC,stroke:#F48FB1
    style BT fill:#FCE4EC,stroke:#F48FB1
    style BK fill:#FCE4EC,stroke:#F48FB1
```

---

## Part 7: Summary Box

```
+==============================================================+
|                      สรุป BOFU                                |
|            Bottom of Funnel — ปิดการขาย                       |
+==============================================================+
|                                                              |
|   เครื่องมือ BOFU 7 ตัวหลัก                                   |
|   +----------------------+------------------------------+    |
|   | Free Trial           | ทดลองฟรี Conversion 15-25%  |    |
|   | Product Demo         | เน้น Benefits, Personalized  |    |
|   | Testimonial          | 92% อ่านรีวิวก่อนซื้อ        |    |
|   | Comparison Chart     | เปรียบเทียบยุติธรรม          |    |
|   | Case Study เชิงลึก   | ROI + Timeline + ขั้นตอน     |    |
|   | Guarantee/Warranty   | คืนเงิน 30 วัน +21% ยอดขาย  |    |
|   | Pricing Page         | Recommended + FAQ + CTA     |    |
|   +----------------------+------------------------------+    |
|                                                              |
|   BOFU KPI                                                   |
|   +----------------------+------------------------------+    |
|   | Conversion Rate      | Lead → ลูกค้า 20-30%         |    |
|   | Revenue              | AOV + CLV                    |    |
|   | CAC                  | ต้นทุนได้ลูกค้า 1 คน          |    |
|   +----------------------+------------------------------+    |
|                                                              |
|   สูตรสำคัญ: CLV/CAC Ratio ≥ 3:1                             |
|   (ต่ำกว่า 3 เท่า = ต้นทุนสูงเกินไป ต้องปรับปรุง funnel)     |
|                                                              |
|   Full Funnel:                                               |
|   TOFU (รู้จัก) → MOFU (เชื่อมั่น) → BOFU (ซื้อ!)            |
|                                                              |
|   3 หลักการสำคัญ:                                             |
|   1. ขจัดข้อกังวลสุดท้าย → ทำให้มั่นใจ 100%                  |
|   2. วัดผลด้วย Conversion Rate + Revenue + CAC               |
|   3. ทั้ง 3 ชั้นต้องสมดุล ขาดชั้นใด Funnel รั่ว!              |
|                                                              |
+==============================================================+
```

---

## สรุปโครงสร้าง Mind Map

| กิ่งหลัก | จำนวนกิ่งย่อย | ประเด็นสำคัญ |
|---------|-------------|-------------|
| BOFU คืออะไร | 4 | Conversion, 20-30%, ขจัดข้อกังวลสุดท้าย |
| เครื่องมือ 7 ตัว | 7 | Trial, Demo, Testimonial, Comparison, Case Study, Guarantee, Pricing |
| BOFU KPI | 3 | Conversion Rate, Revenue, CAC |
| สูตรสำคัญ | 3 | CAC, CLV, CLV/CAC Ratio ≥ 3:1 |
| ความต่างจาก TOFU & MOFU | 3 | Awareness → Trust → Conversion |
| เทคนิคปิดการขาย | 3 | ลดความเสี่ยง, Social Proof, ตัดสินใจง่าย |
| หลักการสำคัญ | 3 | Leads คุณภาพ, มั่นใจ 100%, 3 ชั้นสมดุล |

**จำนวน nodes ทั้งหมด:** 38 nodes

---

> **หมายเหตุ:** Mermaid mindmap สามารถ render ได้ใน GitHub, Notion (embed), VS Code (Mermaid Preview extension)
> Flowchart แบบทางเลือกใช้ได้ในกรณีที่ platform ไม่รองรับ mindmap syntax

---

> ทบทวนต่อ: **CMKTG-006** — เจาะลึก Blog Marketing
> Series: SWP3 Ch28 Content Marketing Mastery
> PinkCastle Academy © 2026
