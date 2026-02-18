# วิธีปรับแต่งแคมเปญ Advance ตอน 1 — YTOPT-014 Slides
> **Format:** Slide Outline
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 14
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:50:18

---

## SLIDE 1: หน้าปก (Title Slide)

- **วิธีปรับแต่งแคมเปญ Advance ตอน 1 — 7 เทคนิคเชิงลึก**
- SWP3 บทที่ 22: วิธีปรับแต่งแคมเปญ Youtube Ads — ตอนที่ 14
- PinkCastle Academy
- วันที่: 18 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- เมื่อไหร่ควรปรับแคมเปญ — กฎ 7 วัน
- วิเคราะห์ข้อมูลเชิงลึก — 3 Metrics + 3 Dimensions
- ปรับ Bidding Strategy — Manual CPC สู่ Target CPA
- ปรับ Audience — ขยาย ตัด สร้าง Similar
- ปรับ Ad Creative — A/B Testing + Responsive Ads
- Device Optimization — ปรับ Bid ตาม Device
- Schedule Optimization — ปรับเวลาแสดงโฆษณา

---

## SLIDE 3: เมื่อไหร่ควรปรับแคมเปญ?

- **กฎเหล็ก:** รออย่างน้อย 7 วันก่อนปรับ
- ข้อมูลน้อยกว่า 7 วัน = ไม่ Reliable
- การปรับเร็วเกินไป = ขุดต้นไม้ดูรากทุกวัน
- **หลักการ:**
  - ยังไม่มีข้อมูล 7 วัน → อย่าปรับ
  - มีข้อมูลแล้วแต่ไม่แน่ใจ → รอเพิ่ม
  - ยิ่งมีข้อมูลเยอะ → ยิ่งตัดสินใจแม่นยำ

---

## SLIDE 4: วิเคราะห์ข้อมูลเชิงลึก — 3 Metrics หลัก

| Metric | คืออะไร | บอกอะไร |
|--------|--------|---------|
| Conversion Rate | อัตราที่คนทำสิ่งที่เราต้องการ | โฆษณา/Landing Page ดีไหม |
| Cost per Conversion | ต้นทุนต่อ 1 Conversion | จ่ายแพงเกินไปไหม |
| ROAS | Return on Ad Spend | ได้คุ้มค่าลงทุนไหม |

- **อย่าดูแค่ Views กับ CTR อย่างเดียว!**

---

## SLIDE 5: เจาะลึกตาม 3 Dimensions

| Dimension | ดูอะไร | Tab ใน Google Ads |
|-----------|--------|------------------|
| Ad Group | กลุ่มไหนดี vs ไม่ดี | "Ad Groups" |
| Audience | Segment ไหนตอบสนองดี | "Audiences" |
| Device | Mobile vs Desktop vs Tablet | "Devices" |

- ภาพรวมอาจดูดี แต่ซ่อนปัญหาไว้
- Ad Group A: ROAS 5x + Ad Group B: ROAS 0.5x = ค่าเฉลี่ยดูพอได้
- **ต้องเจาะลึกจึงจะเห็นจุดที่ต้องปรับ**

---

## SLIDE 6: ปรับ Bidding Strategy

```
Manual CPC (เริ่มต้น)
    ↓ มี 30-50 Conversions ใน 30 วัน
Target CPA (ตั้ง = ค่าปัจจุบัน)
    ↓ ระบบทำงานได้ดี
ค่อยๆ ลด CPA 10-15% ต่อสัปดาห์
    ↓ Volume ลด?
เพิ่ม CPA กลับ (อย่ากดจนระบบทำงานไม่ได้)
```

- **ยังไม่ถึง 30 Conversions → อย่าเพิ่งเปลี่ยน!**
- Machine Learning ต้องมีข้อมูลเพียงพอ

---

## SLIDE 7: ปรับ Audience — 3 Actions

| Action | ทำกับ Audience | วิธีทำ |
|--------|---------------|--------|
| ขยาย | Segment ที่ Conversion Rate สูง | สร้าง Ad Group ใหม่เจาะกลุ่มนี้ เพิ่มงบ |
| Exclude | Segment ที่ 0 Conversions หลัง 14 วัน | ตัดออกไม่ให้เสียเงิน |
| สร้างใหม่ | Similar Audiences | Remarketing List → "Similar to" |

- **Similar Audiences** = Lookalike Audience ของ Facebook
- ให้ Google หาคนลักษณะคล้ายคนที่ Converted แล้ว

---

## SLIDE 8: ปรับ Ad Creative — A/B Testing

- **กฎ A/B Testing:**
  1. สร้าง 2 Ad Variants ใน Ad Group เดียวกัน
  2. ต่างกันแค่ 1 อย่าง (Headline / CTA / วิดีโอ)
  3. รอ 2 สัปดาห์ดูผลลัพธ์
  4. ปิดตัวที่แพ้ สร้าง Variant ใหม่ทดสอบต่อ

- **ทำไมต้องเปลี่ยนแค่ 1 อย่าง?**
  - ถ้าเปลี่ยนหลายอย่าง → ไม่รู้ว่าอะไรทำให้ดีขึ้น/แย่ลง
  - ต้องควบคุมตัวแปรเหมือนการทดลองวิทยาศาสตร์

---

## SLIDE 9: Responsive Ads

- ใส่ Headlines 3-5 ตัว + Description 2-3 ตัว
- Google Machine Learning ผสมคอมบิเนชันให้อัตโนมัติ
- ระบบเรียนรู้ว่า:
  - กลุ่มคน A ชอบ Headline 2 + Description 1
  - กลุ่มคน B ชอบ Headline 4 + Description 3
- **ดู Asset Performance Report** เพื่อเช็คว่าตัวไหนทำงานได้ดี

---

## SLIDE 10: Device Optimization

| Device | Traffic ในไทย | Conversion Rate | แนวโน้ม |
|--------|-------------|-----------------|---------|
| Mobile | สูงสุด | ต่ำกว่า Desktop | Research บน Mobile |
| Desktop | ปานกลาง | สูงกว่า Mobile | Convert บน Desktop |
| Tablet | ต่ำสุด | แตกต่างกันไป | ดูข้อมูลจริง |

- **Bid Adjustment:**
  - Desktop Conversion Rate สูง → เพิ่ม Bid +20-30%
  - Mobile Performance ต่ำ → ลด Bid -10-20%
- ไปที่ Tab "Devices" ใน Google Ads

---

## SLIDE 11: Schedule Optimization

- **ดู Performance ตาม:**
  - วันในสัปดาห์ (Day of Week)
  - ช่วงเวลาของวัน (Hour of Day)

- **ตัวอย่าง:**
  - จันทร์-ศุกร์ 12:00-14:00 → CTR สูงสุด
  - เสาร์-อาทิตย์ เช้า → Conversion Rate ดีที่สุด
  - ตี 2-5 → ไม่มีใครสนใจ

- **การปรับ:**
  - เพิ่ม Bid ช่วงเวลาทอง
  - ลด/หยุดแสดงช่วงที่ไม่ดี
  - **ประหยัดงบได้ 20-30%**

---

## SLIDE 12: สรุปและก้าวต่อไป (Summary & Next Steps)

- **7 เทคนิค Advanced Optimization:**
  1. รอ 7 วันก่อนปรับ — อย่าเร็วเกินไป
  2. วิเคราะห์ Conversion Rate, Cost per Conversion, ROAS
  3. เปลี่ยน Bidding → Target CPA เมื่อ 30-50 Conversions
  4. ปรับ Audience — ขยายดี / ตัดไม่ดี / สร้าง Similar
  5. A/B Testing — เปลี่ยนแค่ 1 อย่าง รอ 2 สัปดาห์
  6. Device Optimization — ปรับ Bid ตาม Device
  7. Schedule Optimization — ประหยัดงบ 20-30%
- **ขั้นตอนถัดไป:** ตอนที่ 15 Advance ตอน 2 — Budget Optimization, Remarketing, Scaling

---

> ทบทวนต่อ: **YTOPT-015** — วิธีปรับแต่งแคมเปญ Advance ตอน 2
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
