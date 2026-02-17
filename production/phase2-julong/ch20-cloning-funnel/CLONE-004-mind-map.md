# วิธีปรับแต่งแคมเปญ Kartra — CLONE-004 Mind Map
> Format: Mind Map (7 Parts)
> Source: SWP3 Ch20 Cloning Sale Funnel Kartra ตอนที่ 4
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 0:16:30

---

## Part 1: Text-based Mind Map

```
วิธีปรับแต่งแคมเปญ Kartra
│
├── ทำไมต้องปรับแต่ง?
│   ├── Template ยังเป็นของคนอื่น
│   ├── ใช้ตรงๆ ทำลายความน่าเชื่อถือ
│   ├── Conversion Rate จะต่ำ
│   └── ต้องปรับ 6 หมวดก่อนเปิดใช้
│
├── 1. Branding
│   ├── Logo → ทุกหน้า (PNG/SVG)
│   ├── Color Scheme → HEX Codes สม่ำเสมอ
│   ├── Font → เดียวกันทุกหน้า
│   └── Tip: ใช้ Global Styles เปลี่ยนทีเดียว
│
├── 2. Copy
│   ├── Headlines → ตรง Pain Points
│   ├── Body Text → น้ำเสียงของเรา
│   └── CTAs → เชิงประโยชน์ (CTR สูงกว่า)
│       ├── ❌ Click Here / Submit / ส่ง
│       └── ✅ รับสิทธิ์เลย / เริ่มฟรีวันนี้
│
├── 3. Images/Videos
│   ├── หลัก: ของจริง ชนะ Stock Photo
│   ├── รูปสินค้าจริง (ถ่ายมือถือก็ได้)
│   ├── Testimonial จากลูกค้าจริง
│   └── วิดีโอแนะนำตัวสั้นๆ
│
├── 4. Email Sequences
│   ├── ชื่อผู้ส่ง → เปลี่ยนเป็นชื่อเรา
│   ├── Subject Line → น่าเปิดอ่าน
│   ├── เนื้อหา → ตรง Value Ladder
│   └── Timing
│       ├── ทันที → Welcome
│       ├── Day 1 → ให้คุณค่า
│       ├── Day 3 → เสนอขาย
│       ├── Day 5 → Follow-up
│       └── Day 7 → Last Chance
│
├── 5. Forms
│   ├── ฟิลด์ → ขอแค่ชื่อ+อีเมล (Lead Magnet)
│   ├── Confirmation → เปลี่ยนข้อความ
│   ├── Redirect URL → ชี้หน้าถูกต้อง
│   └── หลัก: ขอน้อย = Conversion สูง
│
├── 6. Automations
│   ├── Trigger → เงื่อนไขเริ่มทำงาน
│   ├── Action → สิ่งที่เกิดขึ้น
│   ├── Tags → ป้ายกำกับแยกกลุ่ม
│   └── ⚠️ Tags ผิด = ระบบทั้งหมดสับสน
│
└── Testing End-to-end
    ├── กรอกฟอร์ม
    ├── ตรวจอีเมล
    ├── คลิกลิงก์ทุกจุด
    ├── ตรวจ Automations + Tags
    ├── เช็ค Desktop
    └── เช็ค Mobile (70% ใช้ Mobile)
```

---

## Part 2: Mermaid Mind Map

```mermaid
mindmap
  root((ปรับแต่งแคมเปญ Kartra))
    Branding
      Logo ทุกหน้า
      Color Scheme
      Font สม่ำเสมอ
      Global Styles
    Copy
      Headlines ตรง Pain Points
      Body Text น้ำเสียงเรา
      CTA เชิงประโยชน์
    Media
      รูปสินค้าจริง
      Testimonial จริง
      วิดีโอแนะนำตัว
    Email
      ชื่อผู้ส่ง
      Subject Line
      เนื้อหา Value Ladder
      Timing 5 ฉบับ
    Forms
      ฟิลด์น้อย Conversion สูง
      Confirmation
      Redirect URL
    Automations
      Trigger
      Action
      Tags แยกกลุ่ม
    Testing
      End-to-end
      Desktop + Mobile
```

---

## Part 3: Flowchart — ขั้นตอนการปรับแต่ง

```mermaid
flowchart TD
    A[Import Campaign สำเร็จ] --> B[เตรียม Brand Kit]
    B --> B1[Logo PNG/SVG]
    B --> B2[HEX Color Codes]
    B --> B3[Font ที่จะใช้]

    B1 & B2 & B3 --> C[ปรับ Branding<br/>Global Styles]
    C --> D[เขียน Copy ใหม่]
    D --> D1[Headlines ตรง Pain Points]
    D --> D2[Body Text น้ำเสียงเรา]
    D --> D3[CTA เชิงประโยชน์]

    D1 & D2 & D3 --> E[เปลี่ยน Media]
    E --> E1[รูปสินค้าจริง]
    E --> E2[Testimonial]
    E --> E3[วิดีโอแนะนำตัว]

    E1 & E2 & E3 --> F[ปรับ Email Sequences]
    F --> G[ปรับ Forms + Automations]
    G --> H{Testing End-to-end}
    H -->|ผ่าน| I[เปิดใช้ Funnel]
    H -->|ไม่ผ่าน| J[แก้ไขจุดที่มีปัญหา]
    J --> H
```

---

## Part 4: Flowchart — CTA เปรียบเทียบ

```mermaid
flowchart LR
    subgraph BAD["❌ CTA ไม่ดี"]
        B1["Click Here"]
        B2["Submit"]
        B3["ส่ง"]
    end

    subgraph GOOD["✅ CTA ที่ดี"]
        G1["รับสิทธิ์เลย"]
        G2["เริ่มฟรีวันนี้"]
        G3["ดาวน์โหลดคู่มือ"]
    end

    BAD -->|"CTR ต่ำ<br/>ไม่รู้จะได้อะไร"| R1[Conversion ต่ำ]
    GOOD -->|"CTR สูง<br/>เห็นประโยชน์ชัด"| R2[Conversion สูง]
```

---

## Part 5: Flowchart — Automation 3 องค์ประกอบ

```mermaid
flowchart LR
    T[Trigger<br/>เงื่อนไขเริ่ม] -->|"เช่น คนกรอกฟอร์ม"| A[Action<br/>สิ่งที่เกิดขึ้น]
    A -->|"เช่น ส่ง Email"| TG[Tags<br/>ป้ายกำกับ]
    TG -->|"เช่น ติด lead"| R{Tags ถูกต้อง?}
    R -->|ใช่| OK[ลูกค้าได้ Email ถูกชุด]
    R -->|ไม่ใช่| ERR[ลูกค้าจัดกลุ่มผิด<br/>ได้ Email ผิดชุด]

    ERR --> FIX[วาดแผนผัง Tag System<br/>แก้ไข Tags ให้ตรง]
    FIX --> T
```

---

## Part 6: Comparison — Build vs Import+Customize

```mermaid
flowchart TD
    subgraph BUILD["สร้างใหม่ทั้งหมด"]
        direction TB
        BL1["ออกแบบ Layout"] --> BL2["เขียน Copy"]
        BL2 --> BL3["สร้าง Email"]
        BL3 --> BL4["ตั้ง Automations"]
        BL4 --> BL5["ใส่ Media"]
        BL5 --> BL6["Testing"]
        BL6 --> BLR["⏰ 2-4 สัปดาห์"]
    end

    subgraph IMPORT["Import + Customize"]
        direction TB
        IM1["Import Template"] --> IM2["ปรับ 6 หมวด"]
        IM2 --> IM3["Testing"]
        IM3 --> IMR["⏰ 1-2 วัน"]
    end
```

---

## Part 7: สรุป — สูตรสำเร็จ

```
╔══════════════════════════════════════════════════╗
║                                                  ║
║  สูตร: โครงสร้างประหยัดเวลา                        ║
║        แต่เนื้อหาต้องเป็นของเรา                     ║
║                                                  ║
╠══════════════════════════════════════════════════╣
║                                                  ║
║  6 หมวด + Testing = Campaign พร้อมใช้            ║
║                                                  ║
║  Branding → Copy → Media → Email                 ║
║  → Forms → Automations → Testing                 ║
║                                                  ║
║  5 กฎเหล็ก:                                      ║
║  1. ปรับ 6 หมวดให้ครบก่อนเปิด Funnel              ║
║  2. ของจริง ดีกว่า Stock Photo เสมอ               ║
║  3. CTA บอกประโยชน์ ไม่ใช่คำสั่ง                   ║
║  4. วาดแผนผัง Tag System ก่อนปรับ Automations     ║
║  5. Testing End-to-end ห้ามข้าม Desktop+Mobile   ║
║                                                  ║
╚══════════════════════════════════════════════════╝
```

---

> ทบทวนต่อ: **CLONE-005** — ปรับแต่งหน้า Capture Page
> Series: SWP3 Ch20 Cloning Sale Funnel Kartra
> PinkCastle Academy © 2026
