# สร้างบทความ ด้วย Content Builder ตอนที่ 2 — CMKTG-015 Slides
> Format: Slide Outline (12 Slides)
> Source: SWP3 Ch28 Content Marketing Mastery ตอนที่ 15
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 0:26:27

---

## SLIDE 1: หน้าปก (Title Slide)
```
+==========================================+
|                                          |
|   สร้างบทความ ด้วย Content Builder      |
|   ตอนที่ 2 — Advanced Techniques        |
|                                          |
|   SWP3 Ch28: Content Marketing Mastery   |
|   ตอนที่ 15 (ตอนสุดท้าย)                |
|                                          |
|   PinkCastle Academy                     |
|   วันที่: 18 กุมภาพันธ์ 2569             |
|                                          |
+==========================================+
```

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้ (Learning Objectives)
```
+==========================================+
|         Learning Objectives              |
+==========================================+
```

- Custom CSS/Styling — ปรับแต่งบทความให้ตรง Brand Identity
- Embed Code — ฝัง YouTube/Podcast/Maps ในบทความ
- Content Upgrade — สร้าง Lead Magnet เจาะจงแต่ละบทความ
- Related Posts + Social Share + Comment Section
- Blog Analytics — เชื่อม GA4 วัดผลบทความ
- Performance Optimization — Image Compression + Lazy Loading
- Content Calendar — วางแผน Publish สม่ำเสมอ
- Repurpose Blog — แตก 1 บทความเป็น 10-15 ชิ้นคอนเทนต์

---

## SLIDE 3: Custom CSS/Styling
```
+==========================================+
|   1. Custom CSS/Styling                  |
|   ปรับแต่งบทความให้โดดเด่นกว่าคนอื่น   |
+==========================================+
```

**สิ่งที่ทำได้:**
```
+-------------------------------+
|  [Callout Box]               |
|  สีพื้นหลัง + Border         |
|  เน้นข้อมูลสำคัญ             |
+-------------------------------+

+-------------------------------+
|  Custom Heading              |
|  สี/Font ตรง Brand Identity  |
|  + Shadow/Border-bottom      |
+-------------------------------+
```

- เปลี่ยนสี Heading, เพิ่ม Border/Shadow
- สร้าง Callout Box, ปรับ Font
- ใช้ CSS Framework เช่น Tailwind ช่วยได้
- **ข้อควรระวัง**: ต้อง Test Responsive + ใช้ Media Query

---

## SLIDE 4: Embed Code (YouTube/Podcast)
```
+==========================================+
|   2. Embed Code                          |
|   ฝัง Video/Audio ให้บทความมีชีวิต      |
+==========================================+
```

```
+------------------------------------+
|                                    |
|    [  YouTube Video Player  ]      |
|    Responsive: 16:9 ratio          |
|    padding-bottom: 56.25%          |
|                                    |
+------------------------------------+
|    [Spotify Podcast Player]        |
|    Embed from Spotify/Apple        |
+------------------------------------+
```

**กฎ 3 ข้อ:**
1. ใช้ Responsive Embed (wrap ด้วย Container)
2. ไม่เกิน 2-3 Embed ต่อบทความ
3. ใช้ Lazy Loading ทุก Embed

---

## SLIDE 5: Content Upgrade (Lead Magnet ในบทความ)
```
+==========================================+
|   3. Content Upgrade                     |
|   Conversion สูงกว่า Lead Magnet 5-10x  |
+==========================================+
```

```
Lead Magnet ทั่วไป           Content Upgrade
+----------------+          +-------------------+
| ebook ฟรี      |          | SEO Checklist PDF |
| ใช้ทุกหน้า     |          | เจาะจงบทความ SEO  |
| Conv: 0.5-2%   |          | Conv: 3-8%        |
+----------------+          +-------------------+
      ↓                            ↓
  กว้าง ไม่ตรงใจ            ตรงใจ เกี่ยวข้องทันที
```

**วิธีสร้าง:**
- PDF Checklist / Template / Worksheet
- วาง Opt-in Form หลัง Section ที่น่าสนใจที่สุด
- ข้อความดึงดูด: "ดาวน์โหลด Checklist ฉบับเต็ม — ใส่อีเมล"

---

## SLIDE 6: Related Posts + Social Share + Comment
```
+==========================================+
|   4-6. Engagement Elements               |
|   Related Posts | Share | Comment        |
+==========================================+
```

| Element | ประโยชน์ | ตั้งค่า |
|---------|---------|--------|
| Related Posts | ลด Bounce Rate เพิ่ม Time on Site | Manual/Auto/Hybrid — ท้ายบทความ |
| Social Share | เพิ่มการแชร์ เข้าถึงคนใหม่ | FB/LINE/X/LinkedIn/Copy — 2 จุด (บน+ล่าง) |
| Comment | สร้าง Community ดี SEO | Disqus/Native + Moderation ป้องกัน Spam |

**Open Graph Tags สำคัญ:**
- `og:title` — ชื่อบทความ
- `og:description` — คำอธิบาย
- `og:image` — รูป Preview (1200x630px)
- ทดสอบด้วย Facebook Debugger

---

## SLIDE 7: Blog Analytics — GA4 Integration
```
+==========================================+
|   7. Blog Analytics (GA4)                |
|   ถ้าไม่วัดผล ไม่รู้ว่าอะไรดี          |
+==========================================+
```

**5 ตัวเลขที่ต้องดู:**
```
+-------------------+------------------+
| Page Views        | คนเข้ามาเท่าไร  |
| Engagement Time   | อ่านนานแค่ไหน   |
| Bounce Rate       | อ่านหน้าเดียวออก |
| Scroll Depth      | อ่านถึงตรงไหน   |
| Conversion Rate   | กด CTA กี่ %    |
+-------------------+------------------+
```

**วิธีเชื่อม:**
1. สร้าง GA4 Property
2. ติดตั้ง Tracking ผ่าน GTM
3. ตั้ง Custom Events (CTA Click, Scroll 25/50/75/100%, Form Submit)
4. สร้าง Dashboard ใน GA4 / Looker Studio

---

## SLIDE 8: Performance Optimization — Image Compression
```
+==========================================+
|   8. Image Compression                   |
|   โหลดเกิน 3 วินาที = เสียผู้อ่าน 53%  |
+==========================================+
```

```
  PNG/JPEG (500 KB)          WebP (250 KB)
  +-----------+              +-----------+
  | xxxxxxxxx |  Compress    | xxxxxxxxx |
  | xxxxxxxxx | --------->   | xxxxxxxxx |
  | xxxxxxxxx |  -30-50%     | xxxxxxxxx |
  +-----------+              +-----------+
  โหลดช้า                    โหลดเร็ว คุณภาพเท่าเดิม
```

**4 ขั้นตอน:**
1. ใช้รูปแบบ **WebP** (เล็กกว่า 30-50%)
2. Compress ด้วย TinyPNG / Squoosh / ShortPixel
3. ขนาดไม่เกิน 1200px (Full-width) / 800px (In-content)
4. ใช้ Srcset ให้ Browser เลือกขนาดเหมาะสม

---

## SLIDE 9: Performance Optimization — Lazy Loading
```
+==========================================+
|   9. Lazy Loading                        |
|   Page Speed เพิ่ม 20-40 คะแนน          |
+==========================================+
```

```
การโหลดปกติ:                Lazy Loading:
+---------------------------+---------------------------+
| [รูป 1] โหลดทันที         | [รูป 1] โหลดทันที         |
| [รูป 2] โหลดทันที         | [รูป 2] ยังไม่โหลด        |
| [รูป 3] โหลดทันที         | [รูป 3] ยังไม่โหลด        |
| [รูป 4] โหลดทันที         | [รูป 4] ยังไม่โหลด        |
|                           |                           |
| หน้าโหลดช้า               | หน้าโหลดเร็ว              |
+---------------------------+---------------------------+
                               ↓ Scroll มาถึง
                            [รูป 2] โหลด!
```

**วิธีทำ:** เพิ่ม `loading="lazy"` ใน `<img>` หรือใช้ Plugin CMS

---

## SLIDE 10: Content Calendar Integration
```
+==========================================+
|   10. Content Calendar                   |
|   Publish สม่ำเสมอ = Google ชอบ         |
+==========================================+
```

```
+-----+-----+-----+-----+-----+-----+-----+
| จัน | อัง | พุธ | พฤ  | ศุก | เสา | อา  |
+-----+-----+-----+-----+-----+-----+-----+
|     | POST|     |     | POST|     |     |
|     | #1  |     |     | #2  |     |     |
+-----+-----+-----+-----+-----+-----+-----+
|     | POST|     |     | POST|     |     |
|     | #3  |     |     | #4  |     |     |
+-----+-----+-----+-----+-----+-----+-----+
```

**กฎ:**
- 1-2 บทความ/สัปดาห์ (สม่ำเสมอ)
- Batch Process: เขียนหลายบทความในวันเดียว แล้ว Schedule
- เครื่องมือ: Notion, Trello, Pink Castle Content Planner

---

## SLIDE 11: Repurpose Blog เป็น Social Media Content
```
+==========================================+
|   สร้างครั้งเดียว แจกจ่ายหลายที่        |
|   1 บทความ = 10-15 ชิ้นคอนเทนต์        |
+==========================================+
```

```
              Blog Post (Pillar Content)
                       |
       +-------+-------+-------+-------+
       |       |       |       |       |
   Carousel  Quote   Thread  Video  Infographic
   (IG/FB)   Card   (X/Twitter) (Reels) (Pinterest)
       |       |       |       |       |
       +-------+-------+-------+-------+
                       |
                  Newsletter
                  (Email)
```

| # | รูปแบบ | Platform |
|---|--------|----------|
| 1 | Carousel Post | Instagram, Facebook |
| 2 | Quote Card | IG, FB, X |
| 3 | Thread | Twitter/X |
| 4 | Podcast Episode | Spotify, Apple |
| 5 | Short Video | Reels, TikTok |
| 6 | Infographic | Pinterest, LinkedIn |
| 7 | Newsletter | Email |

---

## SLIDE 12: สรุปและ Next Steps
```
+==========================================+
|   สรุป: Content Builder ตอน 2            |
|   จบ Ch28 Content Marketing Mastery      |
+==========================================+
```

**10 Advanced Techniques ที่เรียนรู้:**
1. Custom CSS/Styling — ปรับแต่ง Brand Identity
2. Embed Code — YouTube/Podcast (ไม่เกิน 2-3)
3. Content Upgrade — Conversion สูง 5-10x
4. Related Posts — ลด Bounce Rate
5. Social Share Buttons — 5 แพลตฟอร์ม + OG Tags
6. Comment Section — สร้าง Community
7. GA4 Analytics — วัดผล 5 ตัวเลข
8. Image Compression — WebP เล็กกว่า 30-50%
9. Lazy Loading — Page Speed +20-40 คะแนน
10. Content Calendar — Publish 1-2 บทความ/สัปดาห์

**จำไว้:**
> 1 บทความ = 10-15 ชิ้นคอนเทนต์
> สร้างครั้งเดียว แจกจ่ายหลายที่

**จบ Ch28 Content Marketing Mastery — ทั้งหมด 15 ตอน**

---
*12 slides | เนื้อหา: Content Builder ตอน 2 — CSS, Embed, Content Upgrade, Analytics, Performance, Repurpose*

---

> จบ Ch28 Content Marketing Mastery — ทั้งหมด 15 ตอน
> Series: SWP3 Ch28 Content Marketing Mastery
> PinkCastle Academy © 2026
