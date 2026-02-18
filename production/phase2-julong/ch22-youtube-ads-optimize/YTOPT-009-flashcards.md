# Set Conversion — YTOPT-009 Flashcards
> **Format:** Flashcards
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 9
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:11:11

---

=== CARD 1 ===
Q: Conversion ใน Google Ads คืออะไร?
A: คือการกระทำที่เราต้องการให้ลูกค้าทำหลังจากเห็นโฆษณา เช่น กรอกฟอร์ม ซื้อสินค้า สมัครสมาชิก โทรหาร้าน หรือดาวน์โหลดแอป ใช้เป็นตัวชี้วัดว่าโฆษณาได้ผลลัพธ์จริงหรือไม่

=== CARD 2 ===
Q: Conversion ใน Google Ads แบ่งเป็นกี่ประเภท อะไรบ้าง?
A: แบ่งเป็น 4 ประเภท คือ 1) Website Actions (กรอกฟอร์ม/สั่งซื้อ/สมัคร) 2) Phone Calls (โทรจากเบอร์ในโฆษณา) 3) App Installs (ดาวน์โหลดแอป) 4) Import/Offline (ซื้อที่หน้าร้าน/ปิดดีล CRM)

=== CARD 3 ===
Q: ตั้ง Conversion ใน Google Ads ได้อย่างไร?
A: เข้า Google Ads → เมนู Tools → Measurement → Conversions → คลิก New Conversion Action → เลือกประเภท (Website/Phone/App/Import) → ตั้งชื่อ, Category, Value, Count → ติดตั้ง Tag

=== CARD 4 ===
Q: Count แบบ Every กับ One ต่างกันอย่างไร?
A: Every = นับทุกครั้งที่เกิด Conversion เหมาะกับ E-commerce (ลูกค้าคนเดียวซื้อหลายครั้ง) One = นับแค่ 1 ครั้งต่อคน เหมาะกับ Lead Generation (สนใจแค่ว่าสมัครหรือยัง)

=== CARD 5 ===
Q: Conversion Window คืออะไร มีตัวเลือกอะไรบ้าง?
A: คือระยะเวลาที่จะนับว่าเป็น Conversion หลังจากเห็นหรือคลิกโฆษณา ตัวเลือกมี 7 วัน, 30 วัน, 60 วัน และ 90 วัน ค่าเริ่มต้นคือ 30 วัน เลือกตามพฤติกรรมการตัดสินใจของลูกค้า

=== CARD 6 ===
Q: ควรเลือก Conversion Window กี่วันสำหรับสินค้าราคาถูกกับสินค้าราคาสูง?
A: สินค้าราคาถูก ตัดสินใจเร็ว → 7-14 วัน สินค้าราคาสูง ต้องใช้เวลาตัดสินใจ → 30-90 วัน ถ้าไม่แน่ใจ เริ่มที่ 30 วัน (ค่าเริ่มต้น)

=== CARD 7 ===
Q: Attribution Model มีกี่แบบหลักๆ อะไรบ้าง?
A: มี 5 แบบ คือ 1) Last Click — เครดิตทั้งหมดให้คลิกสุดท้าย 2) First Click — เครดิตให้คลิกแรก 3) Linear — แบ่งเท่ากันทุกจุดสัมผัส 4) Time Decay — เครดิตมากกว่าที่จุดใกล้ Conversion 5) Data-driven — Google ML วิเคราะห์ให้

=== CARD 8 ===
Q: Attribution Model แบบไหนแนะนำสำหรับผู้เริ่มต้น และแบบไหนแม่นยำที่สุด?
A: ผู้เริ่มต้น → Last Click เพราะเข้าใจง่ายที่สุด แม่นยำที่สุด → Data-driven เพราะ Google ใช้ Machine Learning วิเคราะห์ว่าจุดสัมผัสไหนมีผลต่อ Conversion จริงๆ (ต้องมีข้อมูลมากพอ)

=== CARD 9 ===
Q: Conversion Tag ติดตั้งได้กี่วิธี และต้องวางที่หน้าไหน?
A: ติดตั้งได้ 2 วิธี คือ 1) Google Tag Manager (แนะนำ — จัดการง่าย ไม่ต้องแก้โค้ดเว็บตรง) 2) Global Site Tag (วางโค้ดในเว็บโดยตรง) ต้องวางบน Thank You Page หรือหน้ายืนยันเท่านั้น ห้ามวางบนหน้าแรกหรือหน้าสินค้า

=== CARD 10 ===
Q: ติดตั้ง Conversion Tag ผ่าน Google Tag Manager ทำอย่างไร?
A: สร้าง Tag ใหม่ → เลือก Google Ads Conversion Tracking → ใส่ Conversion ID และ Conversion Label จาก Google Ads → ตั้ง Trigger เป็น Page View เฉพาะ Thank You Page URL (เช่น /thank-you)

=== CARD 11 ===
Q: สถานะ Conversion ใน Google Ads มีกี่แบบ อะไรบ้าง?
A: มี 3 สถานะ คือ 1) Recording — ทำงานปกติ กำลังบันทึกข้อมูล 2) No Recent Conversions — Tag ติดตั้งถูกต้องแต่ยังไม่มี Conversion เกิดขึ้น 3) Inactive — มีปัญหา Tag อาจไม่ทำงาน ต้องตรวจสอบแก้ไข

=== CARD 12 ===
Q: ถ้า Conversion สถานะเป็น Inactive ต้องตรวจสอบอะไรบ้าง?
A: 1) ตรวจว่า Tag วางถูกหน้าหรือไม่ (ต้องเป็น Thank You Page) 2) ใช้ Google Tag Assistant ตรวจว่า Tag ยิงถูกต้อง 3) ทำ Test Conversion ด้วยตัวเอง 4) ตรวจว่า Conversion ID และ Label ตรงกับที่ตั้งใน Google Ads

---

> ทบทวนต่อ: **YTOPT-010** — Google กับ Kartra ทำงานร่วมกัน
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*Flashcard count: 12 | Level: Intermediate*
