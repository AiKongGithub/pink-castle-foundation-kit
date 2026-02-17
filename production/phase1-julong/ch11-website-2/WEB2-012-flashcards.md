# Flashcards: วิธีการตั้งค่า WP-Rocket — WEB2-012
> **Format:** Flashcards (Q&A)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 12
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

=== CARD 1 ===

**Q:** WP-Rocket คืออะไร?

**A:** ปลั๊กอิน Cache สำหรับ WordPress ที่ช่วยเพิ่มความเร็วเว็บไซต์ผ่านเทคนิคหลายระดับ ได้แก่ Page Caching, File Optimization, LazyLoad, Preloading, Database Cleanup, CDN Integration และ Heartbeat Control เป็นหนึ่งในปลั๊กอิน Cache ที่นิยมที่สุด

---

=== CARD 2 ===

**Q:** Minify CSS/JS คืออะไร และช่วยอย่างไร?

**A:** Minify คือการลบช่องว่าง บรรทัดว่าง และ comment ที่ไม่จำเป็นออกจากไฟล์ CSS และ JavaScript ทำให้ขนาดไฟล์เล็กลง โหลดเร็วขึ้น โดยไม่ส่งผลต่อการทำงานของโค้ด

---

=== CARD 3 ===

**Q:** Combine CSS/JS คืออะไร และมีข้อควรระวังอะไร?

**A:** Combine คือการรวมไฟล์ CSS หรือ JS หลายไฟล์เป็นไฟล์เดียว เพื่อลดจำนวน HTTP Requests ข้อควรระวังคืออาจทำให้หน้าตาเว็บเพี้ยนหรือฟังก์ชันบางอย่างพัง ถ้าเจอปัญหาให้ปิด Combine แล้วใช้แค่ Minify

---

=== CARD 4 ===

**Q:** Defer JS Loading ทำงานอย่างไร?

**A:** ปกติ browser จะหยุดแสดงหน้าเว็บเพื่อรอดาวน์โหลดและรัน JavaScript ก่อน Defer JS Loading จะให้ HTML โหลดเสร็จก่อนแล้วค่อยรัน JS ทีหลัง ทำให้ผู้ใช้เห็นเนื้อหาเร็วขึ้นมากโดยไม่กระทบการทำงานของ JS

---

=== CARD 5 ===

**Q:** LazyLoad คืออะไร และช่วยเว็บไซต์อย่างไร?

**A:** LazyLoad คือเทคนิคที่ให้รูปภาพ iframes และวิดีโอโหลดเฉพาะตอนที่ผู้ใช้เลื่อนหน้าจอลงมาถึง ไม่โหลดทั้งหมดพร้อมกัน ช่วยลดเวลาโหลดหน้าแรกอย่างมาก โดยเฉพาะเว็บที่มีรูปภาพและวิดีโอจำนวนมาก

---

=== CARD 6 ===

**Q:** Add Missing Image Dimensions ช่วยแก้ปัญหาอะไร?

**A:** ช่วยเพิ่มค่า width และ height ให้กับรูปภาพที่ไม่มี ลดปัญหา Layout Shift (CLS) คือหน้าเว็บกระตุกเมื่อรูปโหลดเสร็จ CLS เป็นหนึ่งใน Core Web Vitals ของ Google ที่ส่งผลต่ออันดับ SEO

---

=== CARD 7 ===

**Q:** WebP คืออะไร และ WP-Rocket ช่วยอย่างไร?

**A:** WebP เป็นรูปแบบภาพจาก Google ที่มีขนาดเล็กกว่า JPEG/PNG ประมาณ 25-30% แต่คุณภาพเท่ากัน WP-Rocket มี WebP Compatibility ที่ส่งไฟล์ WebP ให้ browser ที่รองรับโดยอัตโนมัติ ถ้า browser ไม่รองรับก็ส่ง JPEG/PNG แทน

---

=== CARD 8 ===

**Q:** Sitemap-based Preloading ทำงานอย่างไร?

**A:** WP-Rocket จะไล่ Crawl หน้าเว็บตาม Sitemap ที่กำหนด แล้วสร้าง cache ล่วงหน้าสำหรับทุกหน้า ทำให้ผู้เข้าชมทุกคนได้รับหน้าที่ cache ไว้แล้วทันที ไม่ต้องรอสร้าง cache ใหม่

---

=== CARD 9 ===

**Q:** DNS Prefetch คืออะไร และควรใส่ domain อะไร?

**A:** DNS Prefetch บอกให้ browser ไป resolve DNS ของ domain ภายนอกล่วงหน้า ช่วยลดเวลารอเมื่อโหลดทรัพยากรจาก domain นั้น ควรใส่ domain ที่เว็บใช้บ่อย เช่น fonts.googleapis.com, CDN domain, Google Analytics domain

---

=== CARD 10 ===

**Q:** Never Cache URLs ใช้ตั้งค่าหน้าไหนบ้าง?

**A:** ใช้กับหน้าที่มีข้อมูลเปลี่ยนแปลงตลอดเวลาและไม่ควร cache เช่น หน้า Checkout, หน้า Cart, หน้า My Account, หน้า Login เพื่อให้ผู้ใช้เห็นข้อมูลล่าสุดเสมอ ป้องกันปัญหาข้อมูลล้าสมัย

---

=== CARD 11 ===

**Q:** WP-Rocket ช่วยทำความสะอาดฐานข้อมูลอะไรได้บ้าง?

**A:** ลบได้ 5 ประเภทหลัก ได้แก่ (1) Post Revisions — ประวัติการแก้ไขบทความ (2) Auto Drafts — ร่างอัตโนมัติ (3) Transients — ข้อมูลชั่วคราว (4) Spam Comments — ความคิดเห็นสแปม (5) Optimize Tables — ปรับขนาดตารางฐานข้อมูลให้เล็กลง

---

=== CARD 12 ===

**Q:** Heartbeat API คืออะไร และทำไม WP-Rocket ต้องควบคุม?

**A:** WordPress Heartbeat API คือระบบที่ส่งข้อมูลกลับไปหา server ทุก 15-60 วินาที ใช้สำหรับ auto-save, notifications ฯลฯ แต่กินทรัพยากร server มาก WP-Rocket ช่วยลดความถี่หรือปิด Heartbeat ในหน้าที่ไม่จำเป็น เช่น หน้า Dashboard หรือ Frontend

---

=== CARD 13 ===

**Q:** ควรทดสอบความเร็วเว็บไซต์ก่อน-หลังติดตั้ง WP-Rocket ด้วยเครื่องมืออะไร?

**A:** ใช้ GTmetrix (gtmetrix.com) ทดสอบก่อนเปิด WP-Rocket บันทึกคะแนน จากนั้นตั้งค่าและทดสอบอีกครั้ง โดยทั่วไปคะแนน PageSpeed จะเพิ่มขึ้น 20-40 คะแนน และเวลาโหลดลดลง 40-60%

---

=== CARD 14 ===

**Q:** หลักการสำคัญในการตั้งค่า WP-Rocket คืออะไร?

**A:** เปิดฟีเจอร์ทีละตัว แล้วทดสอบเว็บไซต์หลังเปิดทุกครั้ง อย่าเปิดทุกอย่างพร้อมกัน เพราะถ้ามีปัญหาจะไม่รู้ว่าฟีเจอร์ไหนที่เป็นสาเหตุ เริ่มจาก Minify > Defer JS > LazyLoad > Preloading > Database > CDN ตามลำดับ

---

*จำนวน Flashcards ทั้งหมด: 14 ใบ*
