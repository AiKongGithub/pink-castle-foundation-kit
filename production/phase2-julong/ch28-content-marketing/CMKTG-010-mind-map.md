# ตรวจการบ้าน (ครั้งที่ 1) — CMKTG-010 Mind Map
> **Format:** Mind Map (Mermaid)
> **Source:** SWP3 Ch28 Content Marketing Mastery ตอนที่ 10
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:32:52

---

## Part 1: Text-based Mind Map

```
                     ตรวจการบ้าน Content Marketing (ครั้งที่ 1)
                              Checkpoint CMKTG-010
                                      |
          ┌──────────────┬────────────┼────────────┬──────────────┐
          |              |            |            |              |
   [1.ทบทวน Funnel]  [2.ตรวจ Blog] [3.ตรวจ      [4.Common     [5.เกณฑ์
    TOFU/MOFU/BOFU    โครงสร้าง     Headline      Mistakes      คะแนน]
          |          + Visual       + Hook]        7 ข้อ]       5 ด้าน
    ┌─────┼─────┐        |            |            |           100 คะแนน
    |     |     |   ┌────┼────┐  ┌────┼────┐  ┌───┼───┐
  TOFU  MOFU  BOFU H2/H3 Visual Headline Hook เขียนเพื่อ  ไม่
  60%   30%   10%  ย่อหน้า Alt   4จุด   4เทค ตัวเอง   Research
                   Inverted Text  อ่อน  นิค  ไม่มีCTA  ก๊อป
                   Pyramid TOC                ไม่Proof  ไม่มี
                                              read     Links
```

---

## Part 2: Mermaid Mind Map

```mermaid
mindmap
  root((ตรวจการบ้าน<br/>Content Marketing<br/>ครั้งที่ 1))
    1. ทบทวน Content Funnel
      TOFU 60% Awareness
        ดึงคนใหม่เข้ามา
        Content กว้าง Search Volume สูง
        ตัวอย่าง: ...คืออะไร, 5 วิธี...
      MOFU 30% Consideration
        สร้างความเชื่อมั่น
        How-to Case Study เปรียบเทียบ
      BOFU 10% Conversion
        ปิดการขาย
        รีวิว Social Proof
      ข้อผิดพลาด
        เขียน BOFU ก่อนไม่มี TOFU
        ปน TOFU + BOFU ในบทความเดียว
    2. ตรวจโครงสร้าง Blog
      ปัญหาที่พบ
        ไม่มี H2/H3 เขียนก้อนยาว
        ย่อหน้า 10-15 บรรทัด
        ไม่มี Table of Contents
        ไม่ใช้ Inverted Pyramid
        ไม่มี Visual เลย
      Visual ที่พบ
        มีแค่รูปปก 1 รูป
        Stock Photo ไม่เกี่ยวเนื้อหา
        ไม่มี Alt Text
    3. ตรวจ Headline + Hook
      Headline 4 จุดอ่อน
        ยาวเกิน 70 ตัวอักษร
        ไม่มี Keyword
        ไม่มี Power Words
        ไม่สื่อ Benefit
      Hook 4 เทคนิคที่ดี
        เปิดด้วยคำถาม
        เปิดด้วยสถิติ
        เปิดด้วยเรื่องเล่า
        เปิดด้วยข้อเท็จจริงขัดสามัญสำนึก
      Hook ที่ล้มเหลว
        เปิดด้วยคำนิยาม
      Bridge
        เชื่อม Hook เข้าเนื้อหาหลัก
    4. 7 Common Mistakes
      เขียนเพื่อตัวเอง
      ไม่ทำ Keyword Research
      ไม่มี CTA หรือ CTA ไม่เกี่ยว
      ยาวไม่มีโครงสร้าง
      ไม่ Proofread
      ก๊อปเนื้อหา/AI ไม่ปรับ
      ไม่มี Internal Links
    5. เกณฑ์คะแนน 5 ด้าน
      Funnel Alignment 20 คะแนน
      Headline + Hook 20 คะแนน
      โครงสร้าง + Visual 20 คะแนน
      เนื้อหาและคุณค่า 20 คะแนน
      CTA + SEO Basics 20 คะแนน
```

---

## Part 3: Flowchart — กระบวนการตรวจการบ้านบทความ

```mermaid
flowchart TD
    A[เริ่มตรวจบทความ] --> B{Funnel Stage ชัดเจนไหม?}
    B -->|ไม่ชัด| C[ระบุว่าเป็น TOFU/MOFU/BOFU<br/>ปรับเนื้อหาให้ Match Stage]
    B -->|ชัดเจน| D{Headline ผ่านเกณฑ์ไหม?}
    C --> D
    D -->|ไม่ผ่าน| E[ตรวจ 4 จุด:<br/>สั้น ≤70 ตัวอักษร?<br/>มี Keyword?<br/>มี Power Words?<br/>สื่อ Benefit?]
    D -->|ผ่าน| F{Hook ดึงดูดไหม?}
    E --> F
    F -->|ไม่ดึงดูด| G[เปลี่ยนเป็น 1 ใน 4 เทคนิค:<br/>คำถาม/สถิติ/เรื่องเล่า/<br/>ข้อเท็จจริงขัดสามัญสำนึก]
    F -->|ดึงดูด| H{โครงสร้างดีไหม?}
    G --> H
    H -->|ไม่ดี| I[แก้ไข:<br/>เพิ่ม H2/H3<br/>ย่อหน้า ≤3-4 บรรทัด<br/>ใช้ Inverted Pyramid<br/>เพิ่ม TOC + Visual]
    H -->|ดี| J{CTA + SEO ครบไหม?}
    I --> J
    J -->|ไม่ครบ| K[เพิ่ม CTA ที่ Match เนื้อหา<br/>ใส่ Internal Links 2-3 จุด<br/>เพิ่ม Alt Text ทุกรูป]
    J -->|ครบ| L{Proofread แล้วหรือยัง?}
    K --> L
    L -->|ยัง| M[อ่านทบทวน 2 รอบ:<br/>รอบ 1 คำผิด/ลิงก์เสีย<br/>รอบ 2 ความชัดเจนเนื้อหา]
    L -->|แล้ว| N[ให้คะแนน 5 ด้าน 100 คะแนน]
    M --> N
    N --> O{คะแนน ≥70?}
    O -->|ใช่| P[Publish ได้ ✅]
    O -->|ไม่| Q[ปรับปรุงตามจุดที่ได้<br/>คะแนนต่ำ แล้วตรวจใหม่]
    Q --> B
```

---

## Part 4: Flowchart — กระบวนการแก้ไข Headline

```mermaid
flowchart TD
    A[Headline ปัจจุบัน] --> B{ยาวเกิน 70<br/>ตัวอักษร?}
    B -->|ใช่| C[ตัดให้สั้นลง<br/>เก็บเฉพาะใจความสำคัญ]
    B -->|ไม่| D{มี Keyword ที่คน<br/>ค้นหาจริงไหม?}
    C --> D
    D -->|ไม่| E[ทำ Keyword Research<br/>หา Keyword ที่มี<br/>Search Volume จริง]
    D -->|มี| F{มี Power Words<br/>กระตุ้นอารมณ์ไหม?}
    E --> F
    F -->|ไม่| G[เพิ่ม Power Words เช่น<br/>ฟรี เคล็ดลับ วิธีง่ายๆ<br/>ที่คนส่วนใหญ่ไม่รู้]
    F -->|มี| H{สื่อ Benefit<br/>บอกว่าอ่านแล้ว<br/>จะได้อะไร?}
    G --> H
    H -->|ไม่| I[เพิ่ม Benefit เช่น<br/>เริ่มต้นฟรี ทำได้ทันที<br/>ไม่ต้องมีประสบการณ์]
    H -->|มี| J[Headline พร้อม Publish ✅]
    I --> J

    style J fill:#d4edda
```

---

## Part 5: Flowchart — กระบวนการเลือก Hook ที่เหมาะสม

```mermaid
flowchart TD
    A[ต้องการเขียน<br/>Opening Hook] --> B{บทความมีข้อมูล<br/>สถิติน่าสนใจไหม?}
    B -->|ใช่| C[เปิดด้วยสถิติ<br/>เช่น 70% ของบทความ<br/>ไม่มีคนอ่านเกินย่อหน้าแรก]
    B -->|ไม่| D{มีประสบการณ์จริง<br/>เล่าได้ไหม?}
    D -->|ใช่| E[เปิดด้วยเรื่องเล่า<br/>เช่น ผมเคยเขียน Blog 50 บทความ<br/>แต่ไม่มี Traffic สักคน]
    D -->|ไม่| F{มีข้อเท็จจริง<br/>ที่ขัดสามัญสำนึก?}
    F -->|ใช่| G[เปิดด้วยข้อเท็จจริง<br/>เช่น การเขียน Blog<br/>ไม่ต้องเก่งเขียน]
    F -->|ไม่| H[เปิดด้วยคำถาม<br/>เช่น เคยสงสัยไหมว่า<br/>ทำไมบทความไม่มีคนอ่าน?]
    C --> I[เขียน Bridge เชื่อม<br/>Hook → เนื้อหาหลัก]
    E --> I
    G --> I
    H --> I
    I --> J[ทดสอบ: อ่านออกเสียง<br/>รู้สึกตื่นเต้นไหม?]
    J -->|ตื่นเต้น| K[Hook พร้อมใช้ ✅]
    J -->|เฉยๆ| A

    style K fill:#d4edda
```

---

## Part 6: Comparison — เปรียบเทียบ 5 ด้านของเกณฑ์คะแนน

| มิติ | Funnel Alignment | Headline + Hook | โครงสร้าง + Visual | เนื้อหาและคุณค่า | CTA + SEO Basics |
|------|-----------------|----------------|-------------------|-----------------|-----------------|
| **คะแนนเต็ม** | 20 | 20 | 20 | 20 | 20 |
| **สิ่งที่ตรวจ** | ชัดว่า TOFU/MOFU/BOFU เนื้อหา Match | Keyword, Power Words, Benefit, Hook ดึงดูด | H2/H3, ย่อหน้า, Inverted Pyramid, TOC, Visual | ถูกต้อง มีประโยชน์ มีตัวอย่าง | CTA Match เนื้อหา, Internal Links, Alt Text |
| **ปัญหาที่พบบ่อย** | ไม่ระบุ Stage ปน Funnel หลาย Stage | ยาวเกิน, ไม่มี Keyword, เปิดด้วยคำนิยาม | เรียงความ ย่อหน้ายาว ไม่มี Visual | เขียนเพื่อตัวเอง ก๊อปเนื้อหา | ไม่มี CTA, ไม่มี Internal Links |
| **ผลถ้าได้คะแนนต่ำ** | Content ไม่ตรงกลุ่มเป้าหมาย | CTR ต่ำ คนไม่คลิก ไม่อ่านต่อ | Bounce Rate สูง Time on Page ต่ำ | ไม่มีคนกลับมาอ่านซ้ำ | เสียโอกาสทางธุรกิจ SEO อ่อน |
| **วิธีแก้หลัก** | วางแผน Content Calendar ตามสัดส่วน | ใช้ Formula: Power Word + Keyword + Benefit | เปลี่ยนจาก "เรียงความ" เป็น "บทความออนไลน์" | ถาม "ผู้อ่านอยากรู้อะไร?" | สร้าง Lead Magnet ต่อ Content Pillar |
| **เครื่องมือ** | Content Calendar + Funnel Map | Headline Analyzer + Keyword Tool | Checklist ก่อน Publish | Peer Review + Proofread | CTA Template + Link Audit |
| **ระดับยาก** | ปานกลาง | สูง | ปานกลาง | สูง | ปานกลาง-สูง |
| **ทำก่อนอะไร** | วางแผนก่อนเขียน | เขียน 3 แบบแล้วเลือก | วาง Outline ก่อน | Research ก่อน | สร้าง Lead Magnet ก่อน |

---

## Part 7: สรุปภาพรวม

```
╔═══════════════════════════════════════════════════════════╗
║     ตรวจการบ้าน Content Marketing ครั้งที่ 1              ║
║     Checkpoint: 9 ตอนที่เรียนมา → ลงมือทำ → ตรวจ        ║
╠═══════════════════════════════════════════════════════════╣
║                                                           ║
║  1. ทบทวน Content Funnel                                 ║
║  ┌──────────────────────────────────────────┐             ║
║  │ TOFU 60% → MOFU 30% → BOFU 10%         │             ║
║  │ ห้ามปน Stage  |  ห้ามเขียน BOFU ก่อน    │             ║
║  └──────────────────────────────────────────┘             ║
║                                                           ║
║  2. ตรวจโครงสร้าง Blog                                   ║
║  ┌──────────────────────────────────────────┐             ║
║  │ H2/H3 ✓ | ย่อหน้า 3-4 บรรทัด ✓         │             ║
║  │ Inverted Pyramid ✓ | TOC ✓ | Visual ✓   │             ║
║  └──────────────────────────────────────────┘             ║
║                                                           ║
║  3. ตรวจ Headline + Hook                                 ║
║  ┌──────────────────────────────────────────┐             ║
║  │ Headline: สั้น + Keyword + Power + Benefit│             ║
║  │ Hook: คำถาม/สถิติ/เรื่องเล่า/ข้อเท็จจริง│             ║
║  │ + Bridge เชื่อมเข้าเนื้อหาหลัก          │             ║
║  └──────────────────────────────────────────┘             ║
║                                                           ║
║  4. 7 Common Mistakes                                    ║
║  ┌──────────────────────────────────────────┐             ║
║  │ เขียนเพื่อตัวเอง | ไม่ Research          │             ║
║  │ ไม่มี CTA | ยาวไม่มีโครงสร้าง           │             ║
║  │ ไม่ Proofread | ก๊อป | ไม่มี Links       │             ║
║  └──────────────────────────────────────────┘             ║
║                                                           ║
║  5. เกณฑ์คะแนน 100 คะแนน                                ║
║  ┌──────┐ ┌──────┐ ┌──────┐ ┌──────┐ ┌──────┐           ║
║  │Funnel│ │Head- │ │โครง- │ │เนื้อ-│ │CTA + │           ║
║  │ 20   │ │line  │ │สร้าง │ │หาและ │ │SEO   │           ║
║  │      │ │+Hook │ │+Vis- │ │คุณค่า│ │Basic │           ║
║  │      │ │ 20   │ │ual 20│ │ 20   │ │ 20   │           ║
║  └──────┘ └──────┘ └──────┘ └──────┘ └──────┘           ║
║                                                           ║
║  Feedback: เข้าใจทฤษฎีดี → ลงมือทำไม่ครบ                ║
║  แก้ด้วย: Pre-Publish Checklist + อ่านบนมือถือ           ║
║          + ให้คนอื่นอ่าน + เขียนบ่อยๆ                   ║
╚═══════════════════════════════════════════════════════════╝
```

**Key Takeaways:**
- **ทบทวน Funnel** ก่อนเขียนทุกชิ้น — TOFU 60% เป็นฐานสำคัญที่สุด
- **โครงสร้างบทความ** ต้องเป็นแบบ "บทความออนไลน์" ไม่ใช่ "เรียงความ" — H2/H3 + ย่อหน้าสั้น + Visual
- **Headline Formula** = Power Word + Keyword + Benefit ไม่เกิน 70 ตัวอักษร
- **Hook ที่ดี** = คำถาม / สถิติ / เรื่องเล่า / ข้อเท็จจริงขัดสามัญสำนึก + Bridge เชื่อมเข้าเนื้อหา
- **7 Common Mistakes** ที่ต้องกำจัด — ใช้ Checklist ตรวจทุกข้อก่อน Publish
- **เกณฑ์คะแนน 5 ด้าน 100 คะแนน** = เครื่องมือประเมินตัวเองที่ใช้ได้จริง

---

*Mind map sections: 7 | Mermaid diagrams: 4 | Level: Beginner-Intermediate*

---

> ทบทวนต่อ: **CMKTG-011** — ปรับแต่ง Template Single Blog Post
> Series: SWP3 Ch28 Content Marketing Mastery
> PinkCastle Academy © 2026
