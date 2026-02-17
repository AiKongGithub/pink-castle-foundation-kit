# Flashcards: วิธีตั้งค่า Plugin Akismet — WEB2-009
> **Format:** Flashcards (Q&A)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 9
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

=== CARD 1 (Definition) ===

**Q:** Comment Spam คืออะไร? ทำไมถึงเป็นปัญหา?

**A:** Comment Spam คือคอมเมนต์ที่ถูกสร้างโดย bot อัตโนมัติ มีเป้าหมายเพื่อใส่ลิงก์โฆษณาหรือลิงก์อันตราย เป็นปัญหาเพราะ (1) ลิงก์อาจนำไปยังเว็บ malware (2) Google อาจลงโทษเว็บที่มี spam links (3) ทำให้เว็บดูไม่น่าเชื่อถือ

---

=== CARD 2 (Concept) ===

**Q:** Akismet คืออะไร? ทำงานอย่างไร?

**A:** Akismet คือปลั๊กอิน Anti-spam สำหรับ WordPress ที่ทำงานแบบ cloud-based เมื่อมีคอมเมนต์ใหม่ Akismet จะส่งข้อมูลไปตรวจสอบกับเซิร์ฟเวอร์ที่มีฐานข้อมูล spam จากเว็บไซต์หลายล้านแห่ง ถ้าเป็น spam จะย้ายไป spam queue ถ้าเป็นของจริงจะปล่อยผ่าน

---

=== CARD 3 (Technical) ===

**Q:** API Key ของ Akismet คืออะไร? ขอได้ที่ไหน?

**A:** API Key คือรหัสเฉพาะที่ใช้เชื่อมต่อ Akismet กับเว็บไซต์ของเรา ขอได้ที่ akismet.com สำหรับเว็บส่วนบุคคลหรือบล็อกที่ไม่ได้ทำเงิน ขอฟรีได้โดยเลื่อน slider ราคาไปที่ 0 ต้องมีบัญชี WordPress.com

---

=== CARD 4 (Application) ===

**Q:** ขั้นตอนการตั้งค่า Akismet มีอะไรบ้าง?

**A:** มี 4 ขั้นตอน ได้แก่ (1) ไปที่ Plugins แล้ว Activate Akismet (มากับ WordPress อยู่แล้ว) (2) ขอ API Key ฟรีที่ akismet.com (3) ไปที่ Akismet Settings ใส่ API Key แล้วกด Connect (4) ตั้งค่าความเข้มงวดในการกรอง เลือกย้ายไป spam queue

---

=== CARD 5 (Explanation) ===

**Q:** ทำไมควรเลือกย้ายไป spam queue แทนที่จะลบ spam ทิ้งเลย?

**A:** เพราะบางครั้งอาจมี False Positive คือคอมเมนต์จริงที่ถูก Akismet จับว่าเป็น spam โดยผิดพลาด ถ้าลบทิ้งทันทีจะสูญเสียคอมเมนต์จริง แต่ถ้าย้ายไป spam queue เราสามารถเข้าไปตรวจสอบและกู้คืนคอมเมนต์จริงได้

---

=== CARD 6 (Definition) ===

**Q:** False Positive คืออะไรในบริบทของ Akismet?

**A:** False Positive คือคอมเมนต์ที่เป็นของจริง (ไม่ใช่ spam) แต่ถูก Akismet จับผิดว่าเป็น spam อาจเกิดจากคอมเมนต์ที่มีลิงก์หลายอัน มีคำที่คล้าย spam หรือมาจาก IP ที่เคยถูกรายงาน เมื่อเจอให้กด "Not Spam" เพื่อให้ Akismet เรียนรู้

---

=== CARD 7 (Best Practice) ===

**Q:** ควรตรวจสอบ spam queue บ่อยแค่ไหน? ทำอย่างไร?

**A:** ควรตรวจสอบ spam queue อย่างน้อยสัปดาห์ละ 1 ครั้ง โดยไปที่ Comments > Spam ใน WordPress Admin ดูรายการคอมเมนต์ที่ถูกจับ ถ้าเจอคอมเมนต์จริงให้กด "Not Spam" ถ้าแน่ใจว่าเป็น spam ทั้งหมดให้กด "Empty Spam" ล้างทิ้ง

---

=== CARD 8 (Explanation) ===

**Q:** ทำไมห้ามปิด Anti-spam เด็ดขาด แม้เว็บจะเล็ก?

**A:** เพราะ bot spam ไม่สนว่าเว็บใหญ่หรือเล็ก มันจะ spam ทุกเว็บที่เปิดคอมเมนต์ไว้ ถ้าปิด Anti-spam แม้แค่วันเดียวอาจได้ spam หลายร้อยอัน ต้องมานั่งลบทีหลังเสียเวลา และ spam ที่ค้างอยู่ส่งผลเสียต่อ SEO และความน่าเชื่อถือ

---

=== CARD 9 (Comparison) ===

**Q:** นอกจาก Akismet ยังมีทางเลือก Anti-spam อะไรอีก?

**A:** มี 2 ทางเลือกหลัก ได้แก่ (1) Antispam Bee — ฟรี 100% ไม่ต้อง API Key เป็น privacy-friendly ไม่ส่งข้อมูลไป cloud เหมาะกับเว็บที่ต้อง GDPR (2) CleanTalk — เสียเงิน แต่ฟีเจอร์เยอะกว่า ป้องกัน spam ทั้ง comment และ contact form

---

=== CARD 10 (Application) ===

**Q:** Akismet ทำงานร่วมกับอะไรได้นอกจาก Comment?

**A:** Akismet สามารถทำงานร่วมกับ Contact Form ได้ด้วย เช่น Contact Form 7, WPForms, Gravity Forms เพื่อกรอง spam submission จากฟอร์มติดต่อ ไม่ใช่แค่คอมเมนต์อย่างเดียว ช่วยป้องกัน spam ทุกช่องทางที่มีฟอร์มกรอกข้อมูล

---

=== CARD 11 (Technical) ===

**Q:** Akismet ฟรีกับเสียเงินต่างกันอย่างไร?

**A:** Akismet ฟรีสำหรับเว็บส่วนบุคคล/บล็อกไม่ทำเงิน จะมี credit link "Protected by Akismet" แสดง แพลนเสียเงินสำหรับเว็บธุรกิจ ไม่แสดง credit link ได้ priority support และกรอง spam ปริมาณสูงกว่า

---

=== CARD 12 (Summary) ===

**Q:** สรุปสิ่งสำคัญเกี่ยวกับ Akismet มีอะไรบ้าง?

**A:** (1) Comment spam อันตราย ต้องป้องกัน (2) Akismet ใช้ cloud-based AI กรอง spam แม่นเกือบ 100% (3) API Key ฟรีสำหรับเว็บส่วนบุคคล (4) ตั้งค่าย้ายไป spam queue อย่าลบทันที (5) ตรวจ False Positives สัปดาห์ละครั้ง (6) อย่าปิด Anti-spam เด็ดขาด

---

*จำนวน Flashcards ทั้งหมด: 12 ใบ*
