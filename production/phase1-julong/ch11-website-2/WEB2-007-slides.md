# Slides: วิธีการปรับแต่ง Comment Social Media — WEB2-007
> **Format:** Slide Outline (12 Slides)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 7
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## Slide 1: หน้าปก (Title Slide)

- **วิธีการปรับแต่ง Comment Social Media**
- SWP3 บทที่ 11: สร้างเว็บไซต์ Part 2 — ตอนที่ 7
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## Slide 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- เลือกระบบ Comment ที่เหมาะกับเว็บไซต์
- ตั้งค่า Comment Moderation และ Anti-spam
- เพิ่มปุ่ม Social Sharing และ Open Graph Meta Tags
- วาง Social Follow Buttons และตั้ง Auto-posting
- เปิด Social Login เพื่อเพิ่ม engagement

---

## Slide 3: ระบบ Comment — 3 ทางเลือก

| ระบบ | ข้อดี | ข้อเสีย |
|------|-------|---------|
| WordPress Comment | ข้อมูลอยู่กับเรา, ฟรี | Moderation พื้นฐาน |
| Disqus | Moderation ดี, Social Login | ข้อมูลอยู่ที่ Disqus |
| Facebook Comments | ง่าย, มี FB อยู่แล้ว | ข้อมูลอยู่ที่ Facebook |

- แนะนำ: **เริ่มจาก WordPress Comment ก่อน**

---

## Slide 4: Comment Moderation — กลั่นกรองก่อนแสดง

- ตั้งค่าที่ **Settings > Discussion**
- ให้คอมเมนต์ทุกอันต้องผ่านการอนุมัติ
- คอมเมนต์ที่มีลิงก์ → รออนุมัติอัตโนมัติ
- คนที่เคยคอมเมนต์แล้ว → ผ่านได้เลย (ตัวเลือก)
- ไม่เปิด Moderation = spam เต็มเว็บ

---

## Slide 5: Anti-spam ด้วย Akismet

- **Akismet** = ปลั๊กอินกรอง spam ที่มากับ WordPress
- ใช้ Cloud-based AI ตรวจจับ spam — แม่นเกือบ 100%
- ฟรีสำหรับเว็บไซต์ส่วนบุคคล
- ต้องลงทะเบียน API Key จาก wordpress.com
- ปลั๊กอินตัวแรกที่ต้องเปิดใช้หลังติดตั้ง WordPress

---

## Slide 6: Social Sharing Buttons — ปุ่มแชร์

- ให้ผู้อ่านแชร์บทความไป Social Media ได้ง่าย
- **ตลาดไทย:** Facebook + LINE + Twitter เป็นหลัก
- เพิ่ม: LinkedIn (คนทำงาน), Pinterest (เว็บเน้นภาพ)
- ตำแหน่ง: ท้ายบทความ หรือ Floating Sidebar
- ปลั๊กอิน: Social Warfare, AddToAny, Jetpack

---

## Slide 7: Open Graph Meta Tags — แชร์แล้วสวย

- กำหนดว่าลิงก์จะแสดง **รูป + หัวข้อ + คำอธิบาย** อะไรบน Social Media
- ถ้าไม่ตั้งค่า → Social Media ดึงข้อมูลแบบสุ่ม → รูปผิด ข้อความผิด
- ปลั๊กอิน: **Yoast SEO** หรือ **Rank Math** จัดการอัตโนมัติ
- ตั้ง Featured Image ขนาด 1200x630px สำหรับ Facebook
- ทดสอบด้วย Facebook Sharing Debugger

---

## Slide 8: Social Follow Buttons — ปุ่มติดตาม

- ต่างจาก Sharing: **Follow = ติดตามเรา** / **Share = แชร์บทความ**
- ตำแหน่ง: Sidebar, Footer, About Page
- แพลตฟอร์ม: Facebook Page, Instagram, YouTube, LINE OA
- ใส่ CTA กระตุ้นให้กดติดตาม
- ลิงก์เฉพาะ Social Media ที่ active จริง

---

## Slide 9: Auto-posting — แชร์อัตโนมัติ

- Publish บทความ → แชร์ไป Social Media ทันที
- ไม่ต้องเข้าไปแชร์เอง — ประหยัดเวลา
- **Jetpack** — มีฟีเจอร์ Publicize ในตัว
- **IFTTT** — เชื่อมต่อ WordPress กับ Social Media (ฟรี)
- **Zapier** — Automation ที่ยืดหยุ่นกว่า (มีแพลนฟรี)

---

## Slide 10: Social Login — ล็อกอินด้วย Social Media

- ให้ผู้อ่านล็อกอินด้วย **Facebook / Google / Twitter** เพื่อคอมเมนต์
- ไม่ต้องสมัครสมาชิกใหม่ — คลิกเดียว
- ลดจำนวน spam (ใช้บัญชีจริง)
- เพิ่มจำนวนคอมเมนต์อย่างมาก
- ปลั๊กอิน: Super Socializer, Nextend Social Login

---

## Slide 11: การสร้างชุมชน (Building Community)

- **Comment** — ผู้อ่านมีส่วนร่วมกับเนื้อหา
- **Share** — ขยายการเข้าถึงไปยังเครือข่ายของผู้อ่าน
- **Follow** — สร้างฐานผู้ติดตามระยะยาว
- **ผลลัพธ์:** Returning visitors + Brand loyalty + Traffic ยั่งยืน
- เคล็ดลับ: ตอบคอมเมนต์ทุกอัน + ถามคำถามท้ายบทความ

---

## Slide 12: สรุปและก้าวต่อไป (Summary & Next Steps)

- ระบบ Comment: เริ่มจาก WordPress + Akismet
- Social Sharing: 3-5 แพลตฟอร์ม + Open Graph Tags
- Social Follow + Auto-posting: ขยายฐานผู้ติดตาม
- Social Login: ลด friction เพิ่ม engagement
- **ขั้นตอนถัดไป:** ตั้งค่า Plugin Jetpack ที่รวมหลายฟีเจอร์ในตัวเดียว

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
