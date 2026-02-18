# สร้างบทความ ด้วย Content Builder ตอนที่ 2 — CMKTG-015 Mind Map
> Format: Mind Map (Text + Mermaid + Flowcharts)
> Source: SWP3 Ch28 Content Marketing Mastery ตอนที่ 15
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 0:26:27

---

## Part 1: Text Mind Map

```
Content Builder ตอน 2 — Advanced Techniques (CMKTG-015)
├── 1. Custom CSS/Styling
│   ├── เปลี่ยนสี Heading ตรง Brand
│   ├── เพิ่ม Border / Shadow
│   ├── สร้าง Callout Box
│   ├── ปรับ Font ให้เข้า Brand Identity
│   └── ข้อควรระวัง: Test Responsive + Media Query
├── 2. Embed Code (YouTube/Podcast)
│   ├── YouTube iframe (Responsive 16:9)
│   ├── Spotify / Apple Podcasts Player
│   ├── Google Maps / Social Posts
│   ├── ไม่เกิน 2-3 Embed ต่อบทความ
│   └── ใช้ Lazy Loading ทุก Embed
├── 3. Content Upgrade (Lead Magnet ในบทความ)
│   ├── PDF Checklist / Template / Worksheet
│   ├── เจาะจงแต่ละบทความ
│   ├── Conversion สูงกว่า Lead Magnet ทั่วไป 5-10x
│   ├── Opt-in Form ฝังในบทความ
│   └── วางหลัง Section ที่น่าสนใจที่สุด
├── 4. Related Posts Widget
│   ├── Manual — เลือกเอง (แม่นยำที่สุด)
│   ├── Auto — ดึงจาก Category/Tag
│   ├── Hybrid — ผสมทั้งสองแบบ
│   └── ลด Bounce Rate + เพิ่ม Time on Site
├── 5. Social Share Buttons
│   ├── 5 แพลตฟอร์ม
│   │   ├── Facebook
│   │   ├── LINE
│   │   ├── Twitter/X
│   │   ├── LinkedIn
│   │   └── Copy Link
│   ├── 2 ตำแหน่ง: ใต้ Title + ก่อน Related Posts
│   └── ตั้ง Open Graph Tags (og:title, og:description, og:image)
├── 6. Comment Section
│   ├── Disqus / Native Comment
│   ├── สร้าง Community
│   ├── เพิ่มเนื้อหา ดี SEO
│   └── ตั้ง Moderation ป้องกัน Spam
├── 7. Blog Analytics (GA4 Integration)
│   ├── 5 ตัวเลขที่ต้องดู
│   │   ├── Page Views
│   │   ├── Average Engagement Time
│   │   ├── Bounce Rate
│   │   ├── Scroll Depth
│   │   └── Conversion Rate
│   └── วิธีเชื่อม
│       ├── สร้าง GA4 Property
│       ├── ติดตั้งผ่าน GTM
│       ├── ตั้ง Custom Events
│       └── สร้าง Dashboard (GA4/Looker Studio)
├── 8. Image Compression
│   ├── WebP (เล็กกว่า PNG/JPEG 30-50%)
│   ├── เครื่องมือ: TinyPNG / Squoosh / ShortPixel
│   ├── ขนาด: 1200px (Full-width) / 800px (In-content)
│   └── Srcset ให้ Browser เลือกขนาด
├── 9. Lazy Loading
│   ├── โหลดรูป/Embed เมื่อ Scroll มาถึง
│   ├── loading="lazy" ในแท็ก <img>
│   ├── ใช้ Plugin CMS อัตโนมัติ
│   └── Page Speed เพิ่ม 20-40 คะแนน
├── 10. Content Calendar Integration
│   ├── Publish สม่ำเสมอ 1-2 บทความ/สัปดาห์
│   ├── Batch Process: เขียนหลายบทความในวันเดียว
│   ├── Schedule Publish ตามวันที่กำหนด
│   └── เครื่องมือ: Notion / Trello / Pink Castle
└── 11. Repurpose Blog เป็น Social Media Content
    ├── 7 รูปแบบ
    │   ├── Carousel Post (IG/FB)
    │   ├── Quote Card (IG/FB/X)
    │   ├── Thread (X)
    │   ├── Podcast Episode (Spotify/Apple)
    │   ├── Short Video (Reels/TikTok)
    │   ├── Infographic (Pinterest/LinkedIn)
    │   └── Newsletter (Email)
    ├── หลักการ: สร้างครั้งเดียว แจกจ่ายหลายที่
    └── 1 บทความ = 10-15 ชิ้นคอนเทนต์
```

---

## Part 2: Mermaid Mind Map

```mermaid
mindmap
  root((Content Builder<br/>ตอน 2))
    Custom CSS/Styling
      สี Heading ตรง Brand
      Border Shadow
      Callout Box
      Test Responsive
    Embed Code
      YouTube iframe
      Spotify Podcast
      ไม่เกิน 2-3 ต่อบทความ
      Lazy Loading
    Content Upgrade
      Lead Magnet เจาะจง
      Conversion 5-10x
      PDF Checklist Template
      Opt-in Form
    Engagement Elements
      Related Posts
      Social Share 5 แพลตฟอร์ม
      Comment Section
      Open Graph Tags
    Blog Analytics GA4
      Page Views
      Engagement Time
      Bounce Rate
      Scroll Depth
      Conversion Rate
    Performance
      Image Compression WebP
      Lazy Loading
      Page Speed +20-40
      53% ออกถ้าเกิน 3 วินาที
    Content Calendar
      1-2 บทความ ต่อสัปดาห์
      Batch Process
      Schedule Publish
    Repurpose 7 แบบ
      Carousel Post
      Quote Card
      Thread
      Video Podcast
      Infographic Newsletter
```

---

## Part 3: Flowchart — กระบวนการสร้างบทความขั้นสูง

```mermaid
flowchart TD
    A[เขียนบทความด้วย Content Builder] --> B[เพิ่ม Custom CSS/Styling]
    B --> C[ฝัง Embed Code]
    C --> C1{Embed เกิน 3?}
    C1 -->|ใช่| C2[ลดจำนวน Embed]
    C2 --> C1
    C1 -->|ไม่| D[สร้าง Content Upgrade]

    D --> E[ใส่ Opt-in Form<br/>หลัง Section สำคัญ]
    E --> F[เพิ่ม Related Posts Widget]
    F --> G[ใส่ Social Share Buttons<br/>2 จุด + ตั้ง OG Tags]
    G --> H[เปิด Comment Section<br/>+ ตั้ง Moderation]

    H --> I[Optimize Performance]
    I --> I1[Compress รูป WebP<br/>ไม่เกิน 200 KB]
    I --> I2[เพิ่ม Lazy Loading<br/>ทุกรูป + Embed]
    I1 --> J[ตรวจ Page Speed]
    I2 --> J

    J --> K{Score 85+?}
    K -->|ใช่| L[Schedule ใน Content Calendar]
    K -->|ไม่| I
    L --> M[Publish บทความ]
    M --> N[วัดผลด้วย GA4]
    M --> O[Repurpose เป็น 7 รูปแบบ]
```

---

## Part 4: Flowchart — Content Upgrade vs Lead Magnet

```mermaid
flowchart LR
    A[ผู้อ่านเข้าบทความ] --> B{มี Content Upgrade?}

    B -->|ไม่มี| C[Lead Magnet ทั่วไป]
    C --> C1["eBook ฟรี ใช้ทุกหน้า"]
    C1 --> C2["Conversion: 0.5-2%"]

    B -->|มี| D[Content Upgrade]
    D --> D1["SEO Checklist PDF<br/>เจาะจงบทความ SEO"]
    D1 --> D2["Conversion: 3-8%"]

    C2 --> E{เปรียบเทียบ}
    D2 --> E
    E --> F["Content Upgrade ชนะ 5-10x"]

    F --> G[วิธีสร้าง]
    G --> G1[PDF Checklist]
    G --> G2[Template]
    G --> G3[Worksheet]
    G --> G4[Cheat Sheet]
```

---

## Part 5: Flowchart — Performance Optimization Pipeline

```mermaid
flowchart TD
    A[รูปภาพต้นฉบับ] --> B{รูปแบบไฟล์?}
    B -->|PNG/JPEG| C[แปลงเป็น WebP<br/>เล็กลง 30-50%]
    B -->|WebP แล้ว| D[ตรวจขนาด]
    C --> D

    D --> E{ขนาดเกิน 200 KB?}
    E -->|ใช่| F[Compress ด้วย<br/>TinyPNG / Squoosh]
    F --> D
    E -->|ไม่| G[ตรวจ Dimensions]

    G --> H{Full-width?}
    H -->|ใช่| I[ไม่เกิน 1200px กว้าง]
    H -->|In-content| J[ไม่เกิน 800px กว้าง]

    I --> K[เพิ่ม Srcset]
    J --> K
    K --> L["เพิ่ม loading=lazy"]
    L --> M[อัปโหลดขึ้น Content Builder]

    M --> N[ตรวจ Page Speed Score]
    N --> O{Score 85+?}
    O -->|ใช่| P[พร้อม Publish]
    O -->|ไม่| Q[หา Bottleneck อื่น<br/>Embed / Script / Font]
    Q --> N
```

---

## Part 6: Comparison — ก่อน vs หลังใช้ Advanced Techniques

| ด้าน | ก่อนใช้ Advanced Techniques | หลังใช้ Advanced Techniques |
|------|---------------------------|---------------------------|
| **Styling** | ใช้ Style พื้นฐานเหมือนทุกคน | Custom CSS ตรง Brand โดดเด่น |
| **Media** | แค่ข้อความ + รูปภาพ | Embed YouTube/Podcast + Interactive |
| **Lead Generation** | ไม่มี หรือ Lead Magnet ทั่วไป (Conv 0.5%) | Content Upgrade เจาะจง (Conv 3-8%) |
| **Engagement** | ไม่มี Related Posts/Comment | Related Posts + Comment + Social Share |
| **Analytics** | ไม่รู้ว่าบทความไหนดี | GA4 วัดผล 5 ตัวเลข Real-time |
| **Page Speed** | Score 50-60/100 โหลดช้า | Score 85-95/100 WebP + Lazy Loading |
| **Image Size** | 500 KB - 5 MB ต่อรูป | ไม่เกิน 200 KB (WebP) |
| **Publishing** | Publish เมื่อนึกได้ ไม่สม่ำเสมอ | Content Calendar 1-2 บทความ/สัปดาห์ |
| **Content Output** | 1 บทความ = 1 ชิ้น | 1 บทความ = 10-15 ชิ้น (Repurpose) |
| **Social Shares** | 2-5 ต่อบทความ | 20-50 ต่อบทความ (OG Tags + Share Buttons) |
| **Email Signups** | 0.5% | 3-8% (Content Upgrade) |
| **Bounce Rate** | 65-70% | 35-45% |

---

## Part 7: Summary — สรุปภาพรวม

```
Content Builder ตอน 2 — สรุป 5 ประเด็นหลัก

1. Content Upgrade เป็น Game Changer
   → Lead Magnet เจาะจงแต่ละบทความ
   → Conversion สูงกว่า Lead Magnet ทั่วไป 5-10 เท่า
   → สร้าง PDF/Checklist/Template วางหลัง Section สำคัญ

2. Performance = ปัจจัยชี้เป็นชี้ตาย
   → โหลดเกิน 3 วินาที เสียผู้อ่าน 53%
   → Image Compression: WebP เล็กกว่า 30-50%
   → Lazy Loading: Page Speed เพิ่ม 20-40 คะแนน

3. GA4 Analytics คือตาที่สามของ Content Creator
   → 5 ตัวเลข: Page Views, Engagement Time, Bounce Rate,
     Scroll Depth, Conversion Rate
   → ติดตั้งผ่าน GTM + Custom Events

4. Engagement Elements ทำงานร่วมกัน
   → Related Posts ลด Bounce Rate
   → Social Share + OG Tags เพิ่มการแชร์
   → Comment Section สร้าง Community

5. Repurpose = สร้างครั้งเดียว แจกจ่ายหลายที่
   → 1 บทความ = 10-15 ชิ้นคอนเทนต์
   → 7 รูปแบบ: Carousel, Quote Card, Thread,
     Podcast, Video, Infographic, Newsletter
   → ประหยัดเวลามหาศาล

จบ Ch28 Content Marketing Mastery — ทั้งหมด 15 ตอน
```

---
*7 parts: Text Mind Map + Mermaid Mind Map + 3 Flowcharts + Comparison Table + Summary*

---

> จบ Ch28 Content Marketing Mastery — ทั้งหมด 15 ตอน
> Series: SWP3 Ch28 Content Marketing Mastery
> PinkCastle Academy © 2026
