# ขั้นตอนเตรียมเครื่องมือ 1 — YTCAMP-004 Executive Summary
> **Format:** Executive Summary
> **Source:** SWP3 Ch19 Youtube Ads Campaign ตอนที่ 4
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18
> **Duration:** 0:06:38

---

## สรุปภาพรวม

บทเรียนนี้เป็นขั้นตอนเตรียมเครื่องมือส่วนที่ 1 สำหรับ Youtube Ads Campaign ครอบคลุมการสร้างและตั้งค่า Google Ads Account ในโหมด Expert Mode, การเชื่อม Youtube Channel เข้ากับ Google Ads เพื่อเข้าถึง Video Assets และข้อมูล Retargeting, การติดตั้ง Google Tag Manager (GTM) บนเว็บไซต์เพื่อจัดการ Tag ทั้งหมดจากจุดเดียว, การสร้าง Google Analytics 4 (GA4) Property และเชื่อมกับ Google Ads, การตั้งค่า Conversion Tracking เพื่อนับ Lead และสุดท้ายคือการตั้งค่า Billing สำหรับชำระค่าโฆษณา เครื่องมือทั้ง 6 รายการนี้เป็นพื้นฐานที่ต้องพร้อมก่อนจะสร้างแคมเปญจริงได้

## ประเด็นสำคัญ (Key Takeaways)

| # | ประเด็น | รายละเอียด |
|---|---------|-----------|
| 1 | Expert Mode สำคัญกว่า Smart Campaign | Expert Mode ให้ควบคุม Bidding, Targeting, Placement ได้ทั้งหมด ส่วน Smart Campaign ให้ Google ตัดสินใจแทน |
| 2 | Time Zone + Currency แก้ไม่ได้ | ต้องตั้ง Bangkok (GMT+7) และ THB ตั้งแต่แรก ถ้าตั้งผิดต้องสร้างบัญชีใหม่ |
| 3 | Youtube Channel ต้องเชื่อม Google Ads | เพื่อเข้าถึง Video Assets โดยตรงและเก็บข้อมูล Retargeting จากคนดู |
| 4 | GTM = กล่องเครื่องมือจัดการ Tag | ฝัง GTM Code อันเดียว แล้วจัดการ Tag ทั้งหมดผ่าน Dashboard ไม่ต้องแก้โค้ดเว็บ |
| 5 | GA4 + Google Ads ต้องเชื่อมกัน | ทำให้ข้อมูลไหลระหว่าง 2 ระบบ เห็น Audience ใน Ads และเห็นแคมเปญใน GA4 |

## โครงสร้างเนื้อหา

| Segment | หัวข้อ | Timestamp | สาระสำคัญ |
|---------|--------|-----------|-----------|
| 1 | เปิดรายการ | 00:00 - 01:20 | ภาพรวม 4 เครื่องมือหลักที่ต้องเตรียม |
| 2 | Google Ads Account | 01:20 - 02:50 | สร้างบัญชี Expert Mode + ตั้ง Time Zone/Currency |
| 3 | Youtube + GTM | 02:50 - 04:30 | เชื่อม Channel + ติดตั้ง GTM Container บนเว็บ |
| 4 | GA4 + Conversion Tracking | 04:30 - 05:50 | สร้าง GA4 Property + ตั้งค่า Conversion Action |
| 5 | Billing + Checklist | 05:50 - 06:38 | ตั้งค่าการชำระเงิน + สรุป Checklist 6 ข้อ |

## แผนภาพการเชื่อมต่อเครื่องมือ

```
Youtube Channel
    ↕ Link
Google Ads Account (Expert Mode)
    ↕ Link              ↕ GTM Tags
Google Analytics 4      Google Tag Manager
    ↕ Events                ↕ Container Code
Conversion Tracking     Website (ทุกหน้า)
    ↕
Billing (Visa/Mastercard)
```

## Tool Setup Checklist

| # | เครื่องมือ | สิ่งที่ต้องทำ | สถานะ | หมายเหตุ |
|---|-----------|-------------|--------|---------|
| 1 | Google Ads Account | สร้างบัญชี + Expert Mode | ▢ | Time Zone: Bangkok, Currency: THB |
| 2 | Youtube Channel | เชื่อมกับ Google Ads | ▢ | Tools → Linked accounts → YouTube |
| 3 | Google Tag Manager | สร้าง Container + ใส่โค้ดบนเว็บ | ▢ | โค้ด 2 ชุด: head + body |
| 4 | Google Analytics 4 | สร้าง Property + เชื่อม Google Ads | ▢ | Admin → Google Ads Links |
| 5 | Conversion Tracking | สร้าง Conversion Action | ▢ | Category: Lead, Count: One per click |
| 6 | Billing | ใส่บัตรเครดิต/เดบิต | ▢ | Threshold เริ่มต้น 1,000 บาท |

## คำแนะนำสำหรับผู้บริหาร

การเตรียมเครื่องมือเป็นขั้นตอนที่ไม่ควรข้ามหรือทำลวกๆ เพราะถ้าตั้งค่าผิดตั้งแต่แรก อาจต้องเริ่มใหม่ทั้งหมด โดยเฉพาะ Google Ads Account ที่ Time Zone และ Currency แก้ไม่ได้หลังจากสร้างแล้ว การลงทุนเวลา 30-60 นาทีตั้งค่าให้ถูกต้อง จะป้องกันปัญหาที่ต้องใช้เวลาแก้ไขหลายวันในภายหลัง สิ่งสำคัญ 3 ข้อ: (1) ใช้ Expert Mode เพื่อควบคุม Budget ได้เต็มที่ (2) เชื่อมเครื่องมือทั้งหมดเข้าด้วยกันผ่าน Google Account เดียว (3) ตั้งค่า Conversion Tracking ให้เสร็จก่อนปล่อยแคมเปญ เพื่อให้วัดผลได้ตั้งแต่วันแรก

---

*Word count: ~550 | Tables: 4 | Reading time: 3 minutes*

---

> ทบทวนต่อ: **YTCAMP-005** — ขั้นตอนเตรียมเครื่องมือ 2
> Series: SWP3 Ch19 Youtube Ads Campaign
> PinkCastle Academy © 2026
