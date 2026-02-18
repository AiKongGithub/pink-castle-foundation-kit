# ตรวจสอบเมนูแคมเปญ — YTOPT-002
> **Format:** Executive Summary
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 2
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

## Executive Summary

### สรุปภาพรวม

การตรวจสอบเมนูแคมเปญเป็นทักษะพื้นฐานที่ผู้ลงโฆษณา Google Ads ทุกคนต้องเชี่ยวชาญ เมนูหลักใน Google Ads ประกอบด้วย Overview, Campaigns, Ad Groups, Ads, Keywords และ Audiences ซึ่งแต่ละเมนูแสดงข้อมูลในมุมมองที่ต่างกัน ผู้ลงโฆษณาต้องสามารถอ่านตัวเลขบน Campaign Dashboard ได้อย่างถูกต้อง ดูแนวโน้มและเปรียบเทียบช่วงเวลา ใช้ Filters กรองข้อมูลตามมิติต่างๆ ปรับแต่ง Columns ให้ตรงกับความต้องการ เข้าใจ Status Icons และใช้ Quick Actions จัดการแคมเปญได้อย่างรวดเร็ว

---

### Key Findings

1. **เมนูหลัก 6 ส่วนครอบคลุมทุกมุมมอง** — Overview (ภาพรวม), Campaigns (แคมเปญ), Ad Groups (กลุ่มโฆษณา), Ads (ชิ้นงาน), Keywords (คำค้นหา), Audiences (กลุ่มเป้าหมาย) ให้ข้อมูลครบถ้วนในการตัดสินใจ
2. **การดูแนวโน้มสำคัญกว่าตัวเลขวันเดียว** — ต้องเปรียบเทียบข้ามช่วงเวลา (Week vs Week, Month vs Month) เพื่อจับสัญญาณ Ad Fatigue หรือการเปลี่ยนแปลงของตลาด
3. **Filters & Segments เปิดเผยข้อมูลที่ซ่อนอยู่** — การกรองตาม Device, Network, Time, Location ช่วยระบุจุดที่ต้องปรับแต่งได้อย่างแม่นยำ
4. **Custom Views ประหยัดเวลาในระยะยาว** — สร้าง Quick Check View กับ Deep Analysis View บันทึกไว้ใช้ซ้ำ ไม่ต้องปรับคอลัมน์ใหม่ทุกครั้ง
5. **Quick Actions ช่วยจัดการเร็วขึ้น** — เปลี่ยน Budget, Pause/Enable, Edit Settings ได้จาก Dashboard โดยตรง ไม่ต้องเข้าไปในแคมเปญ

---

### ตารางเมนูหลักใน Google Ads

| เมนู | ข้อมูลที่แสดง | ใช้ดูอะไร | ความถี่ที่ควรเข้าดู |
|------|--------------|-----------|-------------------|
| Overview | สรุปทุกแคมเปญรวม | ภาพรวมประสิทธิภาพทั้งหมด | ทุกครั้งที่เปิด Google Ads |
| Campaigns | รายการแคมเปญ + Metrics | เปรียบเทียบแคมเปญแต่ละตัว | 2-3 ครั้ง/สัปดาห์ |
| Ad Groups | กลุ่มโฆษณาในแคมเปญ | ทดสอบกลุ่มเป้าหมายต่างๆ | เมื่อต้องการ Optimize |
| Ads | ชิ้นงานโฆษณาจริง | ดูว่า Ad ตัวไหนทำงานดี | เมื่อต้องการ A/B Test |
| Keywords | คำค้นหาที่ Trigger โฆษณา | ปรับ Keyword Strategy | สัปดาห์ละครั้ง |
| Audiences | กลุ่มเป้าหมายที่ตั้งไว้ | ดูว่ากลุ่มไหนตอบรับดี | เมื่อต้องการปรับ Targeting |

---

### ตาราง Filters & Segments ที่สำคัญ

| Filter/Segment | ข้อมูลที่ได้ | ประโยชน์ | ตัวอย่างการใช้ |
|----------------|-------------|---------|---------------|
| Device | Mobile vs Desktop vs Tablet | ปรับ Bid ตามอุปกรณ์ | Mobile CTR ดีกว่า → เพิ่ม Bid |
| Network | YouTube Search vs Videos vs Display | เลือก Network ที่ดีที่สุด | YouTube Videos View Rate สูง → เน้น |
| Time | ชั่วโมง/วัน/สัปดาห์ | ตั้ง Ad Schedule | คนดูเยอะ 18:00-22:00 → เน้นช่วงนี้ |
| Location | จังหวัด/ภูมิภาค | ปรับ Geo-Targeting | กรุงเทพ Convert ดี → เพิ่มงบ |

---

### Recommendations

1. **สร้าง 2 Custom Views ไว้ใช้ประจำ** — Quick Check (5 Metrics หลัก) สำหรับดูเร็ว กับ Deep Analysis (รวม Conversion Metrics, Quality Metrics) สำหรับวิเคราะห์ละเอียด บันทึกไว้ครั้งเดียวใช้ได้ตลอด

2. **ใช้ Date Range Comparison ทุกครั้ง** — อย่าดูตัวเลขวันเดียวเด็ดขาด เปรียบเทียบ This Week vs Last Week เป็นอย่างน้อย เพื่อจับแนวโน้มขึ้น-ลง

3. **กรองข้อมูลตาม Device เป็นอันดับแรก** — Mobile vs Desktop มักให้ผลลัพธ์ต่างกันมาก ข้อมูลนี้ช่วยตัดสินใจเรื่อง Bid Adjustment ได้ทันที

4. **ตรวจสอบ Status Icons ทุกครั้ง** — แคมเปญที่ Paused หรือ Limited อาจเสียโอกาสโดยไม่รู้ตัว สแกนสถานะทุกแคมเปญก่อนออกจาก Dashboard

5. **ใช้ Quick Actions แทนการเข้าแก้ในแคมเปญ** — การเปลี่ยน Budget, Pause/Enable สามารถทำจากหน้ารายการได้เลย ประหยัดเวลาและลดขั้นตอน

---

### บทสรุปสำหรับผู้บริหาร

การเข้าใจเมนูแคมเปญใน Google Ads เป็นพื้นฐานที่ขาดไม่ได้สำหรับการบริหารงบโฆษณาอย่างมีประสิทธิภาพ ผู้ที่สามารถนำทางเมนูได้คล่อง ใช้ Filters กรองข้อมูล และอ่านแนวโน้มได้ จะตัดสินใจเรื่อง Budget Allocation, Targeting Adjustment และ Campaign Optimization ได้เร็วและแม่นยำขึ้น ควรลงทุนเวลาตั้ง Custom Views และทำความเข้าใจแต่ละเมนูให้ถ่องแท้ตั้งแต่เริ่มต้น

---

> ทบทวนต่อ: **YTOPT-003** — ลิงก์ช่อง Youtube กับ Google Ads
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*Word count: ~600 | Reading time: 4 minutes*
