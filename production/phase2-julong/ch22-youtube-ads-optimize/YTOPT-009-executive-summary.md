# Set Conversion — YTOPT-009 Executive Summary
> **Format:** Executive Summary
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 9
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:11:11

---

## Executive Summary

### สรุปภาพรวม

การตั้ง Conversion Tracking เป็นขั้นตอนพื้นฐานที่สำคัญที่สุดในการวัดผลแคมเปญ YouTube Ads เพราะถ้าไม่มี Conversion Tracking เราจะไม่รู้เลยว่าโฆษณาที่ลงไปนำไปสู่ผลลัพธ์ทางธุรกิจจริงหรือไม่ Conversion คือการกระทำที่ต้องการให้ลูกค้าทำ เช่น กรอกฟอร์ม ซื้อสินค้า สมัครสมาชิก โดย Google Ads แบ่ง Conversion เป็น 4 ประเภท ได้แก่ Website, Phone Calls, App Installs และ Import (Offline) การตั้งค่าต้องครอบคลุมทั้ง Conversion Window, Attribution Model, การติดตั้ง Conversion Tag บน Thank You Page และการตรวจสอบสถานะให้เป็น Recording เพื่อยืนยันว่าทุกอย่างทำงานถูกต้อง

---

### Key Findings

1. **Conversion = การกระทำที่ต้องการวัดผล** — ทุกธุรกิจต้องกำหนดให้ชัดว่า "สำเร็จ" คือเมื่อลูกค้าทำอะไร เช่น กรอกฟอร์ม Lead, สั่งซื้อสินค้า, สมัครสมาชิก, โทรหาร้าน
2. **4 ประเภท Conversion** — Website Actions (กรอกฟอร์ม/ซื้อ), Phone Calls (โทรจากโฆษณา), App Installs (ติดตั้งแอป), Import (Offline Conversions) ผู้ประกอบการไทยส่วนใหญ่ใช้ Website Actions
3. **Conversion Window กำหนดระยะเวลานับ** — ตั้งได้ 7, 30, 60 หรือ 90 วัน สินค้าตัดสินใจเร็วใช้ 7 วัน สินค้าราคาสูงอาจใช้ 60-90 วัน ค่าเริ่มต้นคือ 30 วัน
4. **Attribution Model กำหนดเครดิต** — Last Click, First Click, Linear, Time Decay, Data-driven แต่ละแบบให้เครดิตกับจุดสัมผัสต่างกัน ผู้เริ่มต้นแนะนำ Last Click
5. **Conversion Tag ต้องอยู่บน Thank You Page** — ติดตั้งผ่าน GTM หรือ Global Site Tag วางเฉพาะหน้ายืนยัน ห้ามวางบนหน้าแรกหรือหน้าสินค้า
6. **ตรวจสอบสถานะ 3 แบบ** — Recording (ปกติ), No Recent Conversions (ยังไม่มีข้อมูล), Inactive (มีปัญหา ต้องแก้ไข)

---

### ตาราง 4 ประเภท Conversion ใน Google Ads

| ประเภท | ตัวอย่าง | Count ที่แนะนำ | เหมาะกับ |
|--------|---------|---------------|----------|
| Website Actions | กรอกฟอร์ม, สั่งซื้อ, สมัครสมาชิก | One (Lead) / Every (E-com) | ธุรกิจที่มีเว็บไซต์/Landing Page |
| Phone Calls | โทรจากเบอร์ในโฆษณา | One | ธุรกิจบริการ, ร้านค้า |
| App Installs | ดาวน์โหลดแอป | One | ธุรกิจที่มี Mobile App |
| Import (Offline) | ซื้อที่หน้าร้าน, ปิดดีล CRM | Every | ธุรกิจ B2B, ร้านค้าปลีก |

---

### ตาราง Attribution Model 5 แบบ

| Model | วิธีให้เครดิต | ข้อดี | เหมาะกับ |
|-------|-------------|-------|----------|
| Last Click | ให้เครดิตทั้งหมดกับคลิกสุดท้าย | เข้าใจง่าย วัดผลตรง | ผู้เริ่มต้น |
| First Click | ให้เครดิตทั้งหมดกับคลิกแรก | รู้ว่าช่องทางไหนสร้าง Awareness | แคมเปญ Awareness |
| Linear | แบ่งเครดิตเท่ากันทุกจุดสัมผัส | เห็นภาพรวม Customer Journey | วิเคราะห์ Multi-channel |
| Time Decay | เครดิตมากกว่าที่จุดใกล้ Conversion | สะท้อนจุดที่มีผลต่อการตัดสินใจ | แคมเปญ Retargeting |
| Data-driven | Google ML วิเคราะห์ให้อัตโนมัติ | แม่นยำที่สุด | บัญชีที่มีข้อมูลมากพอ |

---

### Recommendations

1. **ตั้ง Conversion ก่อนเริ่มแคมเปญ** — อย่าลงโฆษณาก่อนตั้ง Conversion Tracking เพราะจะไม่มีข้อมูลวัดผล เสียงบโดยไม่รู้ว่าได้ผลหรือไม่

2. **เลือก Count ให้ตรงกับเป้าหมาย** — Lead Generation ใช้ One (นับ 1 ครั้งต่อคน) E-commerce ใช้ Every (นับทุกครั้งที่ซื้อ) การเลือกผิดทำให้ข้อมูลบิดเบือน

3. **ตั้ง Conversion Window ตามพฤติกรรมลูกค้า** — สินค้าราคาถูกตัดสินใจเร็ว ใช้ 7-14 วัน สินค้าราคาสูงใช้ 30-90 วัน ถ้าไม่แน่ใจ เริ่มที่ 30 วัน

4. **ติดตั้ง Tag ผ่าน Google Tag Manager** — ง่ายกว่าวางโค้ดตรง จัดการ Tag หลายตัวได้สะดวก แก้ไขได้โดยไม่ต้องแก้โค้ดเว็บ

5. **ตรวจสอบสถานะหลังติดตั้ง** — ทำ Test Conversion ด้วยตัวเอง ใช้ Google Tag Assistant ตรวจว่า Tag ยิงถูกต้อง ต้องเห็นสถานะ Recording จึงจะมั่นใจ

---

### บทสรุปสำหรับผู้บริหาร

การตั้ง Conversion Tracking เป็นเรื่องแรกที่ต้องทำก่อนลงโฆษณา เพราะเป็นตัวชี้วัดว่าเงินที่ลงไปได้ผลลัพธ์กลับมาจริงหรือไม่ หากไม่มี Conversion Tracking เท่ากับลงโฆษณาแบบตาบอด ไม่รู้ว่าโฆษณาชุดไหนนำลูกค้ามา ช่องทางไหนคุ้มค่า การตั้งค่าที่ถูกต้องตั้งแต่ Conversion Type, Window, Attribution Model ไปจนถึง Tag Installation จะทำให้ Google Ads Optimize แคมเปญให้อัตโนมัติ ลดค่าใช้จ่ายต่อ Conversion และเพิ่ม ROI ได้ในระยะยาว

---

> ทบทวนต่อ: **YTOPT-010** — Google กับ Kartra ทำงานร่วมกัน
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*Word count: ~650 | Reading time: 4 minutes*
