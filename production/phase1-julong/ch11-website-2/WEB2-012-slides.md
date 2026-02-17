# Slides: วิธีการตั้งค่า WP-Rocket — WEB2-012
> **Format:** Slide Outline (14 Slides)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 12
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## SLIDE 1: หน้าปก (Title Slide)

- **วิธีการตั้งค่า WP-Rocket**
- SWP3 บทที่ 11: สร้างเว็บไซต์ Part 2 — ตอนที่ 12
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- ตั้งค่า File Optimization (Minify/Combine/Defer)
- ตั้งค่า Media Settings (LazyLoad/WebP)
- ตั้งค่า Preloading และ DNS Prefetch
- ใช้ Advanced Rules (Never Cache URLs)
- ทำ Database Cleanup และ CDN Integration
- ทดสอบก่อน-หลังด้วย GTmetrix

---

## SLIDE 3: ทำไมความเร็วถึงสำคัญ?

- Google ใช้ความเร็วเป็นปัจจัยจัดอันดับ SEO
- **53%** ของผู้ใช้ออกจากเว็บถ้าโหลดนานกว่า 3 วินาที
- เว็บเร็ว 1 วินาที = Conversion เพิ่ม 7%
- WP-Rocket ช่วยเร่งความเร็วได้ **40-60%**
- ตั้งค่าครั้งเดียว ได้ผลถาวร

---

## SLIDE 4: File Optimization — CSS

- **Minify CSS** — ลบช่องว่าง/comment ลดขนาดไฟล์
- **Combine CSS** — รวมหลายไฟล์เป็นไฟล์เดียว
  - ลด HTTP Requests
  - ระวัง: อาจทำให้หน้าตาเพี้ยน
- หลักการ: **เปิดทีละตัว ทดสอบทุกครั้ง**
- ถ้า Combine มีปัญหา ปิดแล้วใช้แค่ Minify

---

## SLIDE 5: File Optimization — JavaScript

- **Minify JS** — ลดขนาดไฟล์ JavaScript
- **Combine JS** — รวมไฟล์เป็นหนึ่ง
- **Defer JS Loading** (สำคัญมาก)
  - ปกติ: Browser หยุดแสดงหน้าเว็บเพื่อรอ JS
  - Defer: HTML โหลดก่อน > JS รันทีหลัง
  - ผลลัพธ์: ผู้ใช้เห็นเนื้อหาเร็วขึ้นมาก

---

## SLIDE 6: Media Settings — LazyLoad

- **LazyLoad คืออะไร?**
  - สื่อโหลดเฉพาะเมื่อเลื่อนลงมาถึง
  - ไม่โหลดทุกอย่างพร้อมกัน
- **เปิดได้สำหรับ:**
  - รูปภาพ (Images)
  - Iframes (YouTube, Maps)
  - วิดีโอ (Videos)
- ผลลัพธ์: เว็บที่มีรูปเยอะเร็วขึ้น **มหาศาล**

---

## SLIDE 7: Media Settings — Image Dimensions & WebP

- **Add Missing Image Dimensions**
  - เพิ่ม width/height ให้รูปที่ไม่มี
  - ลด Layout Shift (CLS) — หน้าเว็บไม่กระตุก
  - CLS = Core Web Vitals ของ Google
- **WebP Compatibility**
  - WebP เล็กกว่า JPEG/PNG 25-30%
  - คุณภาพเท่ากัน ขนาดเล็กกว่า
  - WP-Rocket ส่ง WebP อัตโนมัติตาม browser

---

## SLIDE 8: Preloading

- **Sitemap-based Preloading**
  - Crawl ทุกหน้าตาม Sitemap
  - สร้าง cache ล่วงหน้า
  - ผู้เข้าชมทุกคนได้ cache ทันที
- **DNS Prefetch**
  - Resolve DNS ล่วงหน้าสำหรับ domain ภายนอก
  - ใส่ domain ที่ใช้บ่อย:
    - fonts.googleapis.com
    - CDN domain
    - Analytics domain

---

## SLIDE 9: Advanced Rules

| Rule | ใช้กับ | ตัวอย่าง |
|------|--------|---------|
| Never Cache URLs | หน้าไม่ควร cache | /checkout/, /cart/, /my-account/ |
| Always Purge URLs | Clear cache เมื่ออัปเดต | หน้าแรก, หน้าหมวดหมู่ |
| Cache Query Strings | URL มีพารามิเตอร์ | ?utm_source=..., ?ref=... |

- **สำคัญ:** หน้า Checkout/Cart ห้าม cache เด็ดขาด!

---

## SLIDE 10: Database Optimization

- **ลบข้อมูลที่ไม่จำเป็น:**
  - Post Revisions (ประวัติแก้ไข)
  - Auto Drafts (ร่างอัตโนมัติ)
  - Transients (ข้อมูลชั่วคราว)
  - Spam Comments (ความคิดเห็นสแปม)
- **Optimize Tables** — ลดขนาดฐานข้อมูล
- แนะนำทำ **สัปดาห์ละครั้ง**
- ระวัง: อย่าลบ Revisions ถ้ายังต้องการประวัติการแก้ไข

---

## SLIDE 11: CDN Integration & Heartbeat

- **CDN (Content Delivery Network)**
  - ส่งเนื้อหาจาก server ใกล้ผู้เข้าชมที่สุด
  - ลดเวลาโหลดสำหรับผู้ใช้ต่างประเทศ
  - Cloudflare Add-on สำหรับผู้ใช้ Cloudflare
- **Heartbeat API Control**
  - WordPress ส่ง heartbeat ทุก 15-60 วินาที
  - กินทรัพยากร server มาก
  - ลดความถี่เป็น 120 วินาที หรือปิดในหน้าที่ไม่จำเป็น

---

## SLIDE 12: ทดสอบก่อน-หลังด้วย GTmetrix

| ขั้นตอน | Action |
|---------|--------|
| 1 | ไป gtmetrix.com ทดสอบเว็บก่อนเปิด WP-Rocket |
| 2 | บันทึกคะแนน + Screenshot |
| 3 | เปิด WP-Rocket ตั้งค่าตามลำดับ |
| 4 | ทดสอบอีกครั้ง |
| 5 | เปรียบเทียบผลลัพธ์ |

- คะแนนเพิ่ม: **20-40 คะแนน**
- เวลาโหลดลด: **40-60%**

---

## SLIDE 13: ลำดับการตั้งค่าที่แนะนำ

1. Minify CSS + Minify JS > ทดสอบ
2. Defer JS Loading > ทดสอบ
3. LazyLoad Images/Iframes/Videos > ทดสอบ
4. Add Missing Image Dimensions
5. Sitemap-based Preloading + DNS Prefetch
6. Never Cache URLs (Checkout/Cart/My Account)
7. Database Cleanup
8. CDN Integration (ถ้ามี)
9. Heartbeat Control
10. **ทดสอบด้วย GTmetrix รอบสุดท้าย**

---

## SLIDE 14: สรุปและก้าวต่อไป (Summary & Next Steps)

- WP-Rocket = ปลั๊กอิน Cache ครบวงจรสำหรับ WordPress
- File Optimization + LazyLoad + Preloading + DB Cleanup + CDN
- หลักการทอง: **เปิดทีละตัว ทดสอบทุกครั้ง**
- ทดสอบด้วย GTmetrix ก่อนและหลัง
- **ตอนถัดไป:** วิธีตั้งค่า UpdraftPlus สำรองข้อมูลเว็บไซต์

---

*จำนวน Slides ทั้งหมด: 14 สไลด์*
