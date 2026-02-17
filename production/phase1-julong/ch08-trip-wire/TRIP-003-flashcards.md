# ทำความรู้จักระบบ Affiliate — TRIP-003
> **Format:** Flashcards (Q&A)
> **Source:** SWP3 Ch8 Trip Wire ตอนที่ 3
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## รวมแฟลชการ์ด (12 ใบ)

=== CARD 1 (Definition) ===
**Q:** Cookie Tracking ในระบบ Affiliate ทำงานอย่างไร?
**A:** เมื่อลูกค้าคลิกลิงก์ Affiliate ระบบจะฝัง Cookie ไว้ในเบราว์เซอร์ของลูกค้า Cookie นี้จะจดจำว่าลูกค้ามาจาก Affiliate คนไหน แม้จะปิดเบราว์เซอร์แล้วกลับมาซื้อทีหลัง Cookie ยังจำได้ (ตราบใดที่ยังไม่หมดอายุ)

=== CARD 2 (Technical) ===
**Q:** UTM Parameters คืออะไร และใช้งานอย่างไรในระบบ Affiliate?
**A:** UTM Parameters คือส่วนต่อท้ายของ URL ที่ใช้ระบุแหล่งที่มาของ Traffic เช่น ?utm_source=facebook&utm_medium=affiliate&utm_campaign=tripwire ช่วยให้วิเคราะห์ได้ว่า Traffic มาจากช่องทางไหน และ Campaign ใด

=== CARD 3 (Comparison) ===
**Q:** CPA, CPS และ Recurring Commission แตกต่างกันอย่างไร?
**A:** CPA (Cost Per Action) จ่ายเมื่อลูกค้าทำ action ที่กำหนด เช่น สมัครสมาชิก CPS (Cost Per Sale) จ่ายเมื่อเกิดการขายจริง เป็น % ของยอดขาย Recurring Commission จ่ายทุกรอบที่ลูกค้าต่ออายุ เช่น SaaS รายเดือน — ได้คอมมิชชันทุกเดือน

=== CARD 4 (Framework) ===
**Q:** Affiliate Ecosystem ประกอบด้วยผู้เล่นหลัก 4 ฝ่ายอะไรบ้าง?
**A:** 1) Merchant (ผู้ขาย) — เจ้าของสินค้า 2) Affiliate Network (ตัวกลาง) — แพลตฟอร์มเชื่อม Merchant กับ Affiliate 3) Affiliate (พันธมิตร) — ผู้โปรโมทสินค้า 4) Customer (ลูกค้า) — ผู้ซื้อสินค้า ทุกฝ่ายได้ประโยชน์ร่วมกัน (Win-Win)

=== CARD 5 (Benefit) ===
**Q:** ทำไม Recurring Commission ถึงน่าสนใจที่สุดสำหรับ Affiliate?
**A:** เพราะ Recurring Commission คือ Passive Income ตัวจริง ได้รับคอมมิชชันทุกเดือนตราบใดที่ลูกค้ายังเป็นสมาชิก เช่น แนะนำ SaaS รายเดือน ราคา $50 คอมมิชชัน 30% = $15/เดือน/ลูกค้า ถ้ามี 100 ลูกค้า = $1,500/เดือน โดยไม่ต้องขายเพิ่ม

=== CARD 6 (Platform) ===
**Q:** ClickBank ต่างจาก Amazon Associates อย่างไร?
**A:** ClickBank เน้นสินค้าดิจิทัล คอมมิชชันสูง 50-75% เหมาะสำหรับคอร์ส ebook ส่วน Amazon Associates มีสินค้าหลากหลายมาก แต่คอมมิชชันต่ำ 1-10% เหมาะสำหรับการรีวิวสินค้ากายภาพทุกประเภท

=== CARD 7 (Platform - Thai) ===
**Q:** แพลตฟอร์ม Affiliate ที่เหมาะกับตลาดไทยคืออะไร?
**A:** Shopee Affiliate Program และ Lazada Affiliate เป็นตัวเลือกหลักสำหรับตลาดไทย คอมมิชชัน 3-10% ข้อดีคือคนไทยคุ้นเคยกับทั้งสองแพลตฟอร์มอยู่แล้ว ซื้อง่าย จ่ายสะดวก Conversion Rate จึงสูง

=== CARD 8 (Ethics) ===
**Q:** Disclosure Requirements สำหรับ Affiliate คืออะไร?
**A:** Disclosure Requirements คือข้อกำหนดที่ Affiliate ต้องเปิดเผยสถานะของตัวเองทุกครั้งที่แนะนำสินค้าผ่านลิงก์ Affiliate เช่น "โพสต์นี้มีลิงก์ Affiliate หากซื้อผ่านลิงก์นี้ ผู้เขียนจะได้รับค่าคอมมิชชัน" เป็นทั้งข้อกำหนดทางจริยธรรมและกฎหมาย (FTC)

=== CARD 9 (Strategy) ===
**Q:** ควรเลือกแพลตฟอร์ม Affiliate อย่างไรให้เหมาะสม?
**A:** พิจารณา 4 ปัจจัย: 1) กลุ่มเป้าหมาย — คนไทย = Shopee/Lazada, สากล = Amazon/ClickBank 2) ประเภทสินค้า — ดิจิทัล = ClickBank, กายภาพ = Amazon/Shopee 3) อัตราคอมมิชชัน — สูง = ClickBank, ต่ำแต่ปริมาณเยอะ = Amazon 4) Cookie Duration — ยิ่งนาน ยิ่งดี

=== CARD 10 (Technical) ===
**Q:** Pixel Tracking คืออะไร และต่างจาก Cookie Tracking อย่างไร?
**A:** Pixel Tracking ใช้โค้ดเล็กๆ (1x1 pixel) ฝังในเว็บไซต์เพื่อติดตามพฤติกรรมลูกค้า เช่น การเข้าชม การซื้อ ต่างจาก Cookie ตรงที่ Pixel ทำงานฝั่ง Server ไม่ถูกบล็อกโดย Ad Blocker ง่ายเท่า Cookie และสามารถ track ข้ามอุปกรณ์ได้ดีกว่า

=== CARD 11 (Concept) ===
**Q:** อะไรคือประโยชน์หลัก 3 ข้อของการเป็น Affiliate?
**A:** 1) ต้นทุนต่ำ — ไม่ต้องสร้างสินค้า ไม่ต้องจัดการสต็อก/ส่งสินค้า/บริการหลังขาย 2) Scalable — โปรโมทได้หลายสินค้า หลายช่องทาง พร้อมกัน 3) Passive Income — โดยเฉพาะ Recurring Commission ที่สร้างรายได้ต่อเนื่องโดยไม่ต้องขายเพิ่ม

=== CARD 12 (Application) ===
**Q:** ถ้าต้องเลือกระหว่าง CPA กับ Recurring Commission สำหรับรายได้ระยะยาว ควรเลือกอะไร?
**A:** Recurring Commission ดีกว่าสำหรับรายได้ระยะยาว เพราะได้คอมมิชชันทุกรอบที่ลูกค้าต่ออายุ สร้าง Passive Income ที่ทบต้นได้ ในขณะที่ CPA จ่ายครั้งเดียวต่อ action แม้จะได้เงินเร็วกว่า แต่ต้องหาลูกค้าใหม่ตลอด

---

> **จำนวนแฟลชการ์ด:** 12 ใบ
> **ประเภท:** Definition 1 | Technical 2 | Comparison 2 | Framework 1 | Benefit 1 | Platform 2 | Ethics 1 | Strategy 1 | Application 1
