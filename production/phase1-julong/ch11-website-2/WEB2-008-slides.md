# Slides: วิธีตั้งค่า Plugin Jetpack — WEB2-008
> **Format:** Slide Outline (12 Slides)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 8
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## Slide 1: หน้าปก (Title Slide)

- **วิธีตั้งค่า Plugin Jetpack**
- SWP3 บทที่ 11: สร้างเว็บไซต์ Part 2 — ตอนที่ 8
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## Slide 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- ทำความรู้จัก Jetpack และเหตุผลที่ควรใช้
- ติดตั้งและเชื่อมต่อกับ WordPress.com
- ตั้งค่าฟีเจอร์ Security, Performance, Traffic
- เปรียบเทียบแพลนฟรีกับเสียเงิน
- จัดการ Module ที่ควรเปิดและควรปิด

---

## Slide 3: Jetpack คืออะไร?

- **All-in-one Plugin** — รวม Security + Performance + Traffic
- พัฒนาโดย **Automattic** (ทีมเดียวกับ WordPress.com)
- ติดตั้งมากกว่า **5 ล้านเว็บไซต์** ทั่วโลก
- เหมือน "มีดพับสวิส" ของ WordPress
- ต้องเชื่อมต่อบัญชี WordPress.com เพื่อใช้ฟีเจอร์ cloud

---

## Slide 4: การติดตั้งและเชื่อมต่อ

- **ขั้นตอน 1:** Plugins > Add New > ค้นหา "Jetpack" > Install
- **ขั้นตอน 2:** กด Activate
- **ขั้นตอน 3:** กด "Set up Jetpack" > เชื่อมต่อ WordPress.com
- **ขั้นตอน 4:** ล็อกอินหรือสมัคร WordPress.com (ฟรี)
- **ขั้นตอน 5:** อนุญาตการเชื่อมต่อ > เสร็จ!

---

## Slide 5: Security — Brute Force Protection

- ป้องกันการ **สุ่มรหัสผ่าน** (Brute Force Attack)
- Bot จะลองล็อกอินซ้ำๆ ด้วยรหัสต่างๆ
- Jetpack **บล็อก IP** ที่น่าสงสัยอัตโนมัติ
- ฟีเจอร์นี้ **ฟรี** เปิดได้ทันที
- ใช้ร่วมกับรหัสผ่านแข็งแรง + 2FA ยิ่งปลอดภัย

---

## Slide 6: Security — Downtime Monitoring

- ตรวจสอบว่าเว็บออนไลน์อยู่หรือไม่ **ทุก 5 นาที**
- เว็บล่ม → ส่ง **email แจ้งเตือนทันที**
- แก้ไขได้เร็วก่อนเสียลูกค้าหรืออันดับ SEO
- ฟีเจอร์นี้ **ฟรี** ไม่ต้องอัปเกรด
- แพลนเสียเงินเพิ่ม: Malware Scanning + Automated Backup

---

## Slide 7: Performance — CDN และ Lazy Images

- **Site Accelerator (CDN)**
  - Serve รูปภาพและ Static Files ผ่านเครือข่าย WordPress.com
  - CDN ฟรี — แค่เปิด module ก็ใช้ได้เลย
- **Lazy Images**
  - โหลดรูปเมื่อผู้ใช้เลื่อนมาถึง
  - หน้าแรกเปิดเร็วขึ้นมาก
- ทั้งสองฟีเจอร์ **ฟรี** แนะนำเปิดทั้งคู่

---

## Slide 8: Traffic — Site Stats

- แสดงสถิติในหน้า **WordPress Admin Dashboard**
- ข้อมูลที่เห็น: ผู้เข้าชม, หน้ายอดนิยม, แหล่งที่มา Traffic
- ดูง่าย **ไม่ต้องเปิด Google Analytics** แยกต่างหาก
- เหมาะสำหรับดูภาพรวมเบื้องต้น
- ต้องการเชิงลึกมากกว่า → เพิ่ม Google Analytics

---

## Slide 9: Traffic — Related Posts และ Social

- **Related Posts** — แสดงบทความเกี่ยวข้องท้ายบทความอัตโนมัติ
  - เพิ่ม Pageviews + ลด Bounce Rate
- **Sharing** — ปุ่มแชร์ Social Media บนบทความ
  - Facebook, Twitter, LinkedIn, Pinterest, etc.
- **Publicize** — Auto-posting ไป Social Media เมื่อ publish
  - ตั้งค่าครั้งเดียว ใช้ได้ตลอด

---

## Slide 10: Free vs Paid — เลือกแพลนไหนดี?

| ฟีเจอร์ | Free | Paid |
|---------|:---:|:---:|
| Brute Force + Downtime | ได้ | ได้ |
| CDN + Lazy Images | ได้ | ได้ |
| Stats + Related Posts | ได้ | ได้ |
| Sharing + Publicize | ได้ | ได้ |
| Automated Backup | ไม่ได้ | ได้ |
| Malware Scanning | ไม่ได้ | ได้ |

- **สรุป:** เว็บทั่วไปใช้ฟรีก็พอ

---

## Slide 11: Module Management — เปิดอะไร ปิดอะไร

**ควรเปิด (8 module):**
- Brute Force, Downtime Monitoring
- Site Accelerator, Lazy Images
- Site Stats, Related Posts, Sharing, Publicize

**ควรพิจารณาปิด:**
- Carousel (ถ้าไม่ใช้แกลเลอรี่)
- Tiled Galleries (ถ้าไม่ต้องการ)
- Subscriptions (ถ้าใช้ newsletter ตัวอื่น)
- JSON API (ถ้าไม่ใช้แอปมือถือ)

---

## Slide 12: สรุปและก้าวต่อไป (Summary & Next Steps)

- Jetpack = All-in-one (Security + Performance + Traffic)
- ต้องเชื่อมต่อ WordPress.com
- เปิด 8 module หลัก ปิดที่ไม่ใช้
- แพลนฟรีเพียงพอสำหรับเว็บส่วนใหญ่
- **ขั้นตอนถัดไป:** ตั้งค่า Plugin Akismet สำหรับ Anti-spam

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
