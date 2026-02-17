# แนะนำระบบ Sequence ใน Kartra — CLONE-010 Flashcards
> **Format:** Flashcards (Q&A)
> **Source:** SWP3 Ch20 Cloning Sale Funnel Kartra ตอนที่ 10
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:10:21

---

=== CARD 1 (Concept) ===

**Q:** Sequence ใน Kartra คืออะไร และทำหน้าที่อะไรใน Email Marketing?

**A:** Sequence คือชุดอีเมลอัตโนมัติที่ส่งตามลำดับและเวลาที่กำหนดไว้ล่วงหน้า เป็นหัวใจของ Email Marketing Automation ทำหน้าที่เปลี่ยน Lead ให้กลายเป็นลูกค้าโดยสร้างความสัมพันธ์ ให้ความรู้ และเสนอขายอัตโนมัติ ไม่ต้องนั่งส่งอีเมลเองทีละฉบับ

---

=== CARD 2 (Type) ===

**Q:** Sequence มีกี่ประเภท อะไรบ้าง?

**A:** มี 3 ประเภท คือ (1) Time-based ส่งตามวัน/เวลาที่กำหนด เช่น Day 0 Day 1 Day 3 เข้าใจง่ายที่สุด (2) Event-based ส่งเมื่อเกิดเหตุการณ์ เช่น ลูกค้าคลิกลิงก์ Personalize ได้มาก (3) Conditional ส่งตามเงื่อนไข เช่น เปิด/ไม่เปิดอีเมล แยกเส้นทางให้ลูกค้าแต่ละคน

---

=== CARD 3 (Component) ===

**Q:** องค์ประกอบ (Node) ใน Sequence มีกี่ประเภท อะไรบ้าง?

**A:** มี 4 ประเภท คือ (1) Email Node ตัวอีเมลที่ส่งออกไป มีหัวข้อ เนื้อหา CTA (2) Delay Node กำหนดระยะเวลารอก่อนส่งฉบับถัดไป (3) Condition Node แยกเส้นทางตามพฤติกรรมลูกค้า (4) Action Node ทำ Action เช่น ติด Tag ย้ายกลุ่ม Subscribe เข้า Sequence อื่น

---

=== CARD 4 (Time-based) ===

**Q:** Time-based Sequence ทำงานอย่างไร และเหมาะกับใคร?

**A:** ส่งอีเมลตามวัน/เวลาที่กำหนดล่วงหน้า เช่น Day 0 ส่งทันที Day 1 ส่งวันถัดไป Day 3 ส่งอีก 3 วัน เป็นประเภทที่ใช้มากที่สุดเพราะเข้าใจง่ายและวางแผนได้ล่วงหน้า เหมาะสำหรับผู้เริ่มต้นและ Welcome Sequence

---

=== CARD 5 (How-to) ===

**Q:** วิธีสร้าง Sequence ใน Kartra ทำอย่างไร?

**A:** ไปที่เมนู Communications > Sequences กด New Sequence ตั้งชื่อให้สื่อ จากนั้นใช้ Visual Builder ลาก Email Node มาวาง เขียนอีเมล แล้วลาก Delay Node มาต่อกำหนดเวลารอ ลาก Email Node ฉบับต่อไปมาต่อ ถ้าต้องการแยกทางก็ใส่ Condition Node ทำซ้ำจนครบ

---

=== CARD 6 (Welcome) ===

**Q:** Welcome Sequence มาตรฐาน 5 ฉบับ ส่งวันไหนและเนื้อหาอะไรบ้าง?

**A:** Email 1 Day 0 ต้อนรับและส่ง Lead Magnet ทันที Email 2 Day 1 ให้คุณค่าความรู้ยังไม่ขาย Email 3 Day 3 เสนอขายพร้อม Social Proof Email 4 Day 5 Follow-up ตอบ FAQ แก้ข้อโต้แย้ง Email 5 Day 7 Last Chance สร้าง Urgency ปิดการขาย

---

=== CARD 7 (Delay) ===

**Q:** Delay Node สำคัญอย่างไร และควรตั้งระยะห่างเท่าไร?

**A:** Delay Node กำหนดระยะเวลารอก่อนส่งอีเมลฉบับถัดไป สำคัญมากเพราะถ้าส่งถี่เกินไปลูกค้าจะรำคาญจนกด Unsubscribe ถ้าห่างเกินไปลูกค้าจะลืม สำหรับ Welcome Sequence แนะนำ Day 0 1 3 5 7 คือเริ่มถี่แล้วค่อยห่างออก

---

=== CARD 8 (Funnel) ===

**Q:** Sequence เชื่อมกับ Funnel อย่างไร?

**A:** เมื่อลูกค้ากรอกฟอร์มบน Capture Page จะตั้ง Trigger ให้ Subscribe ลูกค้าเข้า Sequence ที่สร้างไว้ ทั้งหมดอัตโนมัติ ลูกค้าสมัครปุ๊บ Email 1 ของ Sequence ก็ส่งออกไปทันที จากนั้น Delay Node จะนับเวลาส่งฉบับถัดไปตามที่กำหนด

---

=== CARD 9 (Condition) ===

**Q:** Condition Node ใช้ทำอะไร และตัวอย่างการใช้งาน?

**A:** Condition Node ใช้แยกเส้นทางตามพฤติกรรมลูกค้า เช่น ถ้าลูกค้าเปิดอีเมลก่อนหน้า ส่งอีเมลเสนอขายต่อ (ทาง A) แต่ถ้าไม่เปิด ส่งอีเมลหัวข้อใหม่ดึงดูดใจกว่า (ทาง B) ทำให้ Sequence ฉลาดขึ้น ลูกค้าแต่ละคนได้รับประสบการณ์ที่เหมาะสม

---

=== CARD 10 (Metric) ===

**Q:** 4 Metrics ที่ต้องติดตามในการวัดผล Sequence คืออะไร?

**A:** (1) Open Rate วัดว่าลูกค้าเปิดอีเมลกี่% ถ้าต่ำกว่า 20% ปรับ Subject Line (2) Click Rate วัดว่าคลิกลิงก์กี่% ถ้าต่ำปรับเนื้อหาและ CTA (3) Unsubscribe Rate ถ้าสูงกว่า 2% ส่งถี่เกินหรือเนื้อหาไม่ตรง (4) Conversion Rate วัดเป้าหมายสุดท้ายว่ากี่%ซื้อสินค้า

---

=== CARD 11 (Action Node) ===

**Q:** Action Node ทำอะไรได้บ้าง และต่างจาก Email Node อย่างไร?

**A:** Action Node ไม่ได้ส่งอีเมล แต่ทำ Action อื่นๆ ในระบบ เช่น ติด Tag ให้ลูกค้าเพื่อจัดกลุ่ม ย้ายลูกค้าไปกลุ่มอื่น Subscribe ลูกค้าเข้า Sequence อื่น แจ้งเตือนทีมงาน ทำให้ระบบ Automation ทำงานเชื่อมโยงกันทั้งหมดโดยอัตโนมัติ

---

=== CARD 12 (Best Practice) ===

**Q:** เคล็ดลับสำคัญในการสร้าง Sequence ที่มีประสิทธิภาพคืออะไร?

**A:** (1) เริ่มจาก Welcome Sequence 5 ฉบับเป็นพื้นฐาน (2) Email แรกต้องส่งทันที Day 0 อย่าให้รอ (3) ให้คุณค่าก่อนเสนอขาย (4) ใช้ Delay ห่างพอดี ไม่ถี่ไม่ห่างเกิน (5) ติดตาม 4 Metrics ทุกสัปดาห์แล้วปรับปรุง (6) เชื่อม Trigger กับ Capture Page ให้ถูกต้อง

---

*จำนวน Flashcards ทั้งหมด: 12 ใบ*

---

> ทบทวนต่อ: **CLONE-011** — ตรวจการบ้าน
> Series: SWP3 Ch20 Cloning Sale Funnel Kartra
> PinkCastle Academy © 2026
