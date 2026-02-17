# Insights Table: วิธีติดตั้ง Google Analytics — WEB2-011
> **Format:** Insights Table (10 Rows)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 11
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

| # | Insight (ข้อค้นพบ) | Detail (รายละเอียด) | Application (การนำไปใช้) | Impact Level (ระดับผลกระทบ) |
|---|---|---|---|---|
| 1 | GA4 คือเวอร์ชันปัจจุบันของ Google Analytics | Google Analytics 4 เป็นเวอร์ชันใหม่ที่ใช้ Event-based model แทน Session-based แบบเดิม รองรับทั้งเว็บไซต์และแอปพลิเคชัน | สร้าง Account ที่ analytics.google.com ทุกเว็บไซต์ต้องมี GA4 เพื่อเก็บข้อมูลพฤติกรรมผู้เข้าชม | สูง |
| 2 | Time Zone และ Currency ต้องตั้งถูกตั้งแต่แรก | ตั้ง Time Zone เป็น "(GMT+07:00) Bangkok" และ Currency เป็น "Thai Baht (THB)" การแก้ไขภายหลังจะไม่ส่งผลย้อนหลังกับข้อมูลที่เก็บไปแล้ว | ตรวจสอบให้แน่ใจว่า Time Zone และ Currency ถูกต้องก่อนเริ่มเก็บข้อมูล อย่าปล่อยให้เป็นค่า default | สูง |
| 3 | Measurement ID คือกุญแจเชื่อมเว็บกับ Analytics | รหัสรูปแบบ G-XXXXXXXXXX ที่ได้จากการสร้าง Data Stream ใช้ระบุว่าข้อมูลมาจากเว็บไซต์ใด | เก็บ Measurement ID ไว้ในที่ปลอดภัย ใช้ติดตั้งผ่าน Site Kit, gtag.js หรือ GTM | กลาง |
| 4 | Site Kit คือวิธีง่ายที่สุดสำหรับมือใหม่ | ติดตั้ง Analytics ผ่าน Site Kit Plugin ไม่ต้องแตะโค้ดเลย แค่เชื่อมต่อ Google Account และเลือก Property ที่ต้องการ | มือใหม่เริ่มจาก Site Kit ก่อน เมื่อคุ้นเคยแล้วค่อยพิจารณาเปลี่ยนไปใช้ GTM ในภายหลัง | กลาง |
| 5 | Google Tag Manager เหมาะสำหรับจัดการ tag หลายตัว | GTM ช่วยจัดการ Analytics, Facebook Pixel, Ads conversion tag จากที่เดียว ติดตั้ง GTM บนเว็บครั้งเดียว แล้วเพิ่ม/แก้ tag ผ่าน GTM interface | ถ้าวางแผนทำ Digital Marketing จริงจัง (Google Ads + Facebook Ads) ให้ใช้ GTM ตั้งแต่แรก | สูง |
| 6 | Users vs Sessions ต้องเข้าใจความแตกต่าง | Users = ผู้เข้าชมไม่ซ้ำ (1 คนเข้า 10 ครั้ง = 1 User) Sessions = จำนวนเข้าชมทั้งหมด (1 คนเข้า 3 ครั้ง = 3 Sessions) | ใช้ Users เพื่อวัดขนาดกลุ่มเป้าหมาย ใช้ Sessions เพื่อวัดความถี่ในการกลับมา Sessions/Users สูง = คนกลับมาบ่อย | สูง |
| 7 | Bounce Rate สูงเกินไปคือสัญญาณเตือน | Bounce Rate คืออัตราคนที่เข้ามาแล้วออกโดยไม่คลิกอะไร 26-40% ดี 41-55% เฉลี่ย มากกว่า 70% ต้องปรับปรุง | วิเคราะห์หน้าที่มี Bounce Rate สูง แล้วปรับปรุงเนื้อหา ความเร็ว หรือ Call-to-Action ให้ดีขึ้น | สูง |
| 8 | Conversion Tracking เชื่อม Traffic กับผลลัพธ์ธุรกิจ | ตั้งค่าให้ Analytics ติดตามเป้าหมายสำคัญ เช่น ซื้อสินค้า กรอกฟอร์ม สมัครสมาชิก ดาวน์โหลดไฟล์ | ตั้ง Conversion ให้ครบทุกเป้าหมายธุรกิจ ใช้ข้อมูล Conversion วัด ROI ของทุกช่องทางการตลาด | สูง |
| 9 | PDPA กำหนดให้ต้องมี Cookie Consent | พ.ร.บ. คุ้มครองข้อมูลส่วนบุคคล กำหนดให้เว็บไซต์แจ้งและขอความยินยอมก่อนเก็บ Cookie โทษปรับสูงสุด 5 ล้านบาท | ติดตั้งปลั๊กอิน Cookie Consent (เช่น CookieYes, Complianz) ทันทีหลังติดตั้ง Analytics | สูง |
| 10 | Analytics เปลี่ยนการเดาเป็นการใช้ข้อมูล | ข้อมูลจาก Analytics ช่วยตัดสินใจบนพื้นฐานข้อเท็จจริง ไม่ใช่การคาดเดา ทุกการเปลี่ยนแปลงบนเว็บไซต์สามารถวัดผลได้ | ตรวจสอบ Analytics อย่างน้อยสัปดาห์ละครั้ง สร้างรายงานพื้นฐาน ใช้ข้อมูลประกอบทุกการตัดสินใจเกี่ยวกับเว็บไซต์ | กลาง |

---

## สรุปตาม Impact Level

| ระดับ | จำนวน Insights | หัวข้อหลัก |
|-------|:---:|---|
| สูง | 7 | GA4, Time Zone/Currency, GTM, Users vs Sessions, Bounce Rate, Conversion Tracking, PDPA |
| กลาง | 3 | Measurement ID, Site Kit, ใช้ข้อมูลตัดสินใจ |
| ต่ำ | 0 | — |

---

*จำนวน Insights ทั้งหมด: 10 รายการ*
