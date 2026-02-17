# Slides: วิธีตั้งค่า Plugin Site Kit — WEB2-010
> **Format:** Slide Outline (10 Slides)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 10
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## SLIDE 1: หน้าปก (Title Slide)

- **วิธีตั้งค่า Plugin Site Kit**
- SWP3 บทที่ 11: สร้างเว็บไซต์ Part 2 — ตอนที่ 10
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- รู้จัก Google Site Kit และความสำคัญ
- เข้าใจขั้นตอนติดตั้งและ One-click Setup
- รู้จักบริการ Google 4 ตัวที่เชื่อมต่อได้
- อ่านข้อมูล Search Console ได้ (Impressions, Clicks, CTR, Position)
- เข้าใจข้อดีของ Site Kit เทียบกับปลั๊กอินแยก

---

## SLIDE 3: Google Site Kit คืออะไร?

- ปลั๊กอิน WordPress **อย่างเป็นทางการจาก Google**
- ศูนย์กลางเชื่อมต่อบริการ Google กับเว็บไซต์
- ฟรี 100% ไม่มีเวอร์ชัน Premium
- ข้อมูลถูกต้องเพราะมาจาก Google โดยตรง
- ปลั๊กอินตัวแรกๆ ที่ทุกเว็บ WordPress ควรติดตั้ง

---

## SLIDE 4: 4 บริการ Google ที่เชื่อมต่อได้

| บริการ | หน้าที่ |
|--------|---------|
| Google Analytics | วิเคราะห์พฤติกรรมผู้เข้าชม |
| Search Console | ติดตามอันดับในผลการค้นหา |
| AdSense | จัดการโฆษณาและรายได้ |
| PageSpeed Insights | วัดความเร็วเว็บไซต์ |

---

## SLIDE 5: ขั้นตอนการติดตั้ง (One-click Setup)

- **ขั้นที่ 1:** Plugins > Add New > ค้นหา "Site Kit by Google"
- **ขั้นที่ 2:** Install > Activate
- **ขั้นที่ 3:** Setup Wizard จะเปิดขึ้น > Sign in Google Account
- **ขั้นที่ 4:** อนุญาตการเข้าถึง > Ownership Verification อัตโนมัติ
- **ขั้นที่ 5:** เชื่อมต่อบริการทีละตัว (Search Console > Analytics > ฯลฯ)
- ทั้งหมดไม่ต้องแก้ไขโค้ดใดๆ

---

## SLIDE 6: เข้าใจข้อมูล Search Console

| Metric | ความหมาย | ตัวอย่าง |
|--------|----------|---------|
| Impressions | จำนวนครั้งที่เว็บปรากฏในผลค้นหา | 1,000 ครั้ง/เดือน |
| Clicks | จำนวนคนที่คลิกเข้ามาจริง | 50 ครั้ง/เดือน |
| CTR | อัตราการคลิก (Clicks/Impressions) | 5% |
| Position | ตำแหน่งเฉลี่ยในผลค้นหา | 12.5 (หน้า 2) |

---

## SLIDE 7: การวิเคราะห์ข้อมูล Search Console

- **Impressions สูง + Clicks ต่ำ** = ปรับปรุง Title และ Meta Description
- **Position สูงเกินไป (หน้า 3+)** = ทำ SEO เพิ่มเติม
- **CTR ต่ำกว่า 3%** = ผลค้นหาไม่น่าคลิก ต้องปรับ
- **เคล็ดลับ:** ตรวจสอบข้อมูลอย่างน้อยสัปดาห์ละครั้ง
- ติดตามแนวโน้มเพื่อดูว่า SEO ดีขึ้นหรือแย่ลง

---

## SLIDE 8: PageSpeed Insights

- วัดความเร็วเว็บไซต์ทั้ง **Mobile** และ **Desktop**
- คะแนน 0-100 แบ่ง 3 ระดับ:
  - **90-100** = ดีเยี่ยม (สีเขียว)
  - **50-89** = พอใช้ (สีส้ม)
  - **ต่ำกว่า 50** = ต้องปรับปรุงด่วน (สีแดง)
- Google ให้ความสำคัญกับ Mobile-first Indexing
- ความเร็วเว็บส่งผลต่อทั้ง SEO และ User Experience

---

## SLIDE 9: Site Kit vs ติดตั้งปลั๊กอินแยก

| เกณฑ์ | Site Kit | ติดตั้งแยก |
|-------|---------|-----------|
| จำนวนปลั๊กอิน | 1 ตัว | 3-4 ตัว |
| Performance | เบา | หนักกว่า |
| ข้อมูล | ถูกต้อง (จาก Google) | อาจคลาดเคลื่อน |
| Dashboard | รวมศูนย์ | กระจาย |
| ข้อมูลเชิงลึก | ภาพรวม | ละเอียดกว่า |

---

## SLIDE 10: สรุปและก้าวต่อไป (Summary & Next Steps)

- Site Kit = ปลั๊กอินทางการ Google รวม 4 บริการในที่เดียว
- One-click Setup + Ownership Verification อัตโนมัติ
- ดู Impressions, Clicks, CTR, Position ได้จาก Dashboard
- ฟรี 100% ไม่มีค่าใช้จ่าย
- **Action Item:** ติดตั้ง Site Kit วันนี้ เริ่มเก็บข้อมูลทันที
- **ตอนถัดไป:** วิธีติดตั้ง Google Analytics อย่างละเอียด

---

*จำนวน Slides ทั้งหมด: 10 สไลด์*
