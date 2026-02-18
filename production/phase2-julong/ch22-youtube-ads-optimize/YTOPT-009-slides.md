# Set Conversion — YTOPT-009 Slides
> **Format:** Slide Outline
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 9
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:11:11

---

## SLIDE 1: หน้าปก (Title Slide)

- **Set Conversion — ตั้งค่า Conversion Tracking**
- SWP3 บทที่ 22: วิธีปรับแต่งแคมเปญ Youtube Ads — ตอนที่ 9
- PinkCastle Academy
- วันที่: 18 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- เข้าใจว่า Conversion คืออะไร ทำไมต้องตั้ง
- รู้จัก 4 ประเภท Conversion ใน Google Ads
- ตั้งค่า Conversion Action ขั้นตอนจริง
- เลือก Conversion Window ให้เหมาะกับธุรกิจ
- เข้าใจ Attribution Model 5 แบบ
- ติดตั้ง Conversion Tag ผ่าน GTM
- ตรวจสอบและแก้ไขปัญหา Conversion

---

## SLIDE 3: Conversion คืออะไร?

- **Conversion** = การกระทำที่เราต้องการให้ลูกค้าทำ
- เช่น กรอกฟอร์ม, ซื้อสินค้า, สมัครสมาชิก, โทรหาร้าน
- **ถ้าไม่ตั้ง Conversion Tracking:**
  - ไม่รู้ว่าโฆษณาได้ผลหรือไม่
  - ไม่สามารถ Optimize แคมเปญได้
  - เหมือนยิงปืนโดยไม่เห็นเป้า
- **ต้องตั้งก่อนเริ่มลงโฆษณาเสมอ**

---

## SLIDE 4: 4 ประเภท Conversion

| ประเภท | ตัวอย่าง | เหมาะกับ |
|--------|---------|----------|
| Website Actions | กรอกฟอร์ม, สั่งซื้อ, สมัครสมาชิก | ธุรกิจที่มี Landing Page |
| Phone Calls | โทรจากเบอร์ในโฆษณา | ธุรกิจบริการ, ร้านค้า |
| App Installs | ดาวน์โหลดแอปมือถือ | ธุรกิจที่มี Mobile App |
| Import (Offline) | ซื้อหน้าร้าน, ปิดดีล CRM | ธุรกิจ B2B, ร้านค้าปลีก |

- **ผู้ประกอบการไทยใช้บ่อยสุด:** Website Actions

---

## SLIDE 5: ขั้นตอนตั้ง Conversion ใน Google Ads

- เข้า **Google Ads** → เมนู **Tools**
- ไปที่ **Measurement** → **Conversions**
- คลิก **New Conversion Action**
- เลือกประเภท (Website / Phone / App / Import)
- กรอกข้อมูล:
  - **ชื่อ:** ตั้งให้สื่อความหมาย เช่น "Lead Form Submit"
  - **Category:** Lead, Purchase, Sign-up ฯลฯ
  - **Value:** มูลค่าต่อ Conversion (เช่น 500 บาท/Lead)
  - **Count:** Every หรือ One

---

## SLIDE 6: Count — Every vs One

| การตั้งค่า | นับอย่างไร | ตัวอย่าง | เหมาะกับ |
|-----------|-----------|---------|----------|
| **Every** | นับทุกครั้งที่เกิด Conversion | ลูกค้า 1 คนซื้อ 3 ครั้ง = 3 Conversions | E-commerce (ทุกรายการสั่งซื้อมีมูลค่า) |
| **One** | นับแค่ 1 ครั้งต่อคน | ลูกค้า 1 คนสมัคร 3 ครั้ง = 1 Conversion | Lead Generation (สนใจแค่ Lead ใหม่) |

- **เลือกผิด = ข้อมูลบิดเบือนทั้งระบบ**

---

## SLIDE 7: Conversion Window

- **คือ:** ระยะเวลาที่นับว่าเป็น Conversion หลังเห็น/คลิกโฆษณา
- **ตัวเลือก:** 7 วัน / 30 วัน / 60 วัน / 90 วัน
- **ค่าเริ่มต้น:** 30 วัน

| สินค้า/บริการ | Window แนะนำ | เหตุผล |
|-------------|-------------|--------|
| ของราคาถูก, Impulse buy | 7-14 วัน | ตัดสินใจเร็ว |
| คอร์สเรียน, SaaS | 30 วัน | ต้องศึกษาเปรียบเทียบ |
| อสังหาริมทรัพย์, รถยนต์ | 60-90 วัน | ตัดสินใจนาน มูลค่าสูง |

---

## SLIDE 8: Attribution Model — 5 แบบ

| Model | วิธีให้เครดิต | เมื่อไรใช้ |
|-------|-------------|----------|
| Last Click | เครดิตทั้งหมด → คลิกสุดท้าย | ผู้เริ่มต้น เข้าใจง่าย |
| First Click | เครดิตทั้งหมด → คลิกแรก | วัด Awareness channel |
| Linear | แบ่งเท่ากันทุกจุดสัมผัส | ดูภาพรวม Journey |
| Time Decay | เครดิตมากกว่า → จุดใกล้ Conversion | วัด Retargeting |
| Data-driven | Google ML วิเคราะห์ให้ | แม่นยำสุด (ต้องมีข้อมูลมากพอ) |

- **แนะนำ:** เริ่มจาก Last Click → เปลี่ยน Data-driven เมื่อมีข้อมูลมากพอ

---

## SLIDE 9: ติดตั้ง Conversion Tag

- **วิธีที่ 1: Google Tag Manager (แนะนำ)**
  - สร้าง Tag → Google Ads Conversion Tracking
  - ใส่ Conversion ID + Conversion Label
  - ตั้ง Trigger → Page View เฉพาะ Thank You Page
  - Preview → Publish

- **วิธีที่ 2: Global Site Tag**
  - วางโค้ด JavaScript ลงในเว็บไซต์โดยตรง
  - ต้องแก้โค้ดทุกครั้งที่เปลี่ยนแปลง

- **สำคัญ:** Tag ต้องอยู่บน **Thank You Page เท่านั้น**
- **ห้าม:** วางบนหน้าแรก หน้าสินค้า หรือหน้าอื่น

---

## SLIDE 10: Thank You Page — ตำแหน่งที่ถูกต้อง

```
ลูกค้าเห็นโฆษณา
    ↓
คลิกเข้า Landing Page
    ↓
กรอกฟอร์ม / สั่งซื้อ
    ↓
Thank You Page ← [Conversion Tag วางที่นี่]
    ↓
Google Ads นับ Conversion
```

- **ผิด:** วาง Tag บนหน้า Landing Page → ทุกคนที่เข้าถูกนับเป็น Conversion
- **ถูก:** วาง Tag บนหน้า Thank You → นับเฉพาะคนที่ทำ Action สำเร็จ

---

## SLIDE 11: ตรวจสอบสถานะ Conversion

| สถานะ | ความหมาย | สิ่งที่ต้องทำ |
|-------|---------|-------------|
| Recording | ทำงานปกติ กำลังบันทึก | ไม่ต้องทำอะไร ปล่อยทำงานต่อ |
| No Recent Conversions | Tag ถูกต้อง แต่ยังไม่มี Conversion | รอลูกค้าทำ Action หรือทำ Test Conversion |
| Inactive | มีปัญหา Tag ไม่ทำงาน | ตรวจสอบและแก้ไขทันที |

- **ถ้า Inactive ตรวจสอบ 4 จุด:**
  1. Tag วางถูกหน้าหรือไม่
  2. Google Tag Assistant ตรวจผ่านหรือไม่
  3. ทำ Test Conversion ด้วยตัวเอง
  4. Conversion ID / Label ตรงกันหรือไม่

---

## SLIDE 12: สรุปและก้าวต่อไป (Summary & Next Steps)

- **6 ขั้นตอนตั้ง Conversion:**
  1. เข้าใจว่า Conversion คืออะไร → กำหนดเป้าหมาย
  2. เลือกประเภท → Website / Phone / App / Import
  3. ตั้งค่า → ชื่อ, Category, Value, Count
  4. เลือก Window + Attribution Model
  5. ติดตั้ง Tag → GTM บน Thank You Page
  6. ตรวจสอบ → สถานะต้องเป็น Recording
- **หลักคิด:** ตั้ง Conversion ก่อนเริ่มโฆษณาเสมอ
- **ขั้นตอนถัดไป:** ตอนที่ 10 Google กับ Kartra ทำงานร่วมกัน

---

> ทบทวนต่อ: **YTOPT-010** — Google กับ Kartra ทำงานร่วมกัน
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
