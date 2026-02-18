# Google กับ Kartra ทำงานร่วมกัน — YTOPT-010 Flashcards
> **Format:** Flashcards
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 10
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:06:52

---

=== CARD 1 ===
Q: ทำไมต้องเชื่อม Google Ads กับ Kartra?
A: เพื่อวัด Conversion จริง ว่าคนที่คลิกโฆษณามากรอกฟอร์มหรือซื้อสินค้าจริงหรือไม่ ถ้าไม่เชื่อม Google Ads จะเห็นแค่ Clicks แต่ไม่รู้ผลลัพธ์ที่เกิดขึ้นบน Kartra ทำให้ Optimize แคมเปญไม่ได้

=== CARD 2 ===
Q: ใส่ Google Tag ใน Kartra ได้อย่างไร?
A: เข้า Kartra → เลือกหน้า Page ที่ต้องการ → คลิก Page Settings → หาส่วน Tracking Code → วาง Google Tag ในช่อง Header จากนั้นบันทึก

=== CARD 3 ===
Q: Conversion Tracking Flow เมื่อเชื่อม Google กับ Kartra มีขั้นตอนอย่างไร?
A: คนดูโฆษณา → คลิก → เข้า Kartra Landing Page → กรอกฟอร์ม/ซื้อสินค้า → ไปถึง Thank You Page (มี Conversion Tag) → Google Ads บันทึก Conversion ถ้าขาดขั้นตอนใดข้อมูลจะหาย

=== CARD 4 ===
Q: Google Tag ที่ต้องใส่ใน Kartra มี 2 ส่วนคืออะไร?
A: 1) Global Site Tag — วางทุกหน้าที่เกี่ยวข้อง เป็น Tag หลักสำหรับติดตามผู้เยี่ยมชม 2) Event Snippet — วางเฉพาะ Thank You Page เป็น Tag ที่บอก Google ว่าเกิด Conversion แล้ว

=== CARD 5 ===
Q: Global Site Tag กับ Google Tag Manager (GTM) ต่างกันอย่างไร?
A: Global Site Tag = วางโค้ดลง Kartra โดยตรง ง่าย เหมาะมือใหม่ที่มี Tag 1-2 ตัว GTM = วาง Container Code ครั้งเดียว จัดการ Tag ทั้งหมดผ่าน Dashboard ยืดหยุ่นกว่า เหมาะคนใช้หลายแพลตฟอร์มโฆษณา

=== CARD 6 ===
Q: ข้อดีของ Google Tag Manager เมื่อเทียบกับ Global Site Tag มีอะไรบ้าง?
A: 1) จัดการหลาย Tag จากที่เดียว (Google, Facebook, TikTok) 2) แก้ไขได้โดยไม่ต้องแก้โค้ดใน Kartra 3) มี Version Control ย้อนกลับได้ 4) มี Preview Mode ตรวจสอบก่อน Publish

=== CARD 7 ===
Q: ตรวจสอบว่า Google Tag ทำงานถูกต้องบน Kartra ได้อย่างไร?
A: ใช้ Google Tag Assistant ซึ่งเป็น Chrome Extension ฟรี ติดตั้งแล้วเข้าไปที่ Kartra Landing Page จะแสดงว่ามี Tag อะไรติดอยู่ ยิงถูกต้องหรือไม่ เครื่องหมายถูกสีเขียว = ทำงานถูกต้อง

=== CARD 8 ===
Q: ถ้า Google Tag บน Kartra ไม่ทำงาน ควรตรวจสอบอะไร?
A: 1) ตรวจว่าวาง Tag ในส่วน Header ของ Kartra Page Settings ถูกต้อง 2) ตรวจว่า Thank You Page มี Event Snippet 3) ใช้ Tag Assistant ตรวจสอบ 4) ดูสถานะ Conversion ใน Google Ads ว่าเป็น Recording หรือ Inactive

=== CARD 9 ===
Q: ข้อดี 3 ประการหลักของการเชื่อม Google Ads กับ Kartra คืออะไร?
A: 1) ข้อมูล Conversion แม่นยำ — รู้จริงว่าคนจากโฆษณากรอกฟอร์ม/ซื้อกี่คน 2) Optimize Campaign ได้ดีขึ้น — มีข้อมูลจริงให้ปรับปรุง 3) ใช้ Smart Bidding ได้ — Google ปรับราคาประมูลอัตโนมัติตาม Conversion data

=== CARD 10 ===
Q: Smart Bidding ทำงานอย่างไรเมื่อเชื่อม Google กับ Kartra?
A: เมื่อ Google Ads ได้รับข้อมูล Conversion จาก Kartra ระบบ Smart Bidding จะใช้ Machine Learning วิเคราะห์ว่ากลุ่มคนไหนมีแนวโน้ม Convert สูง แล้วปรับราคาประมูลให้อัตโนมัติ เน้นแสดงโฆษณาให้กลุ่มเป้าหมายที่มีโอกาสสูง ลดค่าใช้จ่ายต่อ Conversion

---

> ทบทวนต่อ: **YTOPT-012** — ลงโฆษณา Google Ads ตอนที่ 2
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*Flashcard count: 10 | Level: Intermediate*
