# ขั้นตอนเตรียมเครื่องมือ 1 — YTCAMP-004 Audio Script
> Format: Audio Script (Podcast-style)
> Source: SWP3 Ch19 Youtube Ads Campaign ตอนที่ 4
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 0:06:38

---

## SEGMENT 1: เปิดรายการ (00:00 - 01:20)

**Host A:** สวัสดีครับ กลับมาพบกันอีกครั้งกับ PinkCastle Podcast ซีรีส์ Youtube Ads Campaign ตอนที่ 4 แล้วครับ วันนี้เราจะเข้าสู่ขั้นตอนที่สำคัญมากก่อนจะปล่อยแคมเปญได้ นั่นก็คือ การเตรียมเครื่องมือครับ

**Host B:** ใช่ค่ะ หลายคนอยากรีบทำ Ads เลย แต่ถ้าเครื่องมือยังไม่พร้อม ก็เหมือนทหารออกรบโดยไม่มีอาวุธค่ะ วันนี้เราจะมาเตรียมทุกอย่างให้พร้อม ตั้งแต่ Google Ads Account ไปจนถึง Conversion Tracking

**Host A:** ผมอยากให้มองภาพรวมก่อนครับ เครื่องมือที่เราต้องเตรียมมีทั้งหมด 4 ตัวหลัก ได้แก่ Google Ads, Google Tag Manager, Google Analytics 4 และ Youtube Channel ที่เชื่อมกันหมด ทุกตัวเป็นของ Google ทั้งหมด ดังนั้นถ้ามี Gmail account เดียว ก็จัดการได้สะดวกมากครับ

**Host B:** และเราจะทำแบบ Step-by-step เลยนะคะ ใครที่เปิดคอมพ์ตามได้เลยค่ะ

---

## SEGMENT 2: Google Ads Account — สร้างและตั้งค่า (01:20 - 02:50)

**Host A:** เริ่มจากตัวแรกเลยครับ Google Ads Account ซึ่งเป็นศูนย์บัญชาการของการทำโฆษณาทั้งหมด เข้าไปที่ ads.google.com แล้วคลิก Start Now ได้เลย

**Host B:** ขั้นตอนสร้างบัญชีไม่ยากเลยค่ะ แต่มีจุดที่ต้องระวังคือ ตอนที่ Google ถามว่าจะทำ Smart Campaign ให้เลือก Switch to Expert Mode แทนค่ะ เพราะ Expert Mode จะให้เราควบคุมได้ทุกอย่าง ตั้งแต่ Bidding Strategy ไปจนถึง Audience Targeting

**Host A:** ถูกต้องครับ Smart Campaign มันง่ายก็จริง แต่ควบคุมอะไรไม่ได้เลย เหมือนให้ Google ตัดสินใจทุกอย่างแทนเรา สำหรับ Youtube Ads เราต้องการความยืดหยุ่นในการตั้งค่าครับ

**Host B:** หลังจากสร้างบัญชีเสร็จ อย่าลืมตั้งค่า Time Zone เป็น Bangkok (GMT+7) และ Currency เป็น THB นะคะ ถ้าตั้งผิดแล้วจะแก้ไม่ได้ ต้องสร้างบัญชีใหม่เลยค่ะ

**Host A:** นี่คือจุดที่คนพลาดบ่อยมากครับ Time Zone กับ Currency ต้องตั้งให้ถูกตั้งแต่แรก เพราะ Google Ads ไม่อนุญาตให้เปลี่ยนภายหลัง

---

## SEGMENT 3: เชื่อม Youtube Channel + ติดตั้ง GTM (02:50 - 04:30)

**Host B:** เครื่องมือตัวที่ 2 คือการเชื่อม Youtube Channel กับ Google Ads ค่ะ ขั้นตอนคือเข้าไปที่ Google Ads → Tools & Settings → Linked accounts → YouTube แล้วคลิก Link

**Host A:** ใส่ URL ของ Youtube Channel เรา แล้ว Google จะส่งคำขอไปที่ Channel ครับ ถ้าเราเป็นเจ้าของ Channel อยู่แล้ว แค่กด Approve ก็เสร็จ แต่ถ้าเป็นของคนอื่นต้องรอเจ้าของ Channel อนุมัติ

**Host B:** การเชื่อม Youtube Channel ทำให้เราเข้าถึง Video Assets สำหรับทำโฆษณาได้โดยตรง และยังเห็นข้อมูลว่าคนที่ดูวิดีโอเราไปทำอะไรต่อค่ะ ซึ่งเป็นข้อมูลที่มีค่ามากสำหรับ Retargeting

**Host A:** ต่อมาเครื่องมือตัวที่ 3 ครับ Google Tag Manager หรือ GTM เข้าไปที่ tagmanager.google.com สร้าง Account ใหม่ ตั้งชื่อ Container ให้ตรงกับเว็บไซต์ของเรา แล้วเลือก Container Type เป็น Web

**Host B:** หลังจากสร้าง Container เสร็จ GTM จะให้โค้ด 2 ชุดค่ะ ชุดแรกใส่ใน head ของเว็บ ชุดที่สองใส่หลัง body tag เปิด ต้องใส่ทุกหน้าของเว็บไซต์นะคะ ถ้าใช้ Systeme.io หรือ Kartra ก็ไปหาช่อง Tracking Code แล้ววางได้เลย

**Host A:** GTM เปรียบเหมือนกล่องเครื่องมือครับ แทนที่จะฝัง Code ของ Google Ads, GA4 ลงในเว็บไซต์โดยตรง เราฝังแค่ GTM Code อันเดียว แล้วจัดการ Tag ต่างๆ ผ่าน GTM Dashboard ได้หมด ง่ายต่อการเพิ่ม แก้ไข หรือลบ Tag โดยไม่ต้องแก้โค้ดเว็บ

---

## SEGMENT 4: GA4 + Conversion Tracking (04:30 - 05:50)

**Host B:** เครื่องมือตัวที่ 4 คือ Google Analytics 4 หรือ GA4 ค่ะ ถ้ายังไม่มีให้เข้าไปที่ analytics.google.com สร้าง Property ใหม่ แล้วเลือก Data Stream เป็น Web ใส่ URL เว็บไซต์ของเรา

**Host A:** สิ่งที่ต้องทำหลังจากสร้าง GA4 Property คือเชื่อมกับ Google Ads ครับ เข้าไปที่ GA4 → Admin → Google Ads Links → Link แล้วเลือก Google Ads Account ที่เราสร้างไว้ตอนแรก การเชื่อมนี้ทำให้ข้อมูลไหลระหว่าง 2 ระบบได้ เห็น Audience ใน Google Ads และเห็นข้อมูลแคมเปญใน GA4

**Host B:** ต่อมาคือ Conversion Tracking ซึ่งเป็นหัวใจของการวัดผลค่ะ เข้าไปที่ Google Ads → Tools → Conversions → New Conversion Action เลือก Website แล้วใส่ URL ของ Thank You Page

**Host A:** ตั้งชื่อ Conversion ให้เข้าใจง่ายครับ เช่น "Lead Form Submission" แล้วเลือก Category เป็น Lead ตั้ง Value เป็น 1 ตรง Count เลือก One conversion per click เพราะเราต้องการนับ Lead ไม่ใช่นับ Transaction ครับ

**Host B:** สุดท้ายคือ Install Tag ค่ะ ถ้าเราติดตั้ง GTM ไว้แล้ว ให้เลือก Use Google Tag Manager แล้วทำตามขั้นตอน สร้าง Conversion Linker Tag และ Google Ads Conversion Tracking Tag ใน GTM ค่ะ ง่ายกว่าการฝัง Code เองมากเลย

---

## SEGMENT 5: Billing + Checklist สรุป (05:50 - 06:38)

**Host A:** ขั้นตอนสุดท้ายก่อนจะพร้อมปล่อยแคมเปญคือตั้งค่า Billing ครับ เข้าไปที่ Google Ads → Tools → Billing → Payment Methods ใส่บัตรเครดิตหรือบัตรเดบิตได้เลย สำหรับประเทศไทย Google Ads รองรับ Visa และ Mastercard

**Host B:** สิ่งที่ต้องรู้คือ Google Ads ใช้ระบบ Automatic Payments ค่ะ คือเก็บเงินหลังจากใช้งาน โดยจะเก็บเมื่อถึง Threshold (ปกติเริ่มที่ 1,000 บาท) หรือทุก 30 วัน แล้วแต่อันไหนถึงก่อน

**Host A:** มาถึง Checklist สรุปทั้งหมดครับ เครื่องมือที่ต้องพร้อมก่อนไปตอนต่อไป ข้อ 1 Google Ads Account สร้างแล้ว ตั้ง Expert Mode, Time Zone Bangkok, Currency THB ข้อ 2 Youtube Channel เชื่อมกับ Google Ads แล้ว ข้อ 3 GTM ติดตั้งบนเว็บไซต์แล้ว ข้อ 4 GA4 สร้างแล้ว เชื่อมกับ Google Ads แล้ว ข้อ 5 Conversion Tracking ตั้งค่าแล้ว ข้อ 6 Billing ใส่บัตรแล้ว

**Host B:** ถ้ายังทำไม่ครบทั้ง 6 ข้อ อย่าเพิ่งไปตอนต่อไปนะคะ เพราะตอนหน้าเราจะเตรียมเครื่องมือเพิ่มเติม ซึ่งต้องใช้สิ่งที่ตั้งค่าวันนี้เป็นพื้นฐาน

**Host A:** ถูกต้องครับ ทำให้ครบ Checklist แล้วพบกันใหม่ในตอนที่ 5 ครับ สวัสดีครับ

**Host B:** สวัสดีค่ะ

---

*Word count: ~950 | Segments: 5 | Estimated read time: 7 minutes*

---

> ทบทวนต่อ: **YTCAMP-005** — ขั้นตอนเตรียมเครื่องมือ 2
> Series: SWP3 Ch19 Youtube Ads Campaign
> PinkCastle Academy © 2026
