# วิธีปรับแต่ง Email Header — EMAIL-002
> **Format:** Slide Outline (12 Slides)
> **Source:** SWP3 Ch21 ระบบอีเมล ตอนที่ 2
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## SLIDE 1: หน้าปก (Title Slide)

- **วิธีปรับแต่ง Email Header**
- SWP3 บทที่ 21: เริ่มต้นสร้างระบบอีเมล — ตอนที่ 2
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- เข้าใจหน้าที่และองค์ประกอบของ Email Header
- ตั้งค่า From Name, From Email และ Reply-to ได้ถูกต้อง
- เขียน Pre-header Text ที่ดึงดูดการเปิดอ่าน
- เลือกระหว่าง HTML และ Plain Text ได้อย่างเหมาะสม
- ออกแบบอีเมลให้ Mobile Responsive
- ใส่ Footer ครบถ้วนตามข้อกำหนดทางกฎหมาย

---

## SLIDE 3: Email Header คืออะไร? (Definition)

- ส่วนบนสุดของอีเมล — สิ่งแรกที่ผู้รับเห็น
- สร้าง Brand Recognition (การจดจำแบรนด์)
- สร้างความน่าเชื่อถือ ไม่ให้ถูกมองว่าเป็นสแปม
- เปรียบเทียบ: เหมือน "หน้าร้าน" ของธุรกิจ
- Header ที่ดี = ลูกค้าไว้ใจ = เปิดอ่านมากขึ้น

---

## SLIDE 4: องค์ประกอบ 4 อย่างของ Header (Key Components)

- **โลโก้** — ตรงกลางหรือมุมซ้ายบน ขนาดเหมาะสม
- **สีแบรนด์** — ใช้สีหลักเป็นพื้นหลังหรือเส้นคั่น
- **ลิงก์นำทาง** — เว็บ บล็อก Social Media (ไม่เกิน 3-4 ลิงก์)
- **Pre-header Text** — ข้อความเสริม Subject Line ใน inbox
- สม่ำเสมอทุกอีเมล = Brand Consistency

---

## SLIDE 5: Pre-header Text (ข้อความตัวอย่าง)

- ข้อความสั้นที่แสดงถัดจาก Subject Line ในกล่องจดหมาย
- ช่วยเพิ่ม Open Rate อย่างมาก
- ความยาว 40-100 ตัวอักษร
- เสริม Subject Line — ให้ข้อมูลเพิ่ม ไม่ใช่พูดซ้ำ
- อย่าปล่อยว่าง — ระบบจะดึงข้อความบรรทัดแรกมาแทน

---

## SLIDE 6: การตั้งค่าผู้ส่ง (Sender Settings)

| การตั้งค่า | ตัวอย่างที่ดี | ตัวอย่างที่ไม่ดี |
|-----------|-------------|---------------|
| From Name | "สมชาย จาก PinkCastle" | "noreply" |
| From Email | newsletter@pinkcastle.com | somchai123@gmail.com |
| Reply-to | support@pinkcastle.com | noreply@pinkcastle.com |

- From Name: ชื่อจริง + ชื่อแบรนด์ = จดจำได้ + เป็นส่วนตัว
- Reply-to อาจต่างจาก From Email เพื่อส่งไปทีมที่เหมาะสม

---

## SLIDE 7: Footer — สิ่งที่ต้องมีตามกฎหมาย (Legal Requirements)

- **Unsubscribe Link** — บังคับ! ลิงก์ยกเลิกสมาชิกที่ชัดเจน
- **ที่อยู่ทางกายภาพ** — ที่อยู่จริงของบริษัทหรือ PO Box
- **Privacy Policy Link** — ลิงก์นโยบายความเป็นส่วนตัว
- กฎหมาย CAN-SPAM Act — ฝ่าฝืนมีค่าปรับ
- ถ้าไม่มี Unsubscribe Link → คนกด Report Spam → ถูกบล็อก

---

## SLIDE 8: HTML vs Plain Text Email (Comparison)

| เกณฑ์ | HTML | Plain Text |
|-------|------|-----------|
| รูปแบบ | มีสี รูป ปุ่ม | ข้อความล้วน |
| จุดเด่น | มืออาชีพ สวย | จริงใจ เป็นส่วนตัว |
| เหมาะกับ | Newsletter โปรโมชัน | Follow-up ส่วนตัว |
| Inbox | อาจเข้า Promotion | มักเข้า Primary |

- เคล็ดลับ: ใช้ทั้งสองแบบตามสถานการณ์

---

## SLIDE 9: Mobile Responsive — ทำไมถึงสำคัญ (Mobile Design)

- **60%+ ของคนเปิดอีเมลบนมือถือ**
- อีเมลที่แสดงผลไม่ดีบนมือถือ → ลบทิ้งทันที
- Header ต้องปรับขนาดตามหน้าจอ
- ปุ่ม CTA ต้องใหญ่พอกดด้วยนิ้ว (44x44px+)
- ตัวอักษร 14px ขึ้นไป อ่านง่ายไม่ต้องซูม
- ใช้คอลัมน์เดียวบนมือถือ

---

## SLIDE 10: Email Template มาตรฐาน (Standard Template)

- สร้าง Template ครั้งเดียว ใช้ได้กับทุกอีเมล
- โครงสร้าง: Header → เนื้อหา → CTA → Footer
- รักษา Brand Consistency ทุกฉบับ
- ประหยัดเวลาในการสร้างอีเมลใหม่
- ทดสอบ Template บนทุกอุปกรณ์ก่อนใช้งาน

---

## SLIDE 11: Branding Checklist (ตรวจสอบก่อนส่ง)

- [ ] โลโก้ตำแหน่งถูกต้อง คมชัด
- [ ] สีแบรนด์ตรงกับเว็บไซต์
- [ ] From Name เป็นชื่อที่คนจำได้
- [ ] Pre-header Text เขียนเสริม Subject Line
- [ ] Mobile Responsive ทดสอบแล้ว
- [ ] Footer ครบ: Unsubscribe + ที่อยู่ + Privacy Policy
- [ ] ลิงก์ทั้งหมดทำงานถูกต้อง

---

## SLIDE 12: สรุปและก้าวต่อไป (Summary & Next Steps)

- Email Header สร้างความประทับใจแรกและ Brand Recognition
- ตั้งค่าผู้ส่ง: From Name + From Email + Reply-to
- Pre-header Text เสริม Subject Line เพิ่ม Open Rate
- Footer ต้องครบตามกฎหมาย: Unsubscribe + ที่อยู่ + Privacy
- Mobile Responsive คือสิ่งจำเป็น (60%+ เปิดบนมือถือ)
- **ขั้นตอนถัดไป:** ตอนหน้าจะพูดเรื่องการแก้ไขจดหมายฉบับที่ 1 Welcome Email

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
