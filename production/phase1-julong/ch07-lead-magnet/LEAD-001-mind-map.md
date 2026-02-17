# Lead Magnet คืออะไร — LEAD-001
> **Format:** Mind Map (Mermaid)
> **Source:** SWP3 Ch7 Lead Magnet ตอนที่ 1
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## Mind Map หลัก: Lead Magnet คืออะไร

```mermaid
mindmap
  root((Lead Magnet<br/>คืออะไร))
    นิยาม
      ของฟรีที่มีคุณค่า
      แลกกับข้อมูลติดต่อ
        อีเมล
        เบอร์โทร
        ชื่อ-นามสกุล
      แม่เหล็กดึงดูดลูกค้า
    ความสำคัญ
      สร้าง Email List
        ทรัพย์สินของเราเอง
        ไม่ขึ้นกับแพลตฟอร์ม
        The money is in the list
      สร้างความไว้วางใจ
      สร้างความน่าเชื่อถือ
      กรองกลุ่มเป้าหมาย
    จิตวิทยา
      Reciprocity
        ให้ก่อน รู้สึกอยากตอบแทน
      Perceived Value
        มูลค่าที่รับรู้สูง
      Urgency
        จำกัดเวลา จำนวน
        FOMO
      Authority
        ของฟรีดี ของจริงดีกว่า
    คุณสมบัติ 5 ข้อ
      แก้ปัญหาเฉพาะเจาะจง
      Quick Win ผลลัพธ์เร็ว
      ค่าที่รับรู้สูง
      ง่ายต่อการบริโภค
      เชื่อมโยงสินค้าหลัก
    Sales Funnel
      Lead Magnet ปากกรวย
      Email Sequence
      Trip Wire
      Core Product
      Upsell
    ตัวอย่างตลาดไทย
      PDF คู่มือฟรี
      คอร์สมินิฟรี
      Webinar สด
      Template แจกฟรี
```

---

## แผนภาพ: Give First, Sell Later

```mermaid
flowchart LR
    A[คนแปลกหน้า] -->|เห็น Lead Magnet| B[สนใจ]
    B -->|ให้ข้อมูลติดต่อ| C[กลายเป็น Lead]
    C -->|ได้รับของฟรีดี| D[ไว้วางใจ]
    D -->|Email Sequence| E[สร้างความสัมพันธ์]
    E -->|เสนอ Trip Wire| F[ทดลองซื้อ]
    F -->|พอใจ| G[ซื้อสินค้าหลัก]

    style A fill:#ff9999,stroke:#cc0000
    style C fill:#ffcc99,stroke:#cc6600
    style D fill:#ffff99,stroke:#cccc00
    style G fill:#99ff99,stroke:#00cc00
```

---

## แผนภาพ: คุณสมบัติ 5 ข้อ

```mermaid
flowchart TD
    center[Lead Magnet ที่ดี]
    center --> A[1. แก้ปัญหาเฉพาะเจาะจง]
    center --> B[2. Quick Win ผลลัพธ์เร็ว]
    center --> C[3. ค่าที่รับรู้สูง]
    center --> D[4. ง่ายต่อการบริโภค]
    center --> E[5. เชื่อมโยงสินค้าหลัก]

    A --> A1[เจาะปัญหาเดียว ไม่กว้างเกินไป]
    B --> B1[ใช้แล้วเห็นผลทันที]
    C --> C1[ดีไซน์สวย เนื้อหาดี]
    D --> D1[อ่านจบใน 10-15 นาที]
    E --> E1[เป็นประตูสู่สินค้าหลัก]

    style center fill:#ff69b4,stroke:#cc0066,color:#fff
    style A fill:#ffe6f0,stroke:#ff69b4
    style B fill:#ffe6f0,stroke:#ff69b4
    style C fill:#ffe6f0,stroke:#ff69b4
    style D fill:#ffe6f0,stroke:#ff69b4
    style E fill:#ffe6f0,stroke:#ff69b4
```

---

## แผนภาพ: Lead Magnet ใน Sales Funnel

```mermaid
flowchart TD
    LM["Lead Magnet<br/>(ปากกรวย — กว้างที่สุด)"]
    ES["Email Sequence<br/>(สร้างความสัมพันธ์)"]
    TW["Trip Wire<br/>(สินค้าราคาถูก)"]
    CP["Core Product<br/>(สินค้าหลัก)"]
    US["Upsell / Cross-sell<br/>(ขายเพิ่ม)"]

    LM --> ES --> TW --> CP --> US

    style LM fill:#ff69b4,stroke:#cc0066,color:#fff
    style ES fill:#ff99cc,stroke:#cc6699
    style TW fill:#ffccdd,stroke:#cc9999
    style CP fill:#ffddee,stroke:#ccaaaa
    style US fill:#ffeeee,stroke:#ccbbbb
```

---

## แผนภาพ: จิตวิทยา 4 หลักการ

```mermaid
flowchart LR
    subgraph จิตวิทยา Lead Magnet
        R[Reciprocity<br/>การตอบแทน]
        PV[Perceived Value<br/>ค่าที่รับรู้]
        U[Urgency<br/>ความเร่งด่วน]
        AU[Authority<br/>ความน่าเชื่อถือ]
    end

    R --> R1[ให้ฟรี → รู้สึกอยากตอบแทน]
    PV --> PV1[มูลค่าสูง → คุ้มค่าแลก]
    U --> U1[จำกัดเวลา → ตัดสินใจเร็ว]
    AU --> AU1[ของฟรีดี → ของจริงดีกว่า]

    style R fill:#ff6b6b,stroke:#c92a2a,color:#fff
    style PV fill:#ffd43b,stroke:#fab005
    style U fill:#69db7c,stroke:#2b8a3e
    style AU fill:#74c0fc,stroke:#1c7ed6
```

---

> **จำนวนแผนภาพ:** 5 (Mind Map หลัก + 4 แผนภาพเสริม)
> **เครื่องมือ:** Mermaid.js — render ได้ใน GitHub, Notion, VS Code
