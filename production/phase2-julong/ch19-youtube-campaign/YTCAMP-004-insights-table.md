# ขั้นตอนเตรียมเครื่องมือ 1 — YTCAMP-004 Insights Table
> Format: Insights Table (10 rows)
> Source: SWP3 Ch19 Youtube Ads Campaign ตอนที่ 4
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 0:06:38

---

| # | Insight | รายละเอียด | ระดับสำคัญ | การนำไปใช้ |
|---|---------|-----------|-----------|-----------|
| 1 | **Expert Mode ไม่ใช่ตัวเลือก แต่เป็นข้อบังคับ** | Google Ads จะเสนอ Smart Campaign ก่อนเสมอ ต้องกด Switch to Expert Mode เอง Smart Campaign ควบคุมอะไรแทบไม่ได้ ทั้ง Bidding Strategy, Audience Targeting และ Placement ให้ Google ตัดสินใจทุกอย่าง ซึ่งไม่เหมาะกับ Youtube Ads ที่ต้องการความแม่นยำ | Critical | เลือก Expert Mode ทันทีที่สร้างบัญชี อย่าถูกหลอกด้วยความง่ายของ Smart Campaign |
| 2 | **Time Zone + Currency ตั้งผิด = เริ่มใหม่** | Google Ads ไม่อนุญาตให้เปลี่ยน Time Zone และ Currency หลังจากสร้างบัญชีแล้ว ต้องตั้ง Bangkok (GMT+7) และ THB ตั้งแต่แรก ถ้าผิดต้องสร้างบัญชีใหม่ทั้งหมด นี่คือจุดที่คนพลาดบ่อยที่สุด | Critical | ก่อนกด Create ให้ตรวจสอบ Time Zone = Bangkok (GMT+7) และ Currency = THB ทุกครั้ง อย่ารีบกดผ่าน |
| 3 | **Youtube Channel ต้อง Link ไม่ใช่แค่มี** | การมี Youtube Channel อย่างเดียวไม่พอ ต้อง Link เข้ากับ Google Ads ผ่าน Tools & Settings → Linked accounts การ Link ทำให้เข้าถึง Video Assets โดยตรงและเห็นข้อมูล Viewer สำหรับ Retargeting ถ้าไม่ Link จะใช้วิดีโอจาก Channel ทำ Ads ไม่ได้ | High | เข้า Google Ads → Tools → Linked accounts → YouTube → Link → ใส่ URL Channel → Approve |
| 4 | **GTM = กล่องเครื่องมือ ฝังครั้งเดียวจบ** | Google Tag Manager เปรียบเหมือนกล่องเครื่องมือ ฝัง GTM Code อันเดียวบนเว็บ แล้วจัดการ Tag ทั้งหมด (Google Ads, GA4, Facebook Pixel ฯลฯ) ผ่าน Dashboard ไม่ต้องแก้โค้ดเว็บทุกครั้งที่เพิ่มหรือแก้ Tag ลดโอกาสพัง ลดเวลา ลดความผิดพลาด | Critical | สร้าง GTM Container แล้วติดตั้งโค้ด 2 ชุดบนเว็บทุกหน้า ก่อนเริ่มสร้าง Tag ใดๆ |
| 5 | **GTM Code 2 ชุด ห้ามขาด** | GTM ให้โค้ด 2 ชุด ชุดแรกใส่ใน head ชุดที่สองใส่หลัง body tag เปิด ต้องใส่ทั้ง 2 ชุดและต้องใส่ทุกหน้าของเว็บไซต์ ถ้าใส่ไม่ครบ GTM จะไม่ทำงานบนหน้าที่ขาด Tag ก็ไม่ Fire ข้อมูลก็หาย | Critical | ตรวจสอบว่าโค้ด GTM ทั้ง 2 ชุดอยู่ในทุกหน้าเว็บ ใช้ GTM Preview Mode หรือ Tag Assistant เช็คได้ |
| 6 | **GA4 + Google Ads ต้องเชื่อมกัน 2 ทาง** | การสร้าง GA4 อย่างเดียวไม่พอ ต้องเชื่อมกับ Google Ads ผ่าน GA4 → Admin → Google Ads Links การเชื่อมทำให้ข้อมูลไหลระหว่าง 2 ระบบ เห็น GA4 Audience ใน Google Ads สำหรับ Targeting และเห็น Campaign data ใน GA4 สำหรับ Analysis | High | เชื่อม GA4 กับ Google Ads ทันทีหลังสร้าง GA4 Property อย่าลืมขั้นตอนนี้ |
| 7 | **Conversion Tracking: One per click สำหรับ Lead** | การตั้ง Conversion Count มี 2 ตัวเลือก One per click (นับ 1 ต่อ 1 คน) กับ Every conversion (นับทุกครั้ง) สำหรับ Lead Generation ต้องใช้ One per click เพราะถ้าคนเดียวกรอก 3 ครั้ง ไม่ควรนับเป็น 3 Lead ถ้าใช้ผิดตัวเลือก ข้อมูลจะบิดเบือน | Critical | ตอนสร้าง Conversion Action ให้เลือก Category: Lead และ Count: One conversion per click เสมอ |
| 8 | **Install Conversion Tag ผ่าน GTM ง่ายกว่า** | มี 2 วิธีติดตั้ง Conversion Tag: ฝัง Code เอง หรือ ใช้ GTM ถ้าติดตั้ง GTM ไว้แล้ว ให้เลือก Use Google Tag Manager จะได้ Conversion ID + Label ไปสร้าง Tag ใน GTM ง่ายกว่า ปลอดภัยกว่า และแก้ไขสะดวกกว่าการฝัง Code โดยตรง | High | เลือก Install via GTM → สร้าง Conversion Linker Tag + Conversion Tracking Tag ใน GTM |
| 9 | **Billing Threshold เริ่มที่ 1,000 บาท** | Google Ads ใช้ระบบ Automatic Payments เก็บเงินเมื่อถึง Threshold (เริ่มต้น 1,000 บาท) หรือทุก 30 วัน แล้วแต่อันไหนถึงก่อน สำหรับประเทศไทยรองรับ Visa และ Mastercard ทั้งบัตรเครดิตและบัตรเดบิต | Medium | ใส่บัตรที่ Tools → Billing → Payment Methods แนะนำบัตรเครดิตเพื่อความสะดวก ตรวจสอบ Threshold ให้เข้าใจ |
| 10 | **Checklist 6 ข้อ ต้องครบก่อนไปต่อ** | เครื่องมือ 6 รายการ (Google Ads + Youtube Link + GTM + GA4 + Conversion Tracking + Billing) ต้องพร้อมทั้งหมดก่อนไป YTCAMP-005 เพราะตอนต่อไปจะใช้สิ่งที่ตั้งค่าวันนี้เป็นพื้นฐาน ถ้าขาดข้อใดข้อหนึ่งจะติดปัญหาภายหลัง | Critical | ทำ Checklist 6 ข้อให้ครบ ถ้ายังไม่ครบอย่าเพิ่งไป YTCAMP-005 |

---

## สรุป Priority Actions

| Priority | Action | Timeline |
|----------|--------|----------|
| P1 | สร้าง Google Ads Account (Expert Mode, Bangkok, THB) | วันนี้ |
| P2 | เชื่อม Youtube Channel + ติดตั้ง GTM บนเว็บ | วันนี้ |
| P3 | สร้าง GA4 Property + เชื่อมกับ Google Ads | วันที่ 2 |
| P4 | ตั้งค่า Conversion Tracking + Install Tag ผ่าน GTM | วันที่ 2 |
| P5 | ตั้งค่า Billing + ตรวจ Checklist ให้ครบ 6 ข้อ | วันที่ 3 |

---

> ทบทวนต่อ: **YTCAMP-005** — ขั้นตอนเตรียมเครื่องมือ 2
> Series: SWP3 Ch19 Youtube Ads Campaign
> PinkCastle Academy © 2026
