# Slides: วิธีติดตั้ง WP-Rocket Plugin — WEB1-010
> **Format:** Slide Outline (12 Slides)
> **Source:** SWP3 Ch10 สร้างเว็บไซต์ Part 1 ตอนที่ 10
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## Slide 1: หน้าปก (Title Slide)

- **วิธีติดตั้ง WP-Rocket Plugin**
- SWP3 บทที่ 10: วิธีการสร้างเว็บไซต์ Part 1 — ตอนที่ 10
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

─────────────────

## Slide 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- เข้าใจว่าทำไมความเร็วเว็บไซต์ถึงสำคัญต่อ SEO และ User Experience
- รู้จักฟีเจอร์หลัก 6 ด้านของ WP-Rocket
- เปรียบเทียบ WP-Rocket กับ Plugin ฟรี
- สามารถติดตั้งและตั้งค่า WP-Rocket ได้ด้วยตนเอง
- ทดสอบและวัดผลความเร็วเว็บไซต์ได้

─────────────────

## Slide 3: ทำไมความเร็วเว็บไซต์ถึงสำคัญ

- เว็บโหลดเกิน **3 วินาที** = เสียผู้เยี่ยมชมกว่า **50%**
- **Google** ใช้ความเร็วเป็นปัจจัยจัดอันดับ (Ranking Factor)
- เว็บเร็ว = **User Experience ดีขึ้น** = อยู่ในเว็บนานขึ้น
- เว็บเร็ว = **Conversion Rate สูงขึ้น** = ขายได้มากขึ้น
- สรุป: ความเร็วส่งผลทั้ง **SEO + UX + ยอดขาย**

─────────────────

## Slide 4: WP-Rocket คืออะไร

- **Premium Caching Plugin** สำหรับ WordPress
- ติดตั้งง่าย — ทำงานทันทีหลังเปิดใช้งาน
- รองรับ **ทุก Hosting Provider**
- ครอบคลุมการ Optimize ทุกด้านในตัวเดียว
- ลิขสิทธิ์: ซื้อจาก **wp-rocket.me**

─────────────────

## Slide 5: ฟีเจอร์ที่ 1-3 — Caching & Compression

- **Page Caching** — สร้างสำเนาหน้าเว็บไว้ล่วงหน้า
  - ผู้เยี่ยมชมโหลดจากสำเนา ไม่ต้องประมวลผลใหม่ทุกครั้ง
- **Browser Caching** — เก็บข้อมูลในเบราว์เซอร์ของผู้ใช้
  - การเข้าชมซ้ำโหลดเร็วขึ้นมาก
- **GZIP Compression** — บีบอัดไฟล์ HTML/CSS/JS
  - ลดขนาดไฟล์ได้ 60-70%

─────────────────

## Slide 6: ฟีเจอร์ที่ 4-6 — Loading & Optimization

- **Lazy Loading** — โหลดรูปภาพเมื่อเลื่อนถึงเท่านั้น
  - ลดเวลาโหลดหน้าแรกอย่างมาก
- **Minify CSS/JS** — ตัดช่องว่าง/comments ออกจากไฟล์
  - ข้อควรระวัง: ทดสอบหลังเปิดใช้ทุกครั้ง
- **Database Optimization** — ล้างข้อมูลขยะในฐานข้อมูล
  - Post Revisions, Spam Comments, Transients

─────────────────

## Slide 7: เปรียบเทียบ WP-Rocket vs Plugin ฟรี

| เกณฑ์ | WP-Rocket | W3 Total Cache | LiteSpeed Cache |
|-------|:---------:|:--------------:|:---------------:|
| ราคา | Premium | ฟรี | ฟรี |
| ใช้งานง่าย | ง่ายมาก | ซับซ้อน | ปานกลาง |
| รองรับทุก Hosting | ใช่ | ใช่ | LiteSpeed เท่านั้น |
| DB Optimization | มี | ไม่มี | บางส่วน |
| Lazy Loading | มี | ไม่มี | มี |

─────────────────

## Slide 8: ขั้นตอนการติดตั้ง (Step-by-Step)

1. **ซื้อ License** จาก wp-rocket.me
2. **ดาวน์โหลด** ไฟล์ Plugin (.zip)
3. เข้า WordPress Admin → **Plugins → Add New → Upload Plugin**
4. เลือกไฟล์ zip → กด **Install Now**
5. กด **Activate**
6. Page Caching เปิดใช้งาน **อัตโนมัติ** ทันที

─────────────────

## Slide 9: การตั้งค่าแนะนำ

- ไปที่ **Settings → WP Rocket**
- เปิด **Lazy Loading** สำหรับรูปภาพ
- เปิด **Minify CSS** (ทดสอบหลังเปิด)
- เปิด **Minify JavaScript** (ทดสอบหลังเปิด)
- ตั้งเวลา **Database Cleanup** อย่างน้อยเดือนละครั้ง
- Exclude ไฟล์ที่มีปัญหาจาก Minify ถ้าพบ Layout แตก

─────────────────

## Slide 10: ทดสอบความเร็วก่อนและหลัง

- **ก่อนติดตั้ง:** ทดสอบด้วย Google PageSpeed Insights / GTmetrix
- **จดคะแนน:** Performance Score, Loading Time, Page Size
- **หลังติดตั้ง:** ทดสอบอีกครั้งด้วยเครื่องมือเดียวกัน
- **เปรียบเทียบ:** ดูความแตกต่างของคะแนนและเวลาโหลด
- ผลลัพธ์ทั่วไป: เว็บ 5-6 วินาที → ลดเหลือ **1-2 วินาที**

─────────────────

## Slide 11: สิ่งที่ต้องทำเพิ่มเติม (Beyond WP-Rocket)

- **ปรับขนาดรูปภาพ** ก่อนอัปโหลด (ใช้ TinyPNG หรือ ShortPixel)
- **เลือก Hosting คุณภาพ** ที่มี Server ใกล้กลุ่มเป้าหมาย
- **ลดจำนวน Plugin** ให้น้อยที่สุดเท่าที่จำเป็น
- **เลือก Theme ที่เบา** และเขียนโค้ดดี
- การ Optimize ต้องทำ **แบบองค์รวม** ไม่ใช่แค่ติดตั้ง Plugin

─────────────────

## Slide 12: สรุปและก้าวต่อไป (Summary & Next Steps)

- ความเร็วเว็บไซต์ส่งผลต่อ **SEO + UX + ยอดขาย**
- WP-Rocket มี 6 ฟีเจอร์หลัก: Caching, Compression, Lazy Loading, Minify, DB Optimization
- ติดตั้งง่าย ใช้งานง่าย ให้ผลลัพธ์ทันที
- **Action Item:** ทดสอบความเร็วเว็บของคุณวันนี้ด้วย PageSpeed Insights
- ตอนหน้า: วิธีปรับแต่ง WordPress Admin Panel

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
