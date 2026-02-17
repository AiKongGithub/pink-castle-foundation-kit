# ขั้นตอนเตรียมเครื่องมือ 1 — YTCAMP-004 Quiz
> Format: Multiple Choice Quiz (12 Questions)
> Source: SWP3 Ch19 Youtube Ads Campaign ตอนที่ 4
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 0:06:38
> คะแนนเต็ม: 12 คะแนน | ผ่าน: 9/12 (75%)

---

### คำแนะนำ
- อ่านคำถามแต่ละข้อและเลือกคำตอบที่ถูกต้องที่สุด
- ตรวจคำตอบด้วยส่วน ✅ ด้านล่างแต่ละข้อ
- บันทึกคะแนนของคุณและทบทวนข้อที่ตอบผิด

---

### Q1: เมื่อสร้าง Google Ads Account ใหม่ ควรเลือกโหมดใด?

A) Smart Campaign เพราะง่ายสำหรับมือใหม่
B) Expert Mode เพราะควบคุมได้ทุกอย่าง
C) Basic Mode เพราะค่าใช้จ่ายถูกกว่า
D) Auto Mode เพราะ Google ช่วยปรับให้อัตโนมัติ

✅ **คำตอบ: B) Expert Mode เพราะควบคุมได้ทุกอย่าง**

**อธิบาย:** Expert Mode ให้ควบคุม Bidding Strategy, Audience Targeting, Ad Placement ได้ทั้งหมด ส่วน Smart Campaign ให้ Google ตัดสินใจแทนทุกอย่าง สำหรับ Youtube Ads ที่ต้องการความแม่นยำ Expert Mode เป็นสิ่งจำเป็น

---

### Q2: ถ้าตั้ง Time Zone และ Currency ผิดใน Google Ads จะทำอย่างไร?

A) เข้า Settings แก้ไขได้ทันที
B) ติดต่อ Google Support ให้ช่วยแก้
C) ต้องสร้างบัญชีใหม่ทั้งหมด
D) รอ 30 วันแล้วจะแก้ไขได้

✅ **คำตอบ: C) ต้องสร้างบัญชีใหม่ทั้งหมด**

**อธิบาย:** Google Ads ไม่อนุญาตให้เปลี่ยน Time Zone และ Currency หลังจากสร้างบัญชีแล้ว ต้องตั้ง Bangkok (GMT+7) และ THB ให้ถูกต้องตั้งแต่แรก ถ้าผิดต้องสร้างบัญชีใหม่

---

### Q3: การเชื่อม Youtube Channel กับ Google Ads ทำที่ไหน?

A) Youtube Studio → Settings → Advanced
B) Google Ads → Tools & Settings → Linked accounts → YouTube
C) Google Ads → Campaigns → New Campaign → YouTube
D) Gmail Settings → Connected Accounts

✅ **คำตอบ: B) Google Ads → Tools & Settings → Linked accounts → YouTube**

**อธิบาย:** เข้า Google Ads → Tools & Settings → Linked accounts → YouTube → คลิก Link → ใส่ URL ของ Channel → Approve ทำให้เข้าถึง Video Assets และข้อมูล Retargeting

---

### Q4: การเชื่อม Youtube Channel กับ Google Ads มีประโยชน์อะไร?

A) ทำให้วิดีโอได้ View มากขึ้นอัตโนมัติ
B) ลดค่าโฆษณา 50%
C) เข้าถึง Video Assets โดยตรงและเก็บข้อมูล Retargeting
D) ทำให้ Channel ได้ Subscriber มากขึ้น

✅ **คำตอบ: C) เข้าถึง Video Assets โดยตรงและเก็บข้อมูล Retargeting**

**อธิบาย:** การ Link ทำให้ใช้วิดีโอจาก Channel ทำโฆษณาได้โดยตรง และเห็นข้อมูลว่าคนที่ดูวิดีโอไปทำอะไรต่อ ซึ่งมีค่ามากสำหรับ Retargeting

---

### Q5: Google Tag Manager (GTM) เปรียบเทียบได้กับอะไร?

A) ร้านขายของออนไลน์
B) กล่องเครื่องมือสำหรับจัดการ Tag
C) โปรแกรมสร้างเว็บไซต์
D) ระบบรักษาความปลอดภัย

✅ **คำตอบ: B) กล่องเครื่องมือสำหรับจัดการ Tag**

**อธิบาย:** GTM เปรียบเหมือนกล่องเครื่องมือ ฝัง GTM Code อันเดียวบนเว็บ แล้วจัดการ Tag ทั้งหมด (Google Ads, GA4, Facebook Pixel) ผ่าน Dashboard ไม่ต้องแก้โค้ดเว็บทุกครั้งที่เพิ่มหรือแก้ Tag

---

### Q6: GTM ให้โค้ดกี่ชุดสำหรับติดตั้งบนเว็บไซต์?

A) 1 ชุด ใส่ใน head
B) 2 ชุด — ชุดแรกใน head ชุดที่สองหลัง body tag เปิด
C) 3 ชุด — head, body, footer
D) ไม่ต้องใส่โค้ด ใช้ปลั๊กอินได้เลย

✅ **คำตอบ: B) 2 ชุด — ชุดแรกใน head ชุดที่สองหลัง body tag เปิด**

**อธิบาย:** GTM ให้โค้ด 2 ชุด ชุดแรกใส่ใน `<head>` ชุดที่สองใส่หลัง `<body>` tag เปิด ต้องใส่ทั้ง 2 ชุดและต้องใส่ทุกหน้าของเว็บไซต์ ถ้าใส่ไม่ครบ Tag จะไม่ Fire

---

### Q7: หลังจากสร้าง GA4 Property ต้องทำอะไรเพิ่ม?

A) ตั้งค่า SEO Keywords
B) เชื่อมกับ Google Ads ผ่าน Admin → Google Ads Links
C) อัปโหลดรายชื่อลูกค้า
D) สร้าง Youtube Channel ใหม่

✅ **คำตอบ: B) เชื่อมกับ Google Ads ผ่าน Admin → Google Ads Links**

**อธิบาย:** หลังสร้าง GA4 ต้องเชื่อมกับ Google Ads ที่ GA4 → Admin → Google Ads Links → Link ทำให้ข้อมูลไหลระหว่าง 2 ระบบ เห็น Audience ใน Google Ads และเห็นข้อมูลแคมเปญใน GA4

---

### Q8: เมื่อสร้าง Conversion Action สำหรับ Lead Generation ควรเลือก Count แบบใด?

A) Every conversion
B) One conversion per click
C) No count
D) Unlimited conversions

✅ **คำตอบ: B) One conversion per click**

**อธิบาย:** สำหรับ Lead Generation ต้องใช้ One conversion per click เพราะนับ 1 ต่อ 1 คน ถ้าคนเดียวกรอกฟอร์ม 3 ครั้งจะนับเป็น 1 Conversion เท่านั้น ถ้าใช้ Every conversion จะนับเป็น 3 ซึ่งทำให้ข้อมูลบิดเบือน

---

### Q9: วิธีที่แนะนำในการติดตั้ง Conversion Tag คือวิธีใด?

A) ฝัง Code โดยตรงในทุกหน้าเว็บ
B) ใช้ Google Tag Manager
C) ส่ง Email ให้ Google ติดตั้งให้
D) ใช้ Browser Extension

✅ **คำตอบ: B) ใช้ Google Tag Manager**

**อธิบาย:** ถ้าติดตั้ง GTM ไว้แล้ว ให้เลือก Use Google Tag Manager จะได้ Conversion ID + Label ไปสร้าง Conversion Linker Tag + Conversion Tracking Tag ใน GTM ง่ายกว่า ปลอดภัยกว่า และแก้ไขสะดวกกว่าการฝัง Code โดยตรง

---

### Q10: ระบบ Billing ของ Google Ads เก็บเงินเมื่อไร?

A) ก่อนเริ่มแคมเปญ (Prepaid)
B) เมื่อถึง Threshold หรือทุก 30 วัน แล้วแต่อันไหนถึงก่อน
C) ทุกสิ้นเดือนเท่านั้น
D) เมื่อยอดถึง 10,000 บาท

✅ **คำตอบ: B) เมื่อถึง Threshold หรือทุก 30 วัน แล้วแต่อันไหนถึงก่อน**

**อธิบาย:** Google Ads ใช้ระบบ Automatic Payments เก็บเงินหลังจากใช้งาน โดยเก็บเมื่อถึง Threshold (เริ่มต้น 1,000 บาท) หรือทุก 30 วัน แล้วแต่อันไหนถึงก่อน

---

### Q11: สำหรับประเทศไทย Google Ads รองรับบัตรชำระเงินอะไรบ้าง?

A) เฉพาะ Visa เท่านั้น
B) Visa และ Mastercard
C) เฉพาะบัตรเครดิตธนาคารไทย
D) PromptPay เท่านั้น

✅ **คำตอบ: B) Visa และ Mastercard**

**อธิบาย:** สำหรับประเทศไทย Google Ads รองรับ Visa และ Mastercard ทั้งบัตรเครดิตและบัตรเดบิต ตั้งค่าที่ Tools → Billing → Payment Methods

---

### Q12: เครื่องมือที่ต้องเตรียมให้ครบก่อนไป YTCAMP-005 มีกี่รายการ?

A) 3 รายการ (Google Ads, GTM, GA4)
B) 4 รายการ (Google Ads, Youtube, GTM, GA4)
C) 6 รายการ (Google Ads, Youtube Link, GTM, GA4, Conversion Tracking, Billing)
D) 8 รายการ (รวม Facebook Pixel และ TikTok Pixel)

✅ **คำตอบ: C) 6 รายการ (Google Ads, Youtube Link, GTM, GA4, Conversion Tracking, Billing)**

**อธิบาย:** Checklist 6 ข้อที่ต้องครบ: (1) Google Ads Account (2) Youtube Channel Link (3) GTM ติดตั้งบนเว็บ (4) GA4 เชื่อม Google Ads (5) Conversion Tracking (6) Billing ถ้ายังไม่ครบอย่าเพิ่งไปตอนต่อไป

---

## บันทึกคะแนน

| ช่วงคะแนน | ระดับ | คำแนะนำ |
|-----------|-------|---------|
| 12/12 | Mastery | พร้อมเรียน YTCAMP-005 |
| 9-11/12 | Pass | ทบทวนข้อที่ผิดก่อน |
| 6-8/12 | Average | ดู Lesson ซ้ำ 1 รอบ |
| 0-5/12 | Need Review | ดู Lesson ใหม่ทั้งหมด |

---

> ทบทวนต่อ: **YTCAMP-005** — ขั้นตอนเตรียมเครื่องมือ 2
> Series: SWP3 Ch19 Youtube Ads Campaign
> PinkCastle Academy © 2026
