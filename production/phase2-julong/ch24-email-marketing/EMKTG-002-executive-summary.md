# Email Marketing ตอนที่ 2 — EMKTG-002 Executive Summary
> Format: Executive Summary (~500 words + tables)
> Source: SWP3 Ch24 Email Marketing Mastery ตอนที่ 2
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 1:18:44

---

## สรุปภาพรวม

Email Marketing ตอนที่ 2 เป็นการต่อยอดจากพื้นฐานในตอนที่ 1 เข้าสู่กลยุทธ์ระดับกลาง ครอบคลุม 6 หัวข้อหลัก ได้แก่ Segmentation การแบ่งกลุ่ม Email List ตามพฤติกรรมและความสนใจ, Personalization ที่ลึกกว่าแค่ใส่ชื่อผู้รับ, A/B Testing ทดสอบอีเมลเพื่อหาเวอร์ชันที่ดีที่สุด, Deliverability การทำให้อีเมลเข้า Inbox ไม่ใช่ Spam, Re-engagement Campaign ดึงสมาชิกที่หายไปกลับมา และ Email Analytics การวัดผลด้วย 5 Metrics สำคัญ

เนื้อหาเน้นให้ผู้เรียนเข้าใจว่า การส่งอีเมลเหมือนกันให้ทุกคนเป็นยุคที่ผ่านไปแล้ว การแบ่งกลุ่มและส่งเนื้อหาที่ตรงจุดจะทำให้ Open Rate สูงขึ้น 14% และ Click Rate สูงขึ้น 100% เมื่อเทียบกับการส่งแบบหว่าน

---

## ประเด็นสำคัญ 6 ข้อ

| # | ประเด็น | รายละเอียด |
|---|---------|------------|
| 1 | Segmentation คือกุญแจ | แบ่ง List ตาม Behavior, Purchase History, Engagement Level, Tags ทำให้ Open Rate สูงขึ้น 14% |
| 2 | Personalization 4 ระดับ | ชื่อผู้รับ → เนื้อหาตาม Segment → Dynamic Content → Product Recommendations เพิ่ม Conversion 20-30% |
| 3 | A/B Testing ทีละตัวแปร | ทดสอบ Subject Line, Send Time, CTA, Layout ส่งกลุ่มทดสอบ 20% แล้วส่งตัวที่ชนะให้ 80% |
| 4 | Deliverability ต้องจัดการ | SPF/DKIM/DMARC + Warm up IP + Clean List + หลีกเลี่ยง Spam Words + รักษา Sender Reputation |
| 5 | Re-engagement ก่อนลบ | Win-back Email → Special Offer → Last Chance ถ้ายังเงียบค่อยลบ ทำให้ List สะอาดขึ้น |
| 6 | Analytics 5 ตัวชี้วัด | Open Rate, Click Rate, Conversion Rate, Revenue per Email, List Growth Rate ดูทุกสัปดาห์ |

---

## 4 ระดับ Personalization

| ระดับ | วิธีการ | ตัวอย่าง | ผลกระทบ |
|-------|---------|---------|---------|
| 1. ชื่อผู้รับ | ใส่ชื่อใน Subject/เนื้อหา | "สวัสดี คุณสมชาย" | Open Rate +10% |
| 2. Segment-based | เนื้อหาต่างกันตาม Segment | ลูกค้าเก่าได้ข้อเสนอพิเศษ | Click Rate +25% |
| 3. Dynamic Content | อีเมลฉบับเดียว เนื้อหาต่างกัน | แต่ละคนเห็น product ต่างกัน | Conversion +20% |
| 4. Product Recommendations | แนะนำตามพฤติกรรมการซื้อ | "คุณอาจชอบสินค้านี้ด้วย" | Revenue +30% |

---

## A/B Testing Framework

| ตัวแปร | ทดสอบอะไร | วัดผลด้วย | ตัวอย่าง |
|--------|----------|----------|---------|
| Subject Line | หัวเรื่อง 2 แบบ | Open Rate | "เคล็ดลับ..." vs "คุณรู้ไหมว่า..." |
| Send Time | เวลาส่ง 2 ช่วง | Open Rate | 8:00 AM vs 12:00 PM |
| CTA | ปุ่ม/ข้อความชวนคลิก 2 แบบ | Click Rate | "ดูเพิ่มเติม" vs "รับส่วนลดตอนนี้" |
| Layout | การจัดวาง 2 แบบ | Click Rate | รูปซ้าย+ข้อความขวา vs ข้อความอย่างเดียว |

**กฎทอง**: เปลี่ยนทีละ 1 ตัวแปร, ส่งให้กลุ่มทดสอบ 20%, ส่งตัวที่ชนะให้ 80% ที่เหลือ

---

## Deliverability Checklist

| รายการ | วิธีทำ | ผลลัพธ์ |
|--------|--------|---------|
| SPF/DKIM/DMARC | ตั้งค่า DNS records ของ domain | ยืนยันตัวตนผู้ส่ง |
| Warm up IP | ค่อยๆ เพิ่มจำนวนส่ง (100 → 500 → 1,000) | ไม่ถูก flag เป็น spam |
| Clean List | ลบอีเมล bounce, inactive ทุก 3-6 เดือน | Bounce Rate ต่ำ |
| Avoid Spam Words | ไม่ใช้คำเช่น "ฟรี!!!", "รวยทันที" | ผ่าน spam filter |
| Sender Reputation | รักษา Open Rate > 20%, Spam Complaint < 0.1% | เข้า Inbox ได้สม่ำเสมอ |

---

## ตัวเลขสำคัญ

| Metric | ค่า |
|--------|-----|
| Segmented Email Open Rate เพิ่มขึ้น | +14% |
| Segmented Email Click Rate เพิ่มขึ้น | +100% |
| Personalization Conversion เพิ่มขึ้น | +20-30% |
| A/B Testing กลุ่มทดสอบ | 20% ของ List |
| Spam Complaint Rate ที่ปลอดภัย | < 0.1% |
| ความยาวบทเรียน | 1:18:44 |

---

## สิ่งที่ต้องทำต่อ

1. แบ่ง Email List ออกเป็นอย่างน้อย 3 Segments ตาม Engagement Level
2. ทดลอง Personalization ระดับ 2 ส่งเนื้อหาต่างกันตาม Segment
3. ทำ A/B Testing Subject Line อย่างน้อย 1 ครั้ง วัดผล Open Rate
4. ตรวจสอบ SPF/DKIM/DMARC ของ domain ที่ใช้ส่งอีเมล
5. สร้าง Re-engagement Campaign 3 ฉบับ สำหรับสมาชิกที่ไม่ Active เกิน 90 วัน
6. เรียนตอนที่ 3 เรื่อง Automation และ Funnel Email

---

> ทบทวนต่อ: **EMKTG-003** — Email Marketing ตอนที่ 3
> Series: SWP3 Ch24 Email Marketing Mastery
> PinkCastle Academy © 2026

*Word count: ~530 words*
