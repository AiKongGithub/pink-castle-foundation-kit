# ช่วงตอบคำถาม — YTCAMP-009 Executive Summary
> **Format:** Executive Summary
> **Source:** SWP3 Ch19 Youtube Ads Campaign ตอนที่ 9
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:23:21

---

## สรุปภาพรวม

บทเรียนนี้เป็นช่วง Q&A ตอบคำถามที่นักเรียนถามบ่อยที่สุดเกี่ยวกับ Youtube Ads Campaign ครอบคลุม 10 คำถามสำคัญ ตั้งแต่เรื่องงบประมาณสำหรับมือใหม่ ปัญหา Ad Disapproval การลด CPV ที่สูงเกินไป การแก้ปัญหา Conversion Tracking การเลือก Ad Format ที่เหมาะสม Remarketing Lists ความยาววิดีโอที่เหมาะสม กลยุทธ์แข่งขัน การตัดสินใจทำเองหรือจ้างเอเจนซี่ และวิธีวัดผลสำเร็จของ Campaign

---

## 10 คำถาม-คำตอบ (FAQ Table)

| # | คำถาม | คำตอบสั้น | คำแนะนำหลัก |
|---|-------|----------|-------------|
| 1 | งบน้อยเริ่มยังไง | เริ่มได้ที่ 300-500 บาท/วัน | ใช้ CPV Bidding + Remarketing + Campaign เดียวก่อน วิ่ง 7-14 วันแล้วค่อยขยาย |
| 2 | โฆษณาไม่ผ่านการอนุมัติ | ละเมิด Google Ads Policy | อ่าน Policy Violation ที่แจ้ง แก้ไขแล้วยื่น Appeal ภายใน 1-2 วัน |
| 3 | CPV สูงเกินไป | Targeting แคบ / Creative ไม่ดี / ช่วงแข่งขันสูง | ขยาย Targeting + ปรับปรุง 5 วินาทีแรก + A/B Test Audience |
| 4 | Conversion Tracking ไม่ทำงาน | Tag ไม่ Fire / ตั้งค่าผิด | ใช้ Google Tag Assistant ตรวจ + เช็ค Attribution Window |
| 5 | เลือก TrueView หรือ Bumper | ขึ้นอยู่กับเป้าหมาย | TrueView = Awareness/Consideration (CPV) / Bumper = Brand Recall (CPM) |
| 6 | Remarketing ต้องรอนานแค่ไหน | ต้องมีอย่างน้อย 100 Users | ทำ Prospecting Campaign คู่ไปก่อนระหว่างรอสะสม List |
| 7 | วิดีโอยาวแค่ไหนดี | 15-30 วินาที (Awareness) / 1-2 นาที (Consideration) | ทำ 2 Version แล้ว A/B Test / 5 วินาทีแรกสำคัญที่สุด |
| 8 | คู่แข่งยิง Ads เหมือนกัน | Creative Quality + Differentiation | Hook ใน 5 วินาที + Custom Intent Audiences Target คนค้นหาคู่แข่ง |
| 9 | ทำเองหรือจ้างเอเจนซี่ | ขึ้นอยู่กับงบและเวลา | งบ < 30K ทำเอง / งบ > 100K พิจารณาจ้าง / ต้องเข้าใจพื้นฐานเสมอ |
| 10 | วัดผลสำเร็จอย่างไร | ดู View Rate, CPV, CTR, ROAS | ROAS > 3x = คุ้มค่า / ROAS < 3x = ต้อง Optimize |

---

## Troubleshooting Guide

### ปัญหา: Ad Disapproval

| สาเหตุ | ตัวอย่าง | วิธีแก้ |
|--------|---------|--------|
| Misleading Content | "รวยใน 7 วัน" "การันตี 100%" | ลบคำโฆษณาเกินจริง ใช้ข้อความตามจริง |
| Trademark Issues | ใช้ชื่อแบรนด์คนอื่น | ลบชื่อแบรนด์ออก หรือขออนุญาตเป็นลายลักษณ์อักษร |
| Copyright | เพลง/ภาพมีลิขสิทธิ์ | ใช้เพลง/ภาพ Royalty-free หรือที่สร้างเอง |
| Prohibited Content | สุขภาพ/การเงินไม่มีเอกสาร | เตรียมเอกสารรับรองตาม Google Policy |

### ปัญหา: CPV สูงเกินไป

| สาเหตุ | สัญญาณ | วิธีแก้ |
|--------|--------|--------|
| Targeting แคบเกิน | Reach ต่ำ Impressions น้อย | ขยาย Audience / ลด Targeting Layers |
| Creative ไม่ดึงดูด | View Rate ต่ำกว่า 15% | ปรับปรุง 5 วินาทีแรกให้ดึงดูด |
| ช่วงแข่งขันสูง | CPV สูงขึ้นกะทันหัน | เลี่ยงช่วงเทศกาล / เพิ่ม Budget |
| Bidding ไม่เหมาะ | จ่ายเกินค่าเฉลี่ย | ลอง Manual CPV แทน Maximize |

### ปัญหา: Conversion Tracking ไม่ทำงาน

| จุดตรวจสอบ | เครื่องมือ | วิธีตรวจ |
|------------|-----------|---------|
| Google Tag ติดตั้งถูกหน้า | Google Tag Assistant | ดูว่า Tag Fire ในทุกหน้า |
| Conversion Action ถูกประเภท | Google Ads Dashboard | เช็คว่าเป็น Purchase/Sign-up/Lead ตรงเป้า |
| GTM Trigger ถูกต้อง | GTM Preview Mode | ทดสอบว่า Trigger Fire เมื่อเกิด Action |
| Attribution Window เหมาะสม | Conversion Settings | ปกติตั้ง 30 วัน อย่าตั้งสั้นเกินไป |

---

## เกณฑ์ตัดสินใจ: ทำเอง vs จ้างเอเจนซี่

| เกณฑ์ | ทำเอง | จ้างเอเจนซี่ |
|-------|-------|------------|
| งบโฆษณา/เดือน | < 30,000 บาท | > 100,000 บาท |
| เวลาที่มี | มีเวลาเรียนรู้ + Optimize | ไม่มีเวลาจัดการ |
| ความรู้ | เรียนจบ Course / เข้าใจพื้นฐาน | ไม่มีความรู้เลย |
| ข้อควรจำ | ยืดหยุ่นสูง ควบคุมได้ทุกอย่าง | ต้องเลือกเอเจนซี่ที่เชี่ยวชาญ Youtube Ads |
| งบ 30K-100K | ตัดสินตามเวลาและความรู้ | ตัดสินตามเวลาและความรู้ |

---

## KPI Benchmarks (ตลาดไทย)

| Metric | ค่าที่ดี | ค่าที่ต้อง Optimize | ความหมาย |
|--------|---------|-------------------|----------|
| View Rate | > 15% | < 15% | สัดส่วนคนดูจริง ต่อ Impressions |
| CPV | < 1 บาท | > 1 บาท | ต้นทุนต่อการดู 1 ครั้ง |
| CTR | > 0.5% | < 0.5% | อัตราคลิกต่อ Impressions |
| ROAS | > 3x | < 3x | ผลตอบแทนต่อเงินลงทุนโฆษณา |
| Remarketing List | > 100 Users | < 100 Users | จำนวนขั้นต่ำก่อนใช้ Remarketing |

---

## ตัวเลขสำคัญ

| Metric | ค่า |
|--------|-----|
| งบเริ่มต้นที่แนะนำ | 300-500 บาท/วัน |
| ระยะเวลาทดสอบ Campaign | 7-14 วัน |
| Remarketing List ขั้นต่ำ | 100 Users |
| ROAS เป้าหมาย | > 3x |
| งบที่ควรจ้างเอเจนซี่ | > 100,000 บาท/เดือน |
| 5 วินาทีแรก | สำคัญที่สุดสำหรับ Hook |
| Ad Disapproval Appeal | 1-2 วันทำการ |

---

*Word count: ~700 | Tables: 8 | Estimated read time: 5 minutes*

---

> ทบทวนต่อ: **YTCAMP-010** — ตรวจการบ้าน
> Series: SWP3 Ch19 Youtube Ads Campaign
> PinkCastle Academy © 2026
