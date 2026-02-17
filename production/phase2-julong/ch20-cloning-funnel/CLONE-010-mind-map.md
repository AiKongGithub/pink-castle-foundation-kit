# แนะนำระบบ Sequence ใน Kartra — CLONE-010 Mind Map
> **Format:** Mind Map (Text-based + Mermaid)
> **Source:** SWP3 Ch20 Cloning Sale Funnel Kartra ตอนที่ 10
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:10:21

---

## Part 1: Text Tree — ภาพรวมหัวข้อ

```
                ระบบ Sequence ใน Kartra
               (Kartra Sequence System)
                          |
        ┌────────┬────────┼────────┬────────┐
        |        |        |        |        |
   [ประเภท]  [องค์ประกอบ] [Welcome] [Funnel] [Metrics]
        |        |        |        |        |
```

### Branch 1: ประเภทของ Sequence
- Time-based
  - ส่งตามวัน/เวลาที่กำหนด
  - Day 0, Day 1, Day 3
  - เข้าใจง่าย เหมาะเริ่มต้น
- Event-based
  - ส่งเมื่อเกิดเหตุการณ์
  - คลิกลิงก์ เข้าชมหน้าเว็บ
  - Personalize ได้มาก
- Conditional
  - ส่งตามเงื่อนไข
  - เปิด/ไม่เปิดอีเมล
  - แยกเส้นทางลูกค้าแต่ละคน

### Branch 2: องค์ประกอบ (Node Types)
- Email Node
  - ตัวอีเมลที่ส่งออกไป
  - หัวข้อ + เนื้อหา + CTA
  - เป็น Node หลักของ Sequence
- Delay Node
  - กำหนดระยะเวลารอ
  - ถี่เกินไป → ลูกค้ารำคาญ
  - ห่างเกินไป → ลูกค้าลืม
- Condition Node
  - แยกเส้นทาง A / B
  - ตามพฤติกรรมจริง
  - ทำ Sequence ฉลาดขึ้น
- Action Node
  - ติด Tag จัดกลุ่ม
  - ย้ายกลุ่มลูกค้า
  - Subscribe เข้า Sequence อื่น

### Branch 3: Welcome Sequence 5 ฉบับ
- Email 1 (Day 0)
  - ต้อนรับ + ส่ง Lead Magnet
  - ส่งทันทีเลย อย่าให้รอ
- Email 2 (Day 1)
  - ให้คุณค่า ความรู้
  - ยังไม่ขาย สร้างเชื่อถือ
- Email 3 (Day 3)
  - เสนอขาย
  - Social Proof + CTA ชัดเจน
- Email 4 (Day 5)
  - Follow-up
  - ตอบ FAQ แก้ข้อโต้แย้ง
- Email 5 (Day 7)
  - Last Chance
  - Urgency ปิดการขาย

### Branch 4: การเชื่อมกับ Funnel
- Capture Page กรอกฟอร์ม
  - Trigger → Subscribe เข้า Sequence
  - อัตโนมัติ 100%
- วิธีสร้างใน Kartra
  - Communications > Sequences
  - New Sequence → Visual Builder
  - ลาก Node มาวาง ต่อกัน
- ทดสอบก่อน Go Live
  - กรอกฟอร์มทดลอง
  - ตรวจ Email 1 ส่งทันทีไหม
  - ตรวจ Delay ทำงานถูกต้องไหม

### Branch 5: Metrics ที่ต้องติดตาม
- Open Rate
  - เกณฑ์ > 20%
  - วัด Subject Line
  - ถ้าต่ำ → ปรับหัวข้อ
- Click Rate
  - เกณฑ์ > 3%
  - วัดเนื้อหา + CTA
  - ถ้าต่ำ → ปรับปุ่ม CTA
- Unsubscribe Rate
  - เกณฑ์ < 2%
  - วัดความถี่/ตรงกลุ่ม
  - ถ้าสูง → ลดความถี่
- Conversion Rate
  - เกณฑ์ > 1-3%
  - Metric สำคัญที่สุด
  - วัดเป้าหมายสุดท้าย

---

## Part 2: Mermaid Mind Map

```mermaid
mindmap
  root((Sequence<br>ใน Kartra))
    ประเภท Sequence
      Time-based
        ส่งตามวัน Day 0 1 3
        เหมาะเริ่มต้น
      Event-based
        ส่งเมื่อเกิดเหตุการณ์
        Personalize สูง
      Conditional
        ส่งตามเงื่อนไข
        แยกเส้นทาง
    องค์ประกอบ 4 Node
      Email Node ส่งอีเมล
      Delay Node เวลารอ
      Condition Node แยกทาง
      Action Node ติด Tag
    Welcome Sequence
      Email 1 Day 0 ต้อนรับ
      Email 2 Day 1 คุณค่า
      Email 3 Day 3 เสนอขาย
      Email 4 Day 5 Follow-up
      Email 5 Day 7 Last Chance
    เชื่อมกับ Funnel
      Capture Page Trigger
      Subscribe อัตโนมัติ
      ทดสอบก่อน Go Live
    4 Metrics
      Open Rate มากกว่า 20%
      Click Rate มากกว่า 3%
      Unsubscribe Rate น้อยกว่า 2%
      Conversion Rate สำคัญที่สุด
```

---

## Part 3: Mermaid Flowchart — Sequence Flow

```mermaid
flowchart TD
    A[ลูกค้ากรอกฟอร์ม Capture Page] --> B[Trigger: Subscribe เข้า Sequence]
    B --> C[Email 1: ต้อนรับ + Lead Magnet]
    C --> D[Delay: 1 วัน]
    D --> E[Email 2: ให้คุณค่า ความรู้]
    E --> F[Delay: 2 วัน]
    F --> G[Email 3: เสนอขาย + Social Proof]
    G --> H[Delay: 2 วัน]
    H --> I[Email 4: Follow-up + FAQ]
    I --> J[Delay: 2 วัน]
    J --> K[Email 5: Last Chance + Urgency]
    K --> L{ลูกค้าซื้อ?}
    L -->|ใช่| M[Action: ติด Tag 'customer']
    L -->|ไม่| N[Action: ติด Tag 'nurture']
    M --> O[Subscribe เข้า Customer Sequence]
    N --> P[Subscribe เข้า Re-engage Sequence]

    style A fill:#FF69B4,color:#fff
    style C fill:#4169E1,color:#fff
    style E fill:#4169E1,color:#fff
    style G fill:#FFD700,color:#000
    style I fill:#4169E1,color:#fff
    style K fill:#FF4500,color:#fff
    style M fill:#32CD32,color:#fff
```

---

## Part 4: Mermaid Flowchart — Condition Node Decision Tree

```mermaid
flowchart TD
    A[ส่ง Email 3: เสนอขาย] --> B{Condition Node}

    B -->|เปิดอีเมล| C{คลิกลิงก์?}
    B -->|ไม่เปิด| D[ส่ง Email ใหม่ หัวข้อดึงดูดกว่า]

    C -->|คลิก| E{ซื้อสินค้า?}
    C -->|ไม่คลิก| F[ส่ง Follow-up เน้น Benefit]

    E -->|ซื้อ| G[Action: Tag 'customer' + Thank You Sequence]
    E -->|ไม่ซื้อ| H[ส่ง Last Chance + Countdown]

    D --> I[Delay 2 วัน]
    I --> J[ส่ง Re-engage Email]

    style A fill:#4169E1,color:#fff
    style B fill:#FFD700,color:#000
    style G fill:#32CD32,color:#fff
    style H fill:#FF4500,color:#fff
```

---

## Part 5: Comparison — 3 ประเภท Sequence

| เกณฑ์ | Time-based | Event-based | Conditional |
|-------|:---:|:---:|:---:|
| วิธี Trigger | ส่งตามวัน/เวลา | ส่งเมื่อเกิดเหตุการณ์ | ส่งตามเงื่อนไข |
| ความยากง่าย | ง่าย | ปานกลาง | ยาก |
| ความยืดหยุ่น | ต่ำ | สูง | สูงมาก |
| Personalize | พื้นฐาน | ตามพฤติกรรม | ตามพฤติกรรม + เงื่อนไข |
| เหมาะกับ | Welcome Sequence | Engaged Leads | A/B Testing ขั้นสูง |
| ตัวอย่าง | Day 0 1 3 5 7 | คลิกลิงก์ → ส่ง Offer | เปิด/ไม่เปิด → แยกทาง |
| แนะนำ | เริ่มจากอันนี้ | เพิ่มทีหลัง | ขั้นสูง |

---

## Part 6: Mermaid Flowchart — สร้าง Sequence ใน Kartra

```mermaid
flowchart TD
    A[เปิด Kartra] --> B[ไปที่ Communications]
    B --> C[เลือก Sequences]
    C --> D[กด New Sequence]
    D --> E[ตั้งชื่อ เช่น Welcome Sequence]
    E --> F[เปิด Visual Builder]

    F --> G[ลาก Email Node → เขียน Email 1]
    G --> H[ลาก Delay Node → ตั้ง 1 วัน]
    H --> I[ลาก Email Node → เขียน Email 2]
    I --> J[ทำซ้ำจนครบ 5 ฉบับ]

    J --> K{ต้องการแยกเส้นทาง?}
    K -->|ใช่| L[ใส่ Condition Node]
    K -->|ไม่| M[Preview + ทดสอบ]
    L --> M

    M --> N{ทดสอบผ่าน?}
    N -->|ใช่| O[Activate Sequence!]
    N -->|ไม่| P[แก้ไข แล้วทดสอบอีกรอบ]
    P --> M

    style A fill:#FF69B4,color:#fff
    style O fill:#32CD32,color:#fff
```

---

## Part 7: สรุป Node Count

**จำนวน Nodes ทั้งหมด: 48 nodes**

| ระดับ | จำนวน |
|-------|-------|
| Center Node | 1 |
| Branch (ระดับ 1) | 5 |
| Sub-branch (ระดับ 2) | 19 |
| Leaf (ระดับ 3) | 23 |
| **รวม** | **48** |

---

> ทบทวนต่อ: **CLONE-011** — ตรวจการบ้าน
> Series: SWP3 Ch20 Cloning Sale Funnel Kartra
> PinkCastle Academy © 2026
