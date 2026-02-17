# วิธีปรับแต่ง Pop up form — CLONE-008
> **Format:** Mind Map (Text-based)
> **Source:** SWP3 Ch20 Cloning Sale Funnel Kartra ตอนที่ 8
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:14:26

---

## Part 1: Text Tree

```
                  วิธีปรับแต่ง Pop up form
                 (Pop-up Form Customization)
                            |
        ┌───────────┬───────┼───────┬───────────┐
        |           |       |       |           |
  [ประเภท Pop-up] [องค์ประกอบ] [Timing] [Design] [Automation]
        |           |       |       |           |
```

### Branch 1: ประเภท Pop-up (Types)
- Exit Intent
  - เมาส์เลื่อนไปปุ่มปิด
  - Last-chance Offer
  - Desktop only (ไม่ทำงานบนมือถือ)
- Time Delay
  - แสดงหลังผ่านไปตามเวลาที่ตั้ง
  - แนะนำ 5-15 วินาที
  - ใช้ได้ทุกอุปกรณ์
- Scroll Trigger
  - แสดงเมื่อเลื่อนถึงจุดที่กำหนด
  - แนะนำ 50-70% ของหน้า
  - เหมาะกับผู้อ่านลึก
- Click Trigger
  - แสดงเมื่อคลิกปุ่ม/ลิงก์
  - Conversion Rate สูงสุด
  - ผู้เข้าชมสนใจจริง

### Branch 2: องค์ประกอบที่ดี (Good Elements)
- Headline
  - ชัดเจน บอกประโยชน์ทันที
  - ตัวอย่าง: "รับ E-book ฟรี 50 เทคนิค"
- Offer
  - คุ้มค่า แลกกับข้อมูลที่ขอ
  - E-book / คูปอง / เนื้อหาพิเศษ
- ฟิลด์
  - น้อยที่สุด (Name + Email)
  - ทุกฟิลด์ที่เพิ่ม ลด CR 10-15%
- ปุ่ม CTA
  - สีโดดเด่น ตัดกับพื้นหลัง
  - ข้อความกระตุ้น: "รับเลยฟรี!"
- ปุ่มปิด
  - มองเห็นชัดเจน [X]
  - อย่าซ่อน (ลูกค้าหงุดหงิด)

### Branch 3: Timing & Trigger
- Time Delay
  - 5-15 วินาที
- Scroll Trigger
  - 50-70% ของหน้า
- Frequency Setting
  - Once per session (แนะนำ)
  - Once per visitor
  - ป้องกันเด้งซ้ำรบกวน

### Branch 4: Design
- ขนาด
  - 60-70% ของหน้าจอ
  - ไม่ใหญ่เกินจนบังทั้งหน้า
- ตำแหน่ง
  - กลางหน้าจอ
  - มุมล่างขวา
  - Slide-in จากด้านข้าง
- Animation
  - Fade-in (จางเข้า)
  - Slide-up (เลื่อนขึ้น)
  - นุ่มนวลกว่าเด้งทันที
- Overlay
  - สีดำ 50% โปร่งแสง
  - ช่วยโฟกัสที่ Pop-up

### Branch 5: Automation (หลัง Submit)
- เพิ่มเข้า Email List
  - กำหนดลิสต์ที่ต้องการ
- ส่ง Email Sequence
  - Welcome Email ทันที
  - Follow-up ตามลำดับ
- ติด Tag
  - แบ่งกลุ่มลูกค้า
  - เช่น "Lead จาก Funnel A"
- Redirect
  - ไปหน้า Thank You Page
  - ยืนยันว่ากรอกสำเร็จ

### Branch 6: Testing
- ทดสอบ 4 จุด
  - Timing ถูกต้อง
  - Form Submit ได้จริง
  - Redirect ถูกหน้า
  - ไม่รบกวนมากเกิน
- A/B Test
  - เปลี่ยน Headline
  - เปลี่ยนเวลาแสดง
  - เปลี่ยนสี CTA

---

## Part 2: Mermaid Mind Map

```mermaid
mindmap
  root((วิธีปรับแต่ง Pop up form<br>Pop-up Customization))
    ประเภท Pop-up
      Exit Intent
        Desktop only
        Last-chance Offer
      Time Delay
        5-15 วินาที
        ทุกอุปกรณ์
      Scroll Trigger
        50-70% ของหน้า
        ผู้อ่านลึก
      Click Trigger
        CR สูงสุด
        ผู้สนใจจริง
    องค์ประกอบที่ดี
      Headline ชัดเจน
      Offer คุ้มค่า
      ฟิลด์น้อย Name+Email
      CTA โดดเด่น
      ปุ่มปิดชัดเจน
    Timing & Design
      Frequency Once per session
      ขนาด 60-70%
      Fade-in Animation
      Overlay โปร่งแสง
    Automation
      Email List
      Email Sequence
      Tag แบ่งกลุ่ม
      Redirect Thank You
    Testing
      ทดสอบ 4 จุด
      A/B Test
```

---

## Part 3: Pop-up Workflow Flowchart

```mermaid
flowchart TD
    A[ผู้เข้าชมเปิดหน้า Funnel] --> B{Trigger Condition?}
    B -->|Exit Intent| C[เมาส์เลื่อนไปปุ่มปิด]
    B -->|Time Delay| D[ผ่านไป 5-15 วินาที]
    B -->|Scroll| E[เลื่อน 50-70% ของหน้า]
    B -->|Click| F[คลิกปุ่ม CTA]
    C --> G[แสดง Pop-up Form]
    D --> G
    E --> G
    F --> G
    G --> H{ผู้เข้าชมตัดสินใจ}
    H -->|กรอกฟอร์ม| I[Submit Form]
    H -->|ปิด Pop-up| J[กลับไปหน้าเว็บ]
    I --> K[เพิ่มเข้า Email List]
    K --> L[ส่ง Email Sequence]
    L --> M[ติด Tag]
    M --> N[Redirect → Thank You Page]
```

---

## Part 4: Pop-up Type Comparison

```mermaid
flowchart LR
    subgraph Desktop
        A[Exit Intent<br>CR: สูงมาก<br>รบกวน: ต่ำ]
    end
    subgraph ทุกอุปกรณ์
        B[Time Delay<br>CR: สูง<br>รบกวน: กลาง]
        C[Scroll Trigger<br>CR: กลาง-สูง<br>รบกวน: ต่ำ]
        D[Click Trigger<br>CR: สูงมาก<br>รบกวน: ต่ำมาก]
    end
```

| เกณฑ์ | Exit Intent | Time Delay | Scroll Trigger | Click Trigger |
|-------|:---:|:---:|:---:|:---:|
| Conversion Rate | สูงมาก | สูง | กลาง-สูง | สูงมาก |
| ความรบกวน | ต่ำ | กลาง | ต่ำ | ต่ำมาก |
| ใช้กับมือถือ | ไม่ได้ | ได้ | ได้ | ได้ |
| ตั้งค่า | ง่าย | ง่าย | ปานกลาง | ง่าย |
| เหมาะกับ | Last-chance | ผู้สนใจ | ผู้อ่านลึก | CTA ชัดเจน |

---

## Part 5: Automation Flow

```mermaid
flowchart TD
    A[ลูกค้ากรอก Pop-up Form] --> B[Kartra Form Settings]
    B --> C{Automation Rules}
    C --> D[เพิ่มเข้า Email List]
    C --> E[ส่ง Welcome Email]
    C --> F[ติด Tag แบ่งกลุ่ม]
    C --> G[Redirect → Thank You Page]
    D --> H[Email Sequence ต่อเนื่อง]
    H --> I[Email #1: ส่ง Lead Magnet]
    I --> J[Email #2: เนื้อหามีคุณค่า]
    J --> K[Email #3: Offer พิเศษ]
    F --> L[Segment ลูกค้า]
    L --> M[ส่งเนื้อหาตรงกลุ่ม]
```

---

## Part 6: Testing Checklist Flowchart

```mermaid
flowchart TD
    A[เริ่มทดสอบ Pop-up] --> B{Timing ถูกต้อง?}
    B -->|ใช่| C{Form Submit ได้?}
    B -->|ไม่| B1[ปรับ Timing Setting]
    B1 --> B
    C -->|ใช่| D{Redirect ถูกหน้า?}
    C -->|ไม่| C1[ตรวจ Form Settings + Email List]
    C1 --> C
    D -->|ใช่| E{ไม่รบกวนเกินไป?}
    D -->|ไม่| D1[แก้ไข Redirect URL]
    D1 --> D
    E -->|ใช่| F[พร้อม Publish!]
    E -->|ไม่| E1[ปรับ Frequency / Design / Timing]
    E1 --> E
    F --> G[ทำ A/B Test เพิ่มเติม]
```

---

## Part 7: Summary

**จำนวน Nodes ทั้งหมด: 42 nodes**

| ระดับ | จำนวน |
|-------|-------|
| Center Node | 1 |
| Branch (ระดับ 1) | 6 |
| Sub-branch (ระดับ 2) | 20 |
| Leaf (ระดับ 3) | 15 |
| **รวม** | **42** |

**หลักการสำคัญ:**
- Pop-up ที่ดี = ให้คุณค่า ไม่ใช่รบกวน
- เลือกประเภทให้ตรงพฤติกรรม ฟิลด์น้อย CTA ชัด
- ตั้ง Frequency + Timing ให้เหมาะสม
- เชื่อม Automation ครบวงจร
- ทดสอบทุกอย่างก่อน Publish

---

> ทบทวนต่อ: **CLONE-009** — ปรับแต่งหน้า Thank You Page
> Series: SWP3 Ch20 Cloning Sale Funnel Kartra
> PinkCastle Academy © 2026
