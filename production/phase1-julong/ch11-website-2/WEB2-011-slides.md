# Slides: วิธีติดตั้ง Google Analytics — WEB2-011
> **Format:** Slide Outline (12 Slides)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 11
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## SLIDE 1: หน้าปก (Title Slide)

- **วิธีติดตั้ง Google Analytics**
- SWP3 บทที่ 11: สร้างเว็บไซต์ Part 2 — ตอนที่ 11
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- สร้าง Google Analytics Account (GA4) ได้ด้วยตนเอง
- ตั้งค่า Property, Data Stream และ Measurement ID
- ติดตั้ง Analytics บน WordPress ได้ 3 วิธี
- เข้าใจตัวเลขสำคัญ: Users, Sessions, Bounce Rate, Pages per Session
- ตั้ง Conversion Tracking และรู้จัก PDPA

---

## SLIDE 3: ทำไมต้อง Google Analytics?

- เว็บไซต์ไม่มี Analytics = ขับรถตอนกลางคืนไม่เปิดไฟ
- ไม่รู้ว่า **ใคร** มาเว็บ
- ไม่รู้ว่ามา **จากไหน** (Google, Facebook, Direct?)
- ไม่รู้ว่า **ทำอะไร** บนเว็บ
- ไม่รู้ว่า **ออกไปตรงไหน** และทำไม
- Analytics เปลี่ยนการเดาเป็นข้อมูลจริง

---

## SLIDE 4: ขั้นตอนสร้าง Account (GA4)

- **ขั้นที่ 1:** ไปที่ analytics.google.com > Sign in
- **ขั้นที่ 2:** กด "Start measuring" > ใส่ชื่อ Account
- **ขั้นที่ 3:** สร้าง Property
  - ชื่อเว็บไซต์
  - Time Zone: **(GMT+07:00) Bangkok**
  - Currency: **Thai Baht (THB)**
- **ขั้นที่ 4:** สร้าง Data Stream > เลือก Web > ใส่ URL
- **ขั้นที่ 5:** ได้ Measurement ID (G-XXXXXXXXXX)

---

## SLIDE 5: 3 วิธีติดตั้งบน WordPress

| วิธี | ความง่าย | เหมาะกับ |
|------|---------|---------|
| Site Kit Plugin | ง่ายมาก | มือใหม่ |
| ใส่โค้ด gtag.js | ปานกลาง | รู้โค้ดเบื้องต้น |
| Google Tag Manager | ปานกลาง-ยาก | ติดตั้ง tag หลายตัว |

- แนะนำ: **มือใหม่ใช้ Site Kit** / **นักการตลาดใช้ GTM**

---

## SLIDE 6: ตัวเลขสำคัญที่ 1 — Users vs Sessions

| Metric | ความหมาย | ตัวอย่าง |
|--------|----------|---------|
| Users | ผู้เข้าชมไม่ซ้ำ | 1 คนเข้า 10 ครั้ง = 1 User |
| Sessions | จำนวนเข้าชมทั้งหมด | 1 คนเข้า 3 ครั้ง = 3 Sessions |

- Sessions >= Users เสมอ
- Sessions/Users สูง = คนกลับมาซ้ำบ่อย

---

## SLIDE 7: ตัวเลขสำคัญที่ 2 — Bounce Rate & Pages per Session

- **Bounce Rate** (อัตราตีกลับ) — ยิ่งต่ำยิ่งดี
  - 26-40% = ดี
  - 41-55% = เฉลี่ย
  - 70%+ = ต้องปรับปรุง
- **Pages per Session** — ยิ่งสูงยิ่งดี
  - คนสนใจเนื้อหา = ดูหลายหน้า
  - เพิ่มค่านี้ด้วย Internal Links และ Related Posts

---

## SLIDE 8: Conversion Tracking — วัดผลลัพธ์ธุรกิจ

- **Conversion คืออะไร?** = เป้าหมายที่อยากให้ผู้เข้าชมทำ
- ตัวอย่าง Conversion:
  - ซื้อสินค้าสำเร็จ
  - กรอกฟอร์มติดต่อ
  - สมัครจดหมายข่าว
  - ดาวน์โหลดไฟล์
- ทำไมสำคัญ: เชื่อม Traffic กับ **เงิน** จริงๆ
- ใช้วัด **ROI** ของทุกช่องทางการตลาด

---

## SLIDE 9: สร้างรายงานพื้นฐาน

- **Real-time:** ดูคนที่อยู่บนเว็บตอนนี้
- **Acquisition:** คนมาจากไหน (Google, Facebook, Direct)
- **Engagement:** คนทำอะไรบนเว็บ (หน้าไหนนิยม, เวลาเฉลี่ย)
- **Monetization:** รายได้จาก E-commerce
- **Retention:** คนกลับมาเว็บอีกไหม
- ตรวจสอบ **อย่างน้อยสัปดาห์ละครั้ง**

---

## SLIDE 10: Privacy — PDPA ต้องรู้

- **PDPA** = พ.ร.บ. คุ้มครองข้อมูลส่วนบุคคล
- เว็บไซต์ต้อง **แจ้ง** ผู้ใช้ว่ามีการเก็บ Cookie
- ต้อง **ขอความยินยอม** ก่อนเก็บข้อมูล
- ใช้ **Cookie Consent Banner** (ปลั๊กอินฟรี: CookieYes, Complianz)
- โทษปรับ: **สูงสุด 5 ล้านบาท**
- อย่ามองข้าม ติดตั้ง Banner ทันทีหลังติดตั้ง Analytics

---

## SLIDE 11: Checklist ก่อนจบ

- [ ] สร้าง GA4 Account + Property (Time Zone/Currency ถูกต้อง)
- [ ] สร้าง Data Stream + เก็บ Measurement ID
- [ ] ติดตั้งบน WordPress (Site Kit / gtag.js / GTM)
- [ ] ตรวจสอบว่าข้อมูลเข้า Real-time Report
- [ ] ตั้ง Conversion Tracking สำหรับเป้าหมายธุรกิจ
- [ ] ติดตั้ง Cookie Consent Banner (PDPA)

---

## SLIDE 12: สรุปและก้าวต่อไป (Summary & Next Steps)

- GA4 = ดวงตาของเว็บไซต์ ต้องมีทุกเว็บ
- ตั้ง Time Zone Bangkok + Currency THB ตั้งแต่แรก
- มือใหม่ใช้ Site Kit / นักการตลาดใช้ GTM
- ติดตาม Users, Sessions, Bounce Rate, Pages per Session
- ตั้ง Conversion เพื่อวัดผลลัพธ์ธุรกิจ
- **ตอนถัดไป:** วิธีตั้งค่า WP-Rocket ให้เว็บเร็วขึ้นแบบก้าวกระโดด

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
