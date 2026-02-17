# Insights Table: วิธีปรับแต่ง WordPress Admin Panel — WEB1-011
> **Format:** Insights Table (10 Rows)
> **Source:** SWP3 Ch10 สร้างเว็บไซต์ Part 1 ตอนที่ 11
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

| # | Insight (ข้อค้นพบ) | Detail (รายละเอียด) | Application (การนำไปใช้) | Impact Level (ระดับผลกระทบ) |
|---|---|---|---|---|
| 1 | Permalinks ต้องตั้งให้ถูกตั้งแต่วันแรก | การใช้ Post name (yoursite.com/sample-post) ดีต่อ SEO และผู้ใช้อ่านง่าย การเปลี่ยนภายหลังจะทำให้ URL เดิมเป็น 404 เสีย SEO | เข้า Settings > Permalinks เปลี่ยนเป็น Post name ทันทีหลังติดตั้ง WordPress อย่าใช้แบบ Default (?p=123) | สูง |
| 2 | User Roles ต้องให้สิทธิ์เท่าที่จำเป็น | WordPress มี 5 บทบาท (Admin, Editor, Author, Contributor, Subscriber) การให้ทุกคนเป็น Admin เพิ่มความเสี่ยงด้านความปลอดภัยอย่างมาก | ทบทวน User Roles ของทุกคนในทีม กำหนดบทบาทตามหน้าที่จริง นักเขียน = Author ผู้ส่งบทความ = Contributor | สูง |
| 3 | Security Hardening เริ่มตั้งแต่วันแรก | Username "admin" เป็นเป้าหมายแรกของ Hacker รหัสผ่านอ่อนแอ + ไม่จำกัด Login attempts = ความเสี่ยงสูง | เปลี่ยน Username จาก admin ใช้รหัสผ่านยาว 12+ ตัวอักษร จำกัด Login ผิดได้ 3-5 ครั้ง อัปเดตทุกอย่างสม่ำเสมอ | สูง |
| 4 | Reading Settings กำหนดหน้าตาเว็บทั้งหมด | เลือกได้ว่าหน้าแรกจะแสดงบทความล่าสุด (เหมาะ Blog) หรือ Static Page (เหมาะเว็บธุรกิจ) ส่งผลต่อ First Impression ของผู้เยี่ยมชม | เว็บธุรกิจควรเลือก Static Page แล้วออกแบบ Homepage ให้สวยงาม เว็บ Blog เลือก Your latest posts | สูง |
| 5 | Dashboard Widgets จัดระเบียบได้ | Widget ที่ไม่จำเป็นสร้างความรกและเสียสมาธิ Screen Options ช่วยเลือกแสดงเฉพาะข้อมูลที่ต้องการ | เปิด Screen Options ปิด Widget ที่ไม่ใช้ ลากจัดลำดับ Widget ตามลำดับความสำคัญ | กลาง |
| 6 | Discussion Settings ต้องจัดการเรื่อง Spam | การเปิด Comments โดยไม่ตั้งค่าป้องกันจะถูก Spam Comments รุมเต็มเว็บ ส่งผลเสียต่อภาพลักษณ์และ SEO | เว็บธุรกิจพิจารณาปิด Comments ถ้าเปิดให้ตั้ง Manual Approval + ใช้ Akismet กรอง Spam | กลาง |
| 7 | Media Settings ส่งผลต่อพื้นที่ Hosting | WordPress สร้างรูป 3 ขนาดอัตโนมัติทุกครั้งที่อัปโหลด ถ้าอัปโหลดรูปเยอะจะกินพื้นที่มาก | ตั้งค่าขนาดรูปให้เหมาะกับ Theme ที่ใช้ ขนาดที่ไม่ต้องการให้ตั้งเป็น 0 เพื่อประหยัดพื้นที่ | กลาง |
| 8 | Privacy Policy เป็นข้อบังคับทางกฎหมาย | กฎหมายหลายประเทศ (GDPR, PDPA) กำหนดให้เว็บที่เก็บข้อมูลส่วนบุคคลต้องมีหน้า Privacy Policy | เข้า Settings > Privacy สร้าง Privacy Policy Page โดยใช้เทมเพลตที่ WordPress มีให้ แล้วปรับเนื้อหาให้ตรงกับเว็บ | สูง |
| 9 | Admin Menu Customization ช่วยเพิ่มประสิทธิภาพ | เมนูด้านซ้ายของ Admin Panel มีรายการเยอะ โดยเฉพาะเมื่อติดตั้ง Plugin หลายตัว ทำให้หาเมนูที่ต้องการยาก | ใช้ Plugin เช่น Admin Menu Editor ซ่อนเมนูไม่จำเป็น จัดลำดับใหม่ให้เมนูที่ใช้บ่อยอยู่ด้านบน | กลาง |
| 10 | อัปเดต WordPress/Plugin/Theme สม่ำเสมอ | ทุกเวอร์ชันใหม่มักแก้ช่องโหว่ด้านความปลอดภัย การไม่อัปเดตเท่ากับเปิดช่องให้ Hacker โจมตี | ตั้งเวลาตรวจสอบอัปเดตอย่างน้อยสัปดาห์ละครั้ง สำรองข้อมูลก่อนอัปเดตทุกครั้ง | สูง |

---

## สรุปตาม Impact Level

| ระดับ | จำนวน Insights | หัวข้อหลัก |
|-------|:---:|---|
| สูง | 5 | Permalinks, User Roles, Security, Reading Settings, Privacy, อัปเดต |
| กลาง | 5 | Dashboard Widgets, Discussion/Spam, Media Settings, Admin Menu |
| ต่ำ | 0 | — |

---

*จำนวน Insights ทั้งหมด: 10 รายการ*
