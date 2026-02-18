# Google กับ Kartra ทำงานร่วมกัน — YTOPT-010 Slides
> **Format:** Slide Outline
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 10
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:06:52

---

## SLIDE 1: หน้าปก (Title Slide)

- **Google กับ Kartra ทำงานร่วมกัน**
- SWP3 บทที่ 22: วิธีปรับแต่งแคมเปญ Youtube Ads — ตอนที่ 10
- PinkCastle Academy
- วันที่: 18 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- เข้าใจว่าทำไมต้องเชื่อม Google Ads กับ Kartra
- วิธีใส่ Google Tag ใน Kartra Page Settings
- Conversion Tracking Flow 5 ขั้นตอน
- เปรียบเทียบ Global Site Tag กับ Google Tag Manager
- ตรวจสอบ Tag ด้วย Google Tag Assistant
- ข้อดี 6 ประการของการเชื่อมระบบ

---

## SLIDE 3: ทำไมต้องเชื่อม Google Ads กับ Kartra?

- **ปัญหา:** ลงโฆษณา Google Ads → ส่งคนไป Kartra Landing Page → ไม่รู้ผลลัพธ์
- Google Ads เห็นแค่ **Clicks** แต่ไม่เห็น **Conversions**
- **เปรียบเทียบ:** เหมือนแจกใบปลิวแต่ไม่นับว่าใครมาซื้อจริง
- **คำตอบ:** ใส่ Google Tag ใน Kartra เพื่อวัด Conversion จริง
- ต้องรู้ว่าคนคลิกโฆษณาแล้ว **กรอกฟอร์ม** หรือ **ซื้อจริง** หรือไม่

---

## SLIDE 4: วิธีใส่ Google Tag ใน Kartra

- **ขั้นตอนใน Kartra:**
  1. เข้าหน้า Page ที่ต้องการ
  2. คลิก **Page Settings**
  3. หาส่วน **Tracking Code**
  4. วาง Google Tag ในช่อง **Header**
  5. บันทึก

- **Tag จาก Google Ads มี 2 ส่วน:**
  - **Global Site Tag** → วางทุกหน้าที่เกี่ยวข้อง
  - **Event Snippet** → วางเฉพาะ Thank You Page

---

## SLIDE 5: Conversion Tracking Flow

```
คนดูโฆษณา (YouTube / Google Search)
    ↓
คลิกโฆษณา
    ↓
Kartra Landing Page (มี Global Site Tag)
    ↓
กรอกฟอร์ม / ซื้อสินค้า
    ↓
Thank You Page (มี Event Snippet) ← [Conversion ถูกบันทึกที่นี่]
    ↓
Google Ads รับข้อมูล Conversion
```

- **สำคัญ:** ถ้าขาดขั้นตอนใดขั้นตอนหนึ่ง → Conversion จะไม่ถูกบันทึก
- **จุดพลาดบ่อย:** ลืมใส่ Tag บน Thank You Page

---

## SLIDE 6: Global Site Tag vs Google Tag Manager

| หัวข้อ | Global Site Tag | Google Tag Manager |
|--------|----------------|-------------------|
| ความง่าย | ง่ายมาก วางโค้ดตรง | ต้องเรียนรู้เพิ่มเล็กน้อย |
| ความยืดหยุ่น | จัดการ Tag เดียว | จัดการหลาย Tag จากที่เดียว |
| การแก้ไข | ต้องแก้โค้ดใน Kartra | แก้ผ่าน GTM Dashboard |
| เหมาะกับ | มือใหม่ มี Tag 1-2 ตัว | ใช้หลายแพลตฟอร์มโฆษณา |
| Version Control | ไม่มี | มี ย้อนกลับได้ |

- **มือใหม่:** เริ่มจาก Global Site Tag
- **หลายแพลตฟอร์ม:** ใช้ GTM ตั้งแต่แรก

---

## SLIDE 7: ตรวจสอบ Tag ด้วย Google Tag Assistant

- **Google Tag Assistant** = Chrome Extension ฟรี
- **วิธีใช้:**
  1. ติดตั้ง Extension จาก Chrome Web Store
  2. เข้าไปที่ Kartra Landing Page
  3. เปิด Tag Assistant
  4. ดูผลลัพธ์:
     - สีเขียว = Tag ทำงานถูกต้อง
     - สีเหลือง = มีข้อเตือน
     - สีแดง = มีปัญหา ต้องแก้ไข
- **อีกวิธี:** ดูสถานะ Conversion ใน Google Ads
  - **Recording** = ปกติ
  - **Inactive** = ต้องตรวจ Tag ใหม่

---

## SLIDE 8: ข้อดี 6 ประการของการเชื่อม Google กับ Kartra

| # | ข้อดี | รายละเอียด |
|---|-------|-----------|
| 1 | ข้อมูล Conversion แม่นยำ | รู้จริงว่าคนจากโฆษณากรอกฟอร์ม/ซื้อกี่คน |
| 2 | Optimize Campaign ได้ดีขึ้น | มีข้อมูลจริงให้ปรับปรุงแคมเปญ |
| 3 | ใช้ Smart Bidding ได้ | Google ปรับราคาประมูลอัตโนมัติ |
| 4 | รู้ว่าโฆษณาชุดไหนคุ้มค่า | เห็น Conversion ระดับ Ad Group/Ad |
| 5 | ลดการเสียเงินเปล่า | หยุดโฆษณาที่ไม่ได้ Conversion ได้ทันที |
| 6 | ข้อมูลสะสมยิ่งดีขึ้น | ยิ่งมี Data มาก Google ยิ่ง Optimize ดี |

---

## SLIDE 9: Checklist ก่อนเริ่มลงโฆษณา

- [ ] สร้าง Conversion Action ใน Google Ads
- [ ] คัดลอก Global Site Tag + Event Snippet
- [ ] วาง Global Site Tag ใน Kartra Landing Page (Header)
- [ ] วาง Event Snippet ใน Kartra Thank You Page (Header)
- [ ] ตรวจสอบด้วย Google Tag Assistant (สีเขียว)
- [ ] ทำ Test Conversion ด้วยตัวเอง
- [ ] ตรวจสถานะ Conversion ใน Google Ads = Recording
- [ ] พร้อมเริ่มลงโฆษณา

---

## SLIDE 10: สรุปและก้าวต่อไป (Summary & Next Steps)

- **หลักคิด:** เชื่อม Google Ads กับ Kartra ก่อนเริ่มลงโฆษณาเสมอ
- **3 ขั้นตอนหลัก:**
  1. ใส่ Google Tag ใน Kartra Page Settings → Header
  2. ตรวจสอบด้วย Tag Assistant → เขียว = ปกติ
  3. ทำ Test Conversion → ยืนยันว่าข้อมูลถูกบันทึก
- **ผลลัพธ์:** ข้อมูลแม่นยำ, Optimize ดีขึ้น, Smart Bidding ทำงานได้
- **ขั้นตอนถัดไป:** ตอนที่ 12 ลงโฆษณา Google Ads ตอนที่ 2

---

> ทบทวนต่อ: **YTOPT-012** — ลงโฆษณา Google Ads ตอนที่ 2
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*จำนวน Slides ทั้งหมด: 10 สไลด์*
