# Flashcards: วิธีตั้งค่า Plugin Jetpack — WEB2-008
> **Format:** Flashcards (Q&A)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 8
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

=== CARD 1 (Definition) ===

**Q:** Jetpack คืออะไร? ใครเป็นคนพัฒนา?

**A:** Jetpack คือ all-in-one plugin สำหรับ WordPress ที่รวมฟีเจอร์ Security, Performance และ Traffic ไว้ในตัวเดียว พัฒนาโดย Automattic ซึ่งเป็นบริษัทเดียวกับที่ทำ WordPress.com มีผู้ติดตั้งมากกว่า 5 ล้านเว็บไซต์ทั่วโลก

---

=== CARD 2 (Technical) ===

**Q:** ทำไมต้องเชื่อมต่อ Jetpack กับบัญชี WordPress.com?

**A:** เพราะฟีเจอร์หลายอย่างของ Jetpack ทำงานผ่าน cloud ของ WordPress.com เช่น CDN, Stats, Downtime Monitoring, Brute Force Protection ถ้าไม่เชื่อมต่อจะใช้ฟีเจอร์เหล่านี้ไม่ได้ การสมัครบัญชี WordPress.com ฟรี

---

=== CARD 3 (Concept) ===

**Q:** Brute Force Protection ใน Jetpack คืออะไร? ป้องกันอะไร?

**A:** Brute Force Protection คือฟีเจอร์ที่ป้องกันการพยายามเข้าสู่ระบบแบบสุ่มรหัสผ่าน (Brute Force Attack) โดย bot จะลองล็อกอินซ้ำๆ ด้วยรหัสผ่านต่างๆ Jetpack จะบล็อก IP address ที่มีพฤติกรรมน่าสงสัยอัตโนมัติ ฟีเจอร์นี้ฟรี

---

=== CARD 4 (Explanation) ===

**Q:** Downtime Monitoring ทำงานอย่างไร?

**A:** Downtime Monitoring ตรวจสอบว่าเว็บไซต์ออนไลน์อยู่หรือไม่ ทุกๆ 5 นาที ถ้าเว็บล่มหรือเข้าไม่ได้ จะส่ง email แจ้งเตือนเจ้าของเว็บทันที ทำให้แก้ไขปัญหาได้เร็วก่อนเสียลูกค้า ฟีเจอร์นี้ฟรี ไม่ต้องอัปเกรดแพลน

---

=== CARD 5 (Technical) ===

**Q:** Site Accelerator (CDN) ใน Jetpack คืออะไร? ทำงานอย่างไร?

**A:** Site Accelerator คือ CDN ฟรีจาก Jetpack ที่ serve รูปภาพและ Static Files (CSS, JavaScript) ผ่านเครือข่ายของ WordPress.com แทนที่จะดึงจาก server ของเรา ทำให้เว็บโหลดเร็วขึ้น แค่เปิด module ก็ใช้ได้เลย ไม่ต้องตั้งค่าเพิ่ม

---

=== CARD 6 (Application) ===

**Q:** Site Stats ใน Jetpack แสดงข้อมูลอะไรบ้าง?

**A:** Site Stats แสดงสถิติการเข้าชมเว็บไซต์ในหน้า Admin Dashboard ได้แก่ (1) จำนวนผู้เข้าชมรายวัน/สัปดาห์/เดือน (2) หน้าที่ถูกเข้าชมมากที่สุด (3) แหล่งที่มาของ Traffic (Search, Social, Direct) (4) ลิงก์ที่ถูกคลิก ดูข้อมูลได้ทันทีไม่ต้องเปิด Google Analytics

---

=== CARD 7 (Concept) ===

**Q:** Publicize ใน Jetpack คืออะไร? ต่างจาก Sharing อย่างไร?

**A:** Publicize คือฟีเจอร์ Auto-posting ที่แชร์บทความใหม่ไปยัง Social Media อัตโนมัติเมื่อ publish เชื่อมต่อได้หลายแพลตฟอร์ม ส่วน Sharing คือปุ่มแชร์ที่แสดงบนบทความให้ผู้อ่านกดแชร์เอง สรุปคือ Publicize = เราแชร์อัตโนมัติ / Sharing = ผู้อ่านแชร์

---

=== CARD 8 (Comparison) ===

**Q:** Jetpack แพลนฟรีกับเสียเงินต่างกันอย่างไร?

**A:** แพลนฟรีได้: Brute Force Protection, Downtime Monitoring, CDN, Lazy Images, Stats, Related Posts, Social Sharing, Publicize แพลนเสียเงินเพิ่ม: Automated Backup ทุกวัน, Malware Scanning, Spam Protection ขั้นสูง, Priority Support สำหรับเว็บทั่วไปแพลนฟรีเพียงพอ

---

=== CARD 9 (Best Practice) ===

**Q:** Module ใดใน Jetpack ที่ควรเปิดใช้เสมอ?

**A:** Module ที่ควรเปิดเสมอมี 8 ตัว ได้แก่ (1) Brute Force Protection (2) Downtime Monitoring (3) Site Accelerator/CDN (4) Lazy Images (5) Site Stats (6) Related Posts (7) Sharing (8) Publicize ทั้ง 8 ตัวฟรีและช่วยเรื่อง Security, Performance, Traffic

---

=== CARD 10 (Best Practice) ===

**Q:** Module ใดใน Jetpack ที่ควรพิจารณาปิด?

**A:** Module ที่ควรพิจารณาปิดถ้าไม่ได้ใช้ ได้แก่ (1) Carousel — ถ้าไม่ใช้แกลเลอรี่รูปภาพ (2) Tiled Galleries — ถ้าไม่ต้องการ (3) Subscriptions — ถ้าใช้บริการ newsletter ตัวอื่นอยู่แล้ว (4) JSON API — ถ้าไม่ได้ใช้แอปมือถือ WordPress การปิด module ที่ไม่ใช้ช่วยลดภาระของเว็บ

---

=== CARD 11 (Application) ===

**Q:** Jetpack Social Sharing เชื่อมต่อกับ Social Media ใดได้บ้าง?

**A:** Jetpack Social Sharing เชื่อมต่อได้หลายแพลตฟอร์ม ได้แก่ Facebook, Twitter, LinkedIn, Tumblr สำหรับปุ่มแชร์ยังรองรับ Pinterest, WhatsApp, Telegram, Email และอื่นๆ อีก การตั้งค่า Publicize ทำได้ที่ Jetpack > Settings > Sharing

---

=== CARD 12 (Summary) ===

**Q:** สรุป Jetpack มีฟีเจอร์หลักกี่ด้าน? แต่ละด้านมีอะไรบ้าง?

**A:** Jetpack มี 3 ด้านหลัก ได้แก่ (1) Security — Brute Force Protection, Downtime Monitoring, Security Scanning (Paid) (2) Performance — CDN, Lazy Images (3) Traffic — Site Stats, Related Posts, Social Sharing, Publicize ทั้งหมดรวมอยู่ในปลั๊กอินเดียว

---

*จำนวน Flashcards ทั้งหมด: 12 ใบ*
