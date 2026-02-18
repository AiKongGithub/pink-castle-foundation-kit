# สร้างบทความ ด้วย Content Builder ตอนที่ 1 — CMKTG-013 Mind Map
> Format: Mind Map (Text + Mermaid + Flowcharts)
> Source: SWP3 Ch28 Content Marketing Mastery ตอนที่ 13
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 0:33:55

---

## Part 1: Text Mind Map

```
Content Builder ตอนที่ 1 (CMKTG-013)
├── 1. เข้าถึง Content Builder
│   ├── Kartra Dashboard → My Content → New Post
│   ├── 2 ส่วนหลัก: Settings + Content Builder
│   ├── Settings: ชื่อ, หมวดหมู่, แท็ก, Featured Image
│   └── Content Builder: พื้นที่สร้างเนื้อหาจริง
├── 2. เลือก Template
│   ├── Clean Minimal (แนะนำสำหรับมือใหม่)
│   ├── With Sidebar
│   ├── Full Width
│   ├── Hero Section
│   └── เคล็ดลับ: เริ่มเรียบง่าย แล้วค่อยเพิ่ม Component
├── 3. Drag & Drop Components
│   ├── Text Component
│   │   ├── Heading H1, H2, H3, H4
│   │   ├── ย่อหน้า (Paragraph)
│   │   ├── Bullet Point / Numbered List
│   │   └── H1 มีแค่ 1 ตัว (Heading Hierarchy)
│   ├── Image Component
│   │   ├── อัปโหลดจากเครื่อง หรือ URL
│   │   └── ใส่ Alt Text ทุกรูป (SEO + Accessibility)
│   ├── Video Component
│   │   ├── Embed YouTube/Vimeo (ประหยัด Storage)
│   │   ├── Upload ตรง (วิดีโอเฉพาะสมาชิก)
│   │   └── เพิ่ม Time on Page
│   ├── Button Component
│   │   ├── ข้อความ Action-Oriented
│   │   ├── สีตัดกับพื้นหลัง
│   │   └── Link: สมัคร/ดาวน์โหลด/บทความอื่น
│   └── Divider Component
│       ├── เส้นคั่นแบ่ง Section
│       └── บทความยาวต้องมี ไม่งั้นอ่านยาก
├── 4. Typography
│   ├── Body Text: 16-18px
│   ├── Line Height: 1.5-1.8 เท่า
│   ├── Font Style สม่ำเสมอ
│   └── กฎทอง: ความสม่ำเสมอตลอดบทความ
├── 5. Internal Links
│   ├── เชื่อมไปยังบทความอื่นในบล็อก
│   ├── ข้อดี 1: ผู้อ่านค้นพบเนื้อหา
│   ├── ข้อดี 2: เพิ่ม Pages per Session
│   ├── ข้อดี 3: กระจาย Link Juice (SEO)
│   ├── Anchor Text ต้องสื่อความหมาย
│   └── แนะนำ 3-5 ลิงก์ต่อบทความ
├── 6. SEO On-page
│   ├── Title
│   │   ├── ไม่เกิน 60 ตัวอักษร
│   │   ├── มี Keyword หลัก
│   │   └── ดึงดูดให้คลิก
│   ├── Meta Description
│   │   ├── 150-160 ตัวอักษร
│   │   ├── มี Keyword + CTA เบาๆ
│   │   └── อธิบายว่าบทความเกี่ยวกับอะไร
│   └── URL Slug
│       ├── สั้น ภาษาอังกฤษ
│       ├── คั่นด้วยขีด (-)
│       ├── มี Keyword หลัก
│       └── ห้ามเปลี่ยนหลัง Publish
└── 7. Preview + Publish
    ├── Preview 3 ขนาดจอ (Desktop, Tablet, Mobile)
    ├── ตรวจ: รูปภาพ, ลิงก์, ปุ่ม, Typography
    ├── อ่านจบทั้งบทความอย่างน้อย 1 รอบ
    └── ตรวจ Checklist ครบ → กด Publish
```

---

## Part 2: Mermaid Mind Map

```mermaid
mindmap
  root((Content Builder<br/>ตอนที่ 1))
    เข้าถึง Builder
      My Content → New Post
      Settings + Builder
    เลือก Template
      Clean Minimal
      With Sidebar
      Full Width
      Hero Section
      มือใหม่เริ่มเรียบง่าย
    Drag & Drop
      Text
        Heading H1 H2 H3
        ย่อหน้า
        Bullet List
      Image
        อัปโหลด หรือ URL
        Alt Text ทุกรูป
      Video
        Embed YouTube
        Upload ตรง
        เพิ่ม Time on Page
      Button
        Action-Oriented
        สีตัดกับพื้นหลัง
      Divider
        เส้นคั่น Section
        บทความยาวต้องมี
    Typography
      Body 16-18px
      Line Height 1.5-1.8
      สม่ำเสมอตลอด
    Internal Links
      3-5 ลิงก์ต่อบทความ
      Anchor Text สื่อความหมาย
      กระจาย Link Juice
    SEO On-page
      Title ไม่เกิน 60 ตัว
      Meta 150-160 ตัว
      URL Slug สั้น มี Keyword
    Preview + Publish
      Desktop Tablet Mobile
      อ่านจบ 1 รอบ
      Checklist ครบ → Publish
```

---

## Part 3: Flowchart — ขั้นตอนสร้างบทความ

```mermaid
flowchart TD
    A[เริ่มต้น: สร้างบทความใหม่] --> B[My Content → New Post]
    B --> C{เลือก Template}
    C -->|มือใหม่| D[Clean Minimal]
    C -->|มี Widget| E[With Sidebar]
    C -->|บทความยาว| F[Full Width]
    D --> G[Content Builder เปิดแล้ว]
    E --> G
    F --> G
    G --> H[ลาก Text Component → เขียนเนื้อหา]
    H --> I[ลาก Image Component → ใส่รูป + Alt Text]
    I --> J[ลาก Video Component → Embed/Upload]
    J --> K[ลาก Button Component → ใส่ CTA]
    K --> L[ลาก Divider Component → แบ่ง Section]
    L --> M[จัดรูปแบบ Typography]
    M --> N[ใส่ Internal Links 3-5 จุด]
    N --> O[ตั้งค่า SEO: Title + Meta + URL Slug]
    O --> P[Preview 3 ขนาดจอ]
    P --> Q{ผ่านทั้ง 3 ขนาด?}
    Q -->|ใช่| R[อ่านจบทั้งบทความ 1 รอบ]
    Q -->|ไม่| P
    R --> S{เนื้อหาพร้อม?}
    S -->|ใช่| T[กด Publish]
    S -->|ไม่| H
    T --> U[บทความเผยแพร่แล้ว]
```

---

## Part 4: Flowchart — เลือกวิธี Embed สื่อ

```mermaid
flowchart TD
    A[ต้องการใส่สื่อในบทความ] --> B{ประเภทสื่อ?}

    B -->|รูปภาพ| C[Image Component]
    C --> C1{แหล่งรูป?}
    C1 -->|ไฟล์ในเครื่อง| C2[Upload]
    C1 -->|รูปจากเว็บ| C3[ใส่ URL]
    C2 --> C4[ใส่ Alt Text]
    C3 --> C4
    C4 --> Z[สื่อพร้อมแสดง]

    B -->|วิดีโอ| D{วิดีโออยู่บน YouTube?}
    D -->|ใช่| D1[Embed YouTube]
    D -->|ไม่| D2{เป็นวิดีโอเฉพาะสมาชิก?}
    D2 -->|ใช่| D3[Upload ตรงเข้า Kartra]
    D2 -->|ไม่| D4[อัปโหลดขึ้น YouTube ก่อน → Embed]
    D1 --> Z
    D3 --> Z
    D4 --> Z

    B -->|ปุ่ม CTA| E[Button Component]
    E --> E1[เขียนข้อความ Action-Oriented]
    E1 --> E2[เลือกสีตัดกับพื้นหลัง]
    E2 --> E3[ใส่ Link ปลายทาง]
    E3 --> Z
```

---

## Part 5: Flowchart — SEO On-page Checklist

```mermaid
flowchart TD
    A[ตั้งค่า SEO On-page] --> B[Title]
    A --> C[Meta Description]
    A --> D[URL Slug]

    B --> B1{มี Keyword หลัก?}
    B1 -->|ใช่| B2{ไม่เกิน 60 ตัวอักษร?}
    B1 -->|ไม่| B3[เพิ่ม Keyword ในชื่อ]
    B3 --> B1
    B2 -->|ใช่| B4{ดึงดูดให้คลิก?}
    B2 -->|ไม่| B5[ตัดให้สั้นลง]
    B5 --> B2
    B4 -->|ใช่| B6[Title พร้อม]
    B4 -->|ไม่| B7[ปรับให้น่าสนใจ]
    B7 --> B4

    C --> C1{มี Keyword?}
    C1 -->|ใช่| C2{150-160 ตัวอักษร?}
    C1 -->|ไม่| C3[เพิ่ม Keyword]
    C3 --> C1
    C2 -->|ใช่| C4{มี CTA เบาๆ?}
    C2 -->|ไม่| C5[ปรับความยาว]
    C5 --> C2
    C4 -->|ใช่| C6[Meta พร้อม]
    C4 -->|ไม่| C7[เพิ่ม CTA ท้ายประโยค]
    C7 --> C4

    D --> D1{สั้นกระชับ?}
    D1 -->|ใช่| D2{ภาษาอังกฤษ + ขีดคั่น?}
    D1 -->|ไม่| D3[ตัดคำที่ไม่จำเป็นออก]
    D3 --> D1
    D2 -->|ใช่| D4{มี Keyword?}
    D2 -->|ไม่| D5[แก้เป็นภาษาอังกฤษ คั่นด้วย -]
    D5 --> D2
    D4 -->|ใช่| D6[URL Slug พร้อม]
    D4 -->|ไม่| D7[เพิ่ม Keyword ใน URL]
    D7 --> D4

    B6 --> E[SEO On-page ครบ 3 จุด]
    C6 --> E
    D6 --> E
    E --> F[พร้อม Preview + Publish]
```

---

## Part 6: Comparison — 5 Components หลัก

| ด้าน | Text | Image | Video | Button | Divider |
|------|------|-------|-------|--------|---------|
| **หน้าที่หลัก** | เขียนเนื้อหาทั้งหมด | รูปภาพประกอบ | วิดีโอประกอบ | ปุ่ม CTA นำทาง | เส้นคั่นแบ่ง Section |
| **ความจำเป็น** | ขาดไม่ได้ | สำคัญมาก | สำคัญ | สำคัญ | จำเป็นสำหรับบทความยาว |
| **ช่วย SEO** | Heading Hierarchy | Alt Text | Time on Page | ไม่โดยตรง | ไม่โดยตรง |
| **ช่วย UX** | อ่านง่าย จัดระเบียบ | ดึงดูดสายตา | เข้าใจเนื้อหาง่าย | นำทาง Action ชัดเจน | แบ่งส่วนอ่านไม่เหนื่อย |
| **ความถี่ใช้** | ทุกบทความ | ทุกบทความ | เมื่อมีวิดีโอ | เมื่อมี CTA | บทความยาว |
| **เคล็ดลับ** | H1 มีแค่ 1 ตัว | Alt Text ทุกรูป | Embed YouTube ถ้ามี | ข้อความ Action-Oriented | ใช้แบ่งระหว่างหัวข้อ |
| **วิธี Drag & Drop** | ลากจาก Panel → วาง → พิมพ์ | ลาก → วาง → อัปโหลด/URL | ลาก → วาง → Embed/Upload | ลาก → วาง → ตั้งค่า | ลาก → วาง → เสร็จ |

---

## Part 7: Summary

### สรุป Content Builder ตอนที่ 1 — 7 ขั้นตอนสร้างบทความ

```
┌──────────────────────────────────────────────────────┐
│        CONTENT BUILDER WORKFLOW                        │
│                                                        │
│  [1] เข้าถึง      → My Content → New Post             │
│  [2] Template     → เลือกแบบเรียบง่ายก่อน              │
│  [3] Components   → Text, Image, Video, Button, Divider│
│  [4] Typography   → 16-18px, Line Height 1.5-1.8      │
│  [5] Links        → Internal Links 3-5 จุด             │
│  [6] SEO          → Title + Meta + URL Slug            │
│  [7] Publish      → Preview 3 จอ → อ่าน 1 รอบ → Publish│
│                                                        │
│  จำง่าย — 5 Components: T-I-V-B-D                      │
│  Text, Image, Video, Button, Divider                   │
│                                                        │
│  เป้าหมาย:                                              │
│  บทความดี + Typography ดี + SEO ดี = คุณภาพครบ         │
└──────────────────────────────────────────────────────┘
```

**ตัวเลขสำคัญ:**
- Components หลัก **5** ตัว: Text, Image, Video, Button, Divider
- Body Text **16-18px** / Line Height **1.5-1.8** เท่า
- Internal Links **3-5** ลิงก์ต่อบทความ
- SEO Title ไม่เกิน **60** ตัวอักษร
- Meta Description **150-160** ตัวอักษร
- Preview **3** ขนาดจอก่อน Publish
- H1 มีแค่ **1** ตัวต่อบทความ

---
*Node count: 62 nodes | 7 main branches | 3 flowcharts | 1 comparison table*

---

> ทบทวนต่อ: **CMKTG-014** — ตรวจการบ้าน (ครั้งที่ 2)
> Series: SWP3 Ch28 Content Marketing Mastery
> PinkCastle Academy © 2026
