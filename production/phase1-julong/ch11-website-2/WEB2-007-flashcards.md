# Flashcards: วิธีการปรับแต่ง Comment Social Media — WEB2-007
> **Format:** Flashcards (Q&A)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 7
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

=== CARD 1 (Comparison) ===

**Q:** ระบบ Comment ใน WordPress มีกี่ทางเลือก? แต่ละแบบต่างกันอย่างไร?

**A:** มี 3 ทางเลือกหลัก ได้แก่ (1) WordPress Comment — ระบบในตัว ข้อมูลอยู่กับเรา ฟรี (2) Disqus — ระบบภายนอก moderation ดี รองรับ Social Login แต่ข้อมูลอยู่ที่ Disqus (3) Facebook Comments — คอมเมนต์ด้วย Facebook ง่าย แต่ข้อมูลอยู่ที่ Facebook

---

=== CARD 2 (Definition) ===

**Q:** Comment Moderation คืออะไร? ทำไมต้องเปิดใช้?

**A:** Comment Moderation คือการกลั่นกรองคอมเมนต์ก่อนแสดงบนเว็บไซต์ ต้องเปิดใช้เพราะถ้าไม่กรอง จะมี spam comments เข้ามาเต็ม ทั้งลิงก์โฆษณา ลิงก์อันตราย และเนื้อหาไม่เหมาะสม ส่งผลเสียต่อภาพลักษณ์และ SEO ตั้งค่าได้ที่ Settings > Discussion

---

=== CARD 3 (Concept) ===

**Q:** Akismet คืออะไร? ทำหน้าที่อะไร?

**A:** Akismet คือปลั๊กอิน Anti-spam ที่มาพร้อม WordPress ทำหน้าที่กรอง spam comments อัตโนมัติด้วยระบบ cloud-based มีประสิทธิภาพสูงมาก กรองได้ถูกต้องเกือบ 100% ฟรีสำหรับเว็บไซต์ส่วนบุคคล

---

=== CARD 4 (Application) ===

**Q:** Social Sharing Buttons สำหรับเว็บไซต์ในประเทศไทยควรเลือกแพลตฟอร์มใดบ้าง?

**A:** สำหรับประเทศไทยควรมีอย่างน้อย 3 แพลตฟอร์ม ได้แก่ Facebook (ผู้ใช้มากที่สุดในไทย), LINE (คนไทยใช้สื่อสารหลัก), Twitter (สำหรับข่าวและเทรนด์) เพิ่มเติมได้ตามกลุ่มเป้าหมาย เช่น LinkedIn สำหรับคนทำงาน หรือ Pinterest สำหรับเว็บเน้นภาพ

---

=== CARD 5 (Definition) ===

**Q:** Open Graph Meta Tags คืออะไร? ทำไมสำคัญ?

**A:** Open Graph Meta Tags คือโค้ดที่กำหนดว่าเมื่อมีคนแชร์ลิงก์เว็บเราไป Social Media จะแสดงรูปภาพ หัวข้อ และคำอธิบายอะไร ถ้าไม่ตั้งค่า Social Media จะดึงข้อมูลแบบสุ่ม อาจแสดงรูปผิดหรือข้อความไม่เหมาะสม ใช้ปลั๊กอิน Yoast SEO หรือ Rank Math จัดการอัตโนมัติ

---

=== CARD 6 (Explanation) ===

**Q:** Social Follow Buttons ต่างจาก Social Sharing Buttons อย่างไร?

**A:** Social Sharing Buttons คือปุ่มให้ผู้อ่าน "แชร์" บทความของเราไป Social Media ส่วน Social Follow Buttons คือปุ่มให้ผู้อ่าน "ติดตาม" Social Media ของเรา (เช่น Follow Facebook Page, Subscribe YouTube) Sharing ใช้เพิ่ม reach ส่วน Follow ใช้เพิ่มจำนวนผู้ติดตาม

---

=== CARD 7 (Technical) ===

**Q:** Auto-posting คืออะไร? ใช้เครื่องมืออะไรได้บ้าง?

**A:** Auto-posting คือการแชร์บทความใหม่ไปยัง Social Media อัตโนมัติเมื่อ publish ไม่ต้องเข้าไปแชร์เอง เครื่องมือที่ใช้ได้ เช่น (1) Jetpack — ปลั๊กอิน WordPress มีฟีเจอร์นี้ในตัว (2) IFTTT — เชื่อมต่อ WordPress กับ Social Media (3) Zapier — เครื่องมือ automation ที่ยืดหยุ่นกว่า

---

=== CARD 8 (Concept) ===

**Q:** Social Login สำหรับ Comment คืออะไร? มีข้อดีอย่างไร?

**A:** Social Login คือให้ผู้อ่านล็อกอินด้วยบัญชี Social Media (Facebook, Google, Twitter) เพื่อคอมเมนต์ในเว็บ ข้อดีคือ (1) ไม่ต้องสมัครสมาชิกใหม่ (2) คอมเมนต์ได้ง่ายขึ้น (3) ลดจำนวน spam เพราะใช้บัญชีจริง (4) เพิ่ม engagement อย่างมาก

---

=== CARD 9 (Best Practice) ===

**Q:** ปลั๊กอินอะไรช่วยจัดการ Open Graph Meta Tags ได้อัตโนมัติ?

**A:** ปลั๊กอิน SEO ที่ช่วยจัดการ Open Graph ได้แก่ (1) Yoast SEO — ปลั๊กอิน SEO ยอดนิยมอันดับ 1 (2) Rank Math — ปลั๊กอิน SEO ที่มีฟีเจอร์ครบกว่า ทั้งสองตัวจะสร้าง OG tags อัตโนมัติจาก Featured Image และ Meta Description ที่เราตั้งไว้

---

=== CARD 10 (Application) ===

**Q:** ปุ่ม Social Follow Buttons ควรวางไว้ตำแหน่งใดบนเว็บไซต์?

**A:** ตำแหน่งที่เหมาะสมมี 3 จุด ได้แก่ (1) Sidebar — ด้านข้างของบทความ มองเห็นได้ตลอดขณะอ่าน (2) Footer — ท้ายเว็บไซต์ แสดงทุกหน้า (3) About Page — หน้าเกี่ยวกับเรา ที่คนอยากติดตามมากที่สุด

---

=== CARD 11 (Explanation) ===

**Q:** ทำไมการสร้างชุมชน (Community) รอบเว็บไซต์ถึงสำคัญ?

**A:** เพราะชุมชนสร้าง engagement ที่ยั่งยืน เมื่อคนอ่าน คอมเมนต์ แชร์ ติดตาม จะเกิดความผูกพันกับเว็บ ทำให้ (1) กลับมาเยี่ยมชมซ้ำ (2) เพิ่ม Traffic แบบ organic (3) สร้าง brand loyalty (4) ได้ feedback จากผู้อ่าน (5) เพิ่มโอกาสทางธุรกิจ

---

=== CARD 12 (Summary) ===

**Q:** สรุปการตั้งค่า Comment และ Social Media Integration มีกี่ส่วนหลัก?

**A:** มี 7 ส่วนหลัก ได้แก่ (1) ระบบ Comment (WordPress/Disqus/Facebook) (2) Comment Moderation (3) Anti-spam ด้วย Akismet (4) Social Sharing Buttons (5) Open Graph Meta Tags (6) Social Follow Buttons + Auto-posting (7) Social Login สำหรับคอมเมนต์

---

*จำนวน Flashcards ทั้งหมด: 12 ใบ*
