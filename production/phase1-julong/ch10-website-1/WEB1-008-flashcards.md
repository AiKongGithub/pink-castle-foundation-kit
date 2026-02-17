# Flashcards: วิธีการติดตั้ง Plugin ตอนที่ 1 — WEB1-008
> **Format:** Flashcards (Q&A)
> **Source:** SWP3 Ch10 สร้างเว็บไซต์ Part 1 ตอนที่ 8
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

=== CARD 1 (Definition) ===

**Q:** WordPress Plugin คืออะไร?

**A:** Plugin คือส่วนเสริมหรือโปรแกรมเล็กๆ ที่ติดตั้งเพิ่มลงไปใน WordPress เพื่อเพิ่มความสามารถให้กับเว็บไซต์ เปรียบเสมือนแอปในมือถือ ปัจจุบันคลัง WordPress.org มี Plugin ให้เลือกมากกว่า 60,000 ตัว

---

=== CARD 2 (Process) ===

**Q:** ขั้นตอนการติดตั้ง Plugin จากคลัง WordPress มีอย่างไร?

**A:** (1) เข้าหน้า Admin → Plugins → Add New (2) พิมพ์ค้นหาชื่อ Plugin ในช่อง Search (3) กด Install Now รอการติดตั้ง (4) กด Activate เพื่อเปิดใช้งาน ง่ายเพียง 4 ขั้นตอน

---

=== CARD 3 (Evaluation) ===

**Q:** เกณฑ์ในการประเมินคุณภาพ Plugin ก่อนติดตั้งมีอะไรบ้าง?

**A:** ดูจาก 4 ปัจจัยหลัก ได้แก่ (1) Rating — คะแนนดาว (ควรได้ 4+ จาก 5) (2) Active Installations — จำนวนผู้ใช้งาน (3) Last Updated — วันอัปเดตล่าสุด (ไม่ควรเกิน 3-6 เดือน) (4) Tested up to — รองรับ WordPress เวอร์ชันล่าสุดหรือไม่

---

=== CARD 4 (Security) ===

**Q:** Plugin Security ที่แนะนำมีตัวไหนบ้าง? แต่ละตัวเด่นอะไร?

**A:** (1) Wordfence Security — เด่นด้าน Firewall, สแกนมัลแวร์, บล็อก IP ที่น่าสงสัย (2) iThemes Security — เด่นด้าน Brute Force Protection ป้องกันการเดารหัสผ่าน ควรเลือกติดตั้งเพียงตัวเดียว ไม่ควรลงทั้งสองตัวพร้อมกัน

---

=== CARD 5 (SEO) ===

**Q:** Yoast SEO กับ RankMath ต่างกันอย่างไร?

**A:** Yoast SEO มีผู้ใช้มากที่สุด เสถียร เหมาะกับมือใหม่ ส่วน RankMath เป็นตัวใหม่กว่า มีฟีเจอร์ฟรีมากกว่า (Schema Markup, Keyword Tracking ในเวอร์ชันฟรี) ทั้งสองตัวช่วยปรับแต่ง Title, Meta Description และ Sitemap

---

=== CARD 6 (Contact) ===

**Q:** WPForms ทำอะไรได้บ้าง? ทำไมต้องมี Contact Form Plugin?

**A:** WPForms เป็น Plugin สร้างฟอร์มแบบลากวาง (drag-and-drop) ใช้สร้างฟอร์มติดต่อ ฟอร์มสมัครสมาชิก แบบสอบถาม มีเทมเพลตให้เลือกเยอะ ต้องมีเพราะ Contact Form เป็นช่องทางสื่อสารพื้นฐานที่ทุกเว็บไซต์ธุรกิจต้องมี

---

=== CARD 7 (Analytics) ===

**Q:** Plugin Analytics ที่แนะนำมีอะไร? ทำหน้าที่อะไร?

**A:** MonsterInsights หรือ Site Kit by Google ทั้งสองช่วยเชื่อมต่อ Google Analytics กับ WordPress ทำให้ดูสถิติผู้เข้าชม (จำนวนคนเข้า แหล่งที่มา หน้าที่ดูบ่อย) ได้จากหน้า Dashboard ของ WordPress โดยตรง ไม่ต้องเข้า Google Analytics แยกต่างหาก

---

=== CARD 8 (Backup) ===

**Q:** ทำไม Backup Plugin ถึงสำคัญที่สุดตัวหนึ่ง? แนะนำตัวไหน?

**A:** เพราะถ้าเว็บถูกแฮก ข้อมูลหาย หรือทำอะไรผิดพลาด Backup เป็นทางเดียวที่จะกู้คืนได้ แนะนำ UpdraftPlus ซึ่งตั้งค่าสำรองอัตโนมัติได้ (รายวัน/รายสัปดาห์) และส่งไฟล์ไปเก็บที่ Google Drive หรือ Dropbox

---

=== CARD 9 (Warning) ===

**Q:** ทำไมไม่ควรติดตั้ง Plugin ที่ทำหน้าที่เดียวกันหลายตัว?

**A:** เพราะ Plugin ที่ทำหน้าที่ซ้ำกันอาจเกิด Conflict หรือขัดกัน ทำให้เว็บไซต์ทำงานผิดพลาด โหลดช้า หรืออาจล่มได้ เช่น ไม่ควรลง Wordfence พร้อม iThemes หรือ Yoast พร้อม RankMath ให้เลือกตัวเดียวในแต่ละประเภท

---

=== CARD 10 (Summary) ===

**Q:** Plugin 5 ประเภทที่ทุกเว็บไซต์ WordPress ต้องมีคืออะไรบ้าง?

**A:** (1) Security — ป้องกันแฮกเกอร์ (Wordfence/iThemes) (2) SEO — ขึ้นอันดับ Google (Yoast/RankMath) (3) Contact Form — ฟอร์มติดต่อ (WPForms) (4) Analytics — สถิติผู้เข้าชม (MonsterInsights/Site Kit) (5) Backup — สำรองข้อมูล (UpdraftPlus)

---

=== CARD 11 (Best Practice) ===

**Q:** เว็บไซต์ที่เพิ่งสร้างใหม่ ควรติดตั้ง Plugin เมื่อไร?

**A:** ควรติดตั้ง Plugin ทั้ง 5 ประเภทเป็นอันดับแรกก่อนเริ่มสร้างเนื้อหา โดยเฉพาะ Security Plugin และ Backup Plugin ที่ต้องเปิดใช้งานตั้งแต่วันแรกเพื่อป้องกันปัญหาตั้งแต่ต้น

---

=== CARD 12 (Concept) ===

**Q:** คำว่า "Brute Force Protection" ใน Security Plugin หมายถึงอะไร?

**A:** Brute Force Protection คือระบบป้องกันการพยายามเดารหัสผ่าน โดยแฮกเกอร์จะใช้โปรแกรมทดลองรหัสผ่านหลายพันหลายหมื่นครั้ง ระบบนี้จะบล็อก IP ที่พยายาม Login ผิดพลาดหลายครั้งติดต่อกัน

---

*จำนวน Flashcards ทั้งหมด: 12 ใบ*
