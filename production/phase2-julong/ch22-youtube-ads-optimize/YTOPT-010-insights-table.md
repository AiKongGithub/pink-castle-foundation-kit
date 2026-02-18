# Google กับ Kartra ทำงานร่วมกัน — YTOPT-010 Insights Table
> **Format:** Insights Table
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 10
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:06:52

---

## ตาราง 10 Insights สำคัญ

| # | Insight | Detail | Application | Impact Level |
|---|---------|--------|-------------|--------------|
| 1 | ไม่เชื่อม Google กับ Kartra = ข้อมูลหายครึ่ง | Google Ads เห็นแค่ Clicks แต่ไม่รู้ว่าคนที่คลิกมากรอกฟอร์มหรือซื้อจริงหรือไม่ เหมือนแจกใบปลิวแต่ไม่รู้ว่าใครมาซื้อของ | ติดตั้ง Google Tag บน Kartra ทุกหน้าที่เกี่ยวข้องกับแคมเปญก่อนเริ่มลงโฆษณา ห้ามลงโฆษณาก่อนเชื่อม | สูงมาก |
| 2 | Kartra Page Settings คือจุดใส่ Tag | เข้า Kartra → เลือก Page → Page Settings → Tracking Code → วาง Google Tag ในส่วน Header ไม่ต้องแก้โค้ดเว็บตรง | ใส่ Tag ทั้ง Landing Page (Global Site Tag) และ Thank You Page (Event Snippet) ตรวจสอบทุกหน้าที่ต้องการ Track | สูงมาก |
| 3 | Conversion Flow มี 5 ขั้นตอน ขาดขั้นใดข้อมูลหาย | คนดูโฆษณา → คลิก → Kartra Landing Page → กรอกฟอร์ม/ซื้อ → Thank You Page (มี Tag) → Google บันทึก ถ้าขาด Tag บน Thank You Page จะไม่มี Conversion เลย | ตรวจสอบ Flow ทั้งหมดตั้งแต่โฆษณาถึง Thank You Page ทำ Test Conversion ด้วยตัวเองเพื่อยืนยันว่าทุกขั้นตอนทำงาน | สูงมาก |
| 4 | Global Site Tag ง่ายสำหรับมือใหม่ | วางโค้ดลง Kartra โดยตรง ไม่ต้องเรียนรู้เครื่องมือเพิ่ม เหมาะกับคนที่มี Tag แค่ 1-2 ตัว เช่น Google Ads อย่างเดียว | ถ้าใช้แค่ Google Ads เลือก Global Site Tag เพราะตั้งค่าเสร็จภายใน 5 นาที ไม่ต้องสร้าง GTM Account | สูง |
| 5 | GTM ยืดหยุ่นกว่าสำหรับหลายแพลตฟอร์ม | วาง GTM Container Code ครั้งเดียว จัดการ Tag ทั้งหมดผ่าน Dashboard ทั้ง Google Ads, Facebook Pixel, TikTok Pixel มี Version Control และ Preview Mode | ถ้าใช้โฆษณามากกว่า 1 แพลตฟอร์ม เลือก GTM ตั้งแต่แรก เพราะไม่ต้องกลับไปแก้ Code ใน Kartra ทุกครั้งที่เพิ่ม Tag | สูง |
| 6 | Google Tag Assistant คือเครื่องมือตรวจสอบฟรี | Chrome Extension ที่ตรวจว่า Tag ติดตั้งถูกต้อง ยิงข้อมูลกลับไปที่ Google Ads ได้จริง เครื่องหมายสีเขียว = ปกติ สีแดง = มีปัญหา | ติดตั้ง Tag Assistant ไว้ใน Chrome ตรวจสอบทุกครั้งหลังใส่ Tag ใน Kartra และหลังทุกครั้งที่แก้ไข Page | สูง |
| 7 | Smart Bidding ต้องมี Conversion Data จึงทำงานได้ | Smart Bidding ใช้ Machine Learning ปรับราคาประมูลอัตโนมัติ แต่ต้องมีข้อมูล Conversion เพียงพอจึงจะวิเคราะห์ได้แม่นยำ ยิ่งมีข้อมูลมาก ยิ่ง Optimize ดี | เชื่อม Google กับ Kartra ให้เร็วที่สุด สะสม Conversion Data แล้วเปิด Smart Bidding เมื่อมี Conversion 15-30 ครั้งใน 30 วัน | ปานกลาง-สูง |
| 8 | Thank You Page คือจุดวาง Conversion Tag | Event Snippet ต้องอยู่บน Thank You Page เท่านั้น ไม่ใช่ Landing Page ถ้าวางผิดหน้าจะนับ Conversion ทุกคนที่เข้าหน้านั้น ข้อมูลบิดเบือนทั้งระบบ | สร้าง Thank You Page แยกชัดเจนใน Kartra ใส่ Event Snippet เฉพาะหน้านี้ ตรวจสอบว่าฟอร์ม Redirect ไปถูกหน้า | ปานกลาง-สูง |
| 9 | การเชื่อมใช้เวลาไม่ถึง 15 นาที | ขั้นตอนทั้งหมดตั้งแต่สร้าง Conversion Action ใน Google Ads คัดลอก Tag วางใน Kartra และตรวจสอบ ใช้เวลาไม่นาน แต่ผลลัพธ์มหาศาล | อย่าผัดวันประกันพรุ่ง ทำทันทีเมื่อสร้าง Kartra Page เสร็จ ก่อนเริ่มลงโฆษณาจริง | ปานกลาง-สูง |
| 10 | ข้อมูล Conversion ช่วยตัดสินใจหยุดโฆษณาที่ไม่ได้ผล | เมื่อมีข้อมูล Conversion จะเห็นชัดว่าโฆษณาชุดไหนได้ Conversion โฆษณาชุดไหนไม่ได้ สามารถหยุดชุดที่ไม่ได้ผลและเพิ่มงบให้ชุดที่ดี | ตรวจสอบ Conversion ระดับ Ad Group และ Ad ทุกสัปดาห์ หยุดโฆษณาที่ Cost per Conversion สูงเกินไป เพิ่มงบให้โฆษณาที่ Convert ดี | ปานกลาง |

---

### สรุป Impact Level

| Level | จำนวน Insights |
|-------|---------------|
| สูงมาก | 3 |
| สูง | 3 |
| ปานกลาง-สูง | 3 |
| ปานกลาง | 1 |

---

> ทบทวนต่อ: **YTOPT-012** — ลงโฆษณา Google Ads ตอนที่ 2
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*Insights count: 10 | Focus: Google Ads + Kartra Integration & Conversion Tracking*
