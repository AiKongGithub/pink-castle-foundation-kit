# Flashcards: วิธีการตั้งค่าต่างๆ ของ WordPress — WEB2-001
> **Format:** Flashcards (Q&A)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 1
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

=== CARD 1 (Concept) ===

**Q:** WordPress Settings มีกี่หมวดหลัก และมีอะไรบ้าง?

**A:** มี 6 หมวดหลัก ได้แก่ (1) General — ตั้งค่าทั่วไป (2) Writing — ตั้งค่าการเขียน (3) Reading — ตั้งค่าการอ่าน (4) Discussion — ตั้งค่าคอมเมนต์ (5) Media — ตั้งค่ารูปภาพ (6) Permalinks — ตั้งค่าโครงสร้าง URL

---

=== CARD 2 (Detail) ===

**Q:** General Settings มีการตั้งค่าอะไรบ้างที่สำคัญ?

**A:** มี 5 รายการหลัก ได้แก่ Site Title (ชื่อเว็บไซต์), Tagline (คำอธิบายสั้น), Timezone (เขตเวลา), Date Format (รูปแบบวันที่), และ Site Language (ภาษาของเว็บไซต์) โดย Site Title และ Tagline จะแสดงในผลการค้นหาของ Google ด้วย

---

=== CARD 3 (Practical) ===

**Q:** สำหรับเว็บไซต์ภาษาไทย ควรตั้ง Timezone เป็นอะไร?

**A:** ควรตั้งเป็น Bangkok หรือ UTC+7 เพื่อให้เวลาที่แสดงในบทความตรงกับเวลาจริงในประเทศไทย หากตั้งผิด เวลาที่แสดงจะเพี้ยน ดูไม่เป็นมืออาชีพ

---

=== CARD 4 (Concept) ===

**Q:** Reading Settings มีตัวเลือกหน้าแรกกี่แบบ อะไรบ้าง?

**A:** มี 2 แบบ คือ (1) Your latest posts — แสดงบทความล่าสุดเป็นหน้าแรก เหมาะกับเว็บบล็อก (2) A static page — กำหนดหน้าเฉพาะเป็นหน้าแรก เหมาะกับเว็บธุรกิจที่ต้องการ Landing Page

---

=== CARD 5 (Warning) ===

**Q:** Search Engine Visibility ใน Reading Settings คืออะไร และต้องระวังอะไร?

**A:** คือตัวเลือกที่กำหนดว่าจะให้ Google เข้ามาจัดอันดับเว็บไซต์หรือไม่ หากติ๊ก "Discourage search engines from indexing this site" Google จะไม่จัดอันดับเว็บเราเลย ตอนสร้างเว็บอาจเปิดไว้ได้ แต่เมื่อเว็บพร้อมต้องเอาออกทันที

---

=== CARD 6 (Detail) ===

**Q:** Writing Settings มีการตั้งค่าสำคัญอะไรบ้าง?

**A:** มี 2 รายการหลัก คือ (1) Default Post Category — หมวดหมู่เริ่มต้นที่ระบบจะจัดให้โดยอัตโนมัติหากเราลืมเลือก (2) Post Format — รูปแบบของบทความ ส่วนใหญ่ใช้ Standard เป็นค่าเริ่มต้น

---

=== CARD 7 (Practical) ===

**Q:** ทำไมควรเปิด Comment Moderation ใน Discussion Settings?

**A:** เพราะเว็บไซต์จะได้รับคอมเมนต์สแปมจำนวนมาก การเปิด Comment Moderation ทำให้ต้องอนุมัติคอมเมนต์ก่อนจะแสดงบนหน้าเว็บ ช่วยป้องกันสแปมและเนื้อหาที่ไม่เหมาะสมค่ะ

---

=== CARD 8 (Detail) ===

**Q:** WordPress สร้างรูปภาพกี่ขนาดเมื่ออัปโหลด และแต่ละขนาดเท่าไร?

**A:** สร้าง 3 ขนาด คือ (1) Thumbnail — 150x150 พิกเซล (2) Medium — 300x300 พิกเซล (3) Large — 1024x1024 พิกเซล นอกจากไฟล์ต้นฉบับแล้ว WordPress จะสร้างสำเนา 3 ขนาดนี้โดยอัตโนมัติ

---

=== CARD 9 (Critical) ===

**Q:** Permalink Settings แนะนำให้เลือกรูปแบบไหน เพราะอะไร?

**A:** แนะนำ Post name เพราะได้ URL ที่สะอาด อ่านง่าย เช่น yoursite.com/how-to-setup-wordpress ทั้ง Google และผู้อ่านเข้าใจว่าหน้านี้เกี่ยวกับอะไร ส่งผลดีต่อ SEO โดยตรง ต่างจาก Plain ที่ได้ URL แบบ ?p=123 ซึ่งอ่านไม่รู้เรื่อง

---

=== CARD 10 (Warning) ===

**Q:** ทำไมต้องตั้ง Permalink ตั้งแต่วันแรก?

**A:** เพราะถ้าเปลี่ยน Permalink หลังจากมีบทความจำนวนมาก ลิงก์เก่าทั้งหมดจะใช้งานไม่ได้ ส่งผลให้ผู้ที่บันทึกลิงก์ไว้เข้าไม่ถึง Google ที่จัดอันดับไว้จะเจอหน้า 404 และต้องทำ Redirect ซึ่งยุ่งยากมาก

---

=== CARD 11 (Comparison) ===

**Q:** เปรียบเทียบ Permalink แบบ Plain กับ Post name ต่างกันอย่างไร?

**A:** Plain ได้ URL แบบ yoursite.com/?p=123 ซึ่งไม่มีความหมาย อ่านไม่รู้เรื่อง ไม่ดีต่อ SEO ส่วน Post name ได้ URL แบบ yoursite.com/your-post-title ซึ่งอ่านเข้าใจง่าย สื่อความหมาย และเป็นมิตรกับ SEO

---

=== CARD 12 (Checklist) ===

**Q:** หลังติดตั้ง WordPress เสร็จ ควรตั้งค่าอะไรก่อนเป็นลำดับแรก?

**A:** ลำดับที่ 1: Permalink เป็น Post name (สำคัญที่สุด เปลี่ยนทีหลังยาก) ลำดับที่ 2: Timezone เป็น Bangkok/UTC+7 ลำดับที่ 3: Site Title และ Tagline ลำดับที่ 4: เปิด Comment Moderation ลำดับที่ 5: ตรวจสอบ Search Engine Visibility

---

*จำนวน Flashcards ทั้งหมด: 12 ใบ*
