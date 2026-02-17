# Slides: วิธีปรับแต่ง Performance — WEB2-006
> **Format:** Slide Outline (12 Slides)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 6
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## Slide 1: หน้าปก (Title Slide)

- **วิธีปรับแต่ง Performance**
- SWP3 บทที่ 11: สร้างเว็บไซต์ Part 2 — ตอนที่ 6
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## Slide 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- เข้าใจว่าทำไมความเร็วเว็บไซต์ถึงสำคัญต่อ SEO และ UX
- รู้จักเทคนิค Browser Caching และ GZIP Compression
- เรียนรู้วิธี Optimize รูปภาพและ Lazy Loading
- ทำ Minification และ Database Optimization
- ใช้เครื่องมือทดสอบความเร็ว PageSpeed Insights และ GTmetrix

---

## Slide 3: ทำไมความเร็วถึงสำคัญ?

- **SEO:** Google ใช้ Core Web Vitals จัดอันดับ
- **User Experience:** 53% ออกจากเว็บถ้าโหลดเกิน 3 วินาที
- **Conversion:** ช้า 1 วินาที = Conversion ลด 7%
- **Mobile:** 60%+ ของ traffic มาจากมือถือ — ต้องเร็ว
- **เป้าหมาย:** โหลดภายใน 3 วินาที (ดีมาก: ต่ำกว่า 2 วินาที)

---

## Slide 4: Browser Caching — โหลดครั้งเดียว ใช้ได้หลายรอบ

- เก็บไฟล์ CSS, JavaScript, รูปภาพ ไว้ในเบราว์เซอร์ผู้ใช้
- ครั้งที่ 2 ไม่ต้องโหลดใหม่ — เร็วขึ้น 40-60%
- ตั้ง Expiry Time ให้เหมาะสม (เช่น 30 วันสำหรับรูปภาพ)
- ปลั๊กอิน: WP Rocket, W3 Total Cache, WP Super Cache (ฟรี)
- ตั้งค่าผ่าน .htaccess ก็ได้ถ้าชำนาญ

---

## Slide 5: GZIP Compression — ซิปไฟล์ก่อนส่ง

- บีบอัดไฟล์ก่อนส่งจาก server → เบราว์เซอร์ decompress
- ลดขนาดไฟล์ได้ **60-80%** ไม่ส่งผลต่อคุณภาพ
- เหมือนการซิปไฟล์ก่อนส่งอีเมล
- ตั้งค่าผ่าน .htaccess หรือปลั๊กอิน cache
- ตรวจสอบที่: checkgzipcompression.com

---

## Slide 6: Image Optimization — ลดขนาดรูป ลดเวลาโหลด

- รูปภาพ = **50-80%** ของขนาดหน้าเว็บทั้งหมด
- **วิธีที่ 1:** ลดขนาดไฟล์ก่อนอัปโหลด (TinyPNG, ShortPixel)
- **วิธีที่ 2:** ใช้รูปแบบที่เหมาะสม (JPEG / PNG / WebP)
- **วิธีที่ 3:** กำหนดขนาดรูปให้ตรงกับตำแหน่งแสดง
- WebP เล็กกว่า JPEG 25-34% — คุณภาพเทียบเท่า

---

## Slide 7: Lazy Loading — โหลดเมื่อเลื่อนมาถึง

- โหลดรูปภาพ/วิดีโอเฉพาะตอนที่ผู้ใช้เลื่อนมาถึงจุดนั้น
- หน้าแรกเปิดเร็วขึ้นมาก — โหลดแค่ส่วนที่เห็นก่อน
- WordPress 5.5+ มี Lazy Loading ในตัวสำหรับรูปภาพ
- วิดีโอ embed อาจต้องใช้ปลั๊กอินเสริม
- เหมาะมากสำหรับหน้าที่มีรูปภาพเยอะ

---

## Slide 8: Minification — ลดขนาดโค้ด

- เอาช่องว่าง, comment, line break ออกจาก CSS/JavaScript
- ลดขนาดไฟล์ **10-30%** โดยทำงานเหมือนเดิม
- ปลั๊กอิน: **Autoptimize** (ฟรี), **WP Rocket** (มีค่าใช้จ่าย)
- สำคัญ: ทดสอบหลังเปิดใช้ว่าเว็บไม่พัง
- สามารถ Combine ไฟล์หลายตัวรวมกันเพื่อลด HTTP requests

---

## Slide 9: Database Optimization — ทำความสะอาดฐานข้อมูล

- WordPress สะสมข้อมูลที่ไม่จำเป็นเมื่อเวลาผ่านไป
- **Post Revisions** — ฉบับร่างเก่าๆ ของบทความ
- **Spam Comments** — คอมเมนต์ spam ที่ยังไม่ลบ
- **Transient Data** — ข้อมูลชั่วคราวที่หมดอายุ
- ปลั๊กอิน: **WP-Optimize** ทำความสะอาดเดือนละ 1-2 ครั้ง

---

## Slide 10: CDN — ส่งไฟล์จากจุดที่ใกล้ที่สุด

- CDN = Content Delivery Network
- กระจาย server ไว้ทั่วโลก (Edge Servers)
- ผู้ใช้จากไทย → รับไฟล์จาก server ในเอเชีย (ไม่ใช่อเมริกา)
- **Cloudflare** — CDN ฟรี + DDoS Protection + SSL
- ตั้งค่าง่าย: แค่เปลี่ยน Nameserver ของโดเมน

---

## Slide 11: เครื่องมือทดสอบ (Speed Testing Tools)

| เครื่องมือ | จุดเด่น | ค่าใช้จ่าย |
|-----------|---------|:---:|
| Google PageSpeed Insights | คะแนน 0-100 + คำแนะนำจาก Google | ฟรี |
| GTmetrix | Waterfall chart + ประวัติการทดสอบ | ฟรี (พื้นฐาน) |
| Pingdom | ทดสอบจากหลาย location | ฟรี (พื้นฐาน) |

- ทดสอบทั้ง Mobile และ Desktop
- เก็บผลลัพธ์เปรียบเทียบก่อน-หลังปรับแต่ง

---

## Slide 12: สรุปและก้าวต่อไป (Summary & Next Steps)

- ความเร็วสำคัญต่อทั้ง SEO, UX และ Conversion
- 7 เทคนิค: Cache, GZIP, Image, Lazy Load, Minify, DB, CDN
- เป้าหมาย: โหลดภายใน 3 วินาที
- ทดสอบเป็นประจำด้วย PageSpeed Insights + GTmetrix
- **ขั้นตอนถัดไป:** ตั้งค่า Comment และ Social Media Integration

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
