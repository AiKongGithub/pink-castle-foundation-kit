# ขั้นตอนเตรียมเครื่องมือ 1 — YTCAMP-004 Flashcards
> Format: Flashcards (12 Cards)
> Source: SWP3 Ch19 Youtube Ads Campaign ตอนที่ 4
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 0:06:38

---

=== CARD 1 ===
Q: เครื่องมือหลัก 4 ตัวที่ต้องเตรียมก่อนทำ Youtube Ads Campaign คืออะไร?
A: **(1) Google Ads** — ศูนย์บัญชาการสร้างและจัดการโฆษณา **(2) Youtube Channel** — เชื่อมเพื่อเข้าถึง Video Assets **(3) Google Tag Manager (GTM)** — จัดการ Tracking Tag ทั้งหมดจากจุดเดียว **(4) Google Analytics 4 (GA4)** — วิเคราะห์พฤติกรรมผู้ใช้และวัดผลแคมเปญ ทั้ง 4 ตัวเป็นของ Google ใช้ Gmail account เดียวจัดการได้หมด

---

=== CARD 2 ===
Q: ทำไมต้องเลือก Expert Mode แทน Smart Campaign ใน Google Ads?
A: **Expert Mode** ให้เราควบคุมได้ทุกอย่าง ตั้งแต่ **Bidding Strategy, Audience Targeting, Ad Placement** ไปจนถึงงบประมาณ ส่วน **Smart Campaign** ให้ Google ตัดสินใจทุกอย่างแทน ควบคุมอะไรแทบไม่ได้เลย สำหรับ Youtube Ads ที่ต้องการความแม่นยำในการ Target กลุ่มเป้าหมาย **Expert Mode เป็นสิ่งจำเป็น**

---

=== CARD 3 ===
Q: การตั้งค่า Time Zone และ Currency ใน Google Ads มีอะไรที่ต้องระวัง?
A: ต้องตั้งให้ถูกตั้งแต่แรกเลย คือ **Time Zone: Bangkok (GMT+7)** และ **Currency: THB (บาท)** เพราะ **Google Ads ไม่อนุญาตให้เปลี่ยนภายหลัง** ถ้าตั้งผิดต้องสร้างบัญชีใหม่ทั้งหมด นี่คือจุดที่คนพลาดบ่อยที่สุดในขั้นตอนการสร้างบัญชี

---

=== CARD 4 ===
Q: การเชื่อม Youtube Channel กับ Google Ads ทำอย่างไร และมีประโยชน์อะไร?
A: **วิธีเชื่อม:** Google Ads → Tools & Settings → Linked accounts → YouTube → คลิก Link → ใส่ URL ของ Channel → Approve **ประโยชน์ 2 ข้อ:** **(1)** เข้าถึง Video Assets ของเราโดยตรงสำหรับทำโฆษณา **(2)** เห็นข้อมูลว่าคนที่ดูวิดีโอเราไปทำอะไรต่อ ซึ่งมีค่ามากสำหรับ **Retargeting**

---

=== CARD 5 ===
Q: Google Tag Manager (GTM) คืออะไร และทำไมต้องใช้?
A: GTM เปรียบเหมือน **กล่องเครื่องมือ** สำหรับจัดการ Tracking Code ทั้งหมด แทนที่จะฝัง Code ของ Google Ads, GA4, Facebook Pixel ลงในเว็บไซต์โดยตรง เราฝังแค่ **GTM Code อันเดียว** แล้วจัดการ Tag ต่างๆ ผ่าน GTM Dashboard ได้หมด **ง่ายต่อการเพิ่ม แก้ไข หรือลบ Tag โดยไม่ต้องแก้โค้ดเว็บ**

---

=== CARD 6 ===
Q: ขั้นตอนติดตั้ง GTM บนเว็บไซต์ทำอย่างไร?
A: **(1)** เข้า tagmanager.google.com → สร้าง Account ใหม่ **(2)** ตั้งชื่อ Container ให้ตรงกับเว็บไซต์ **(3)** เลือก Container Type เป็น **Web** **(4)** GTM จะให้โค้ด **2 ชุด** — ชุดแรกใส่ใน `<head>` ชุดที่สองใส่หลัง `<body>` tag เปิด **(5)** ต้องใส่ **ทุกหน้า** ของเว็บไซต์ ถ้าใช้ Systeme.io หรือ Kartra ไปวางในช่อง Tracking Code ได้เลย

---

=== CARD 7 ===
Q: GA4 Property สร้างอย่างไร และต้องเชื่อมอะไรเพิ่ม?
A: **สร้าง GA4:** เข้า analytics.google.com → สร้าง Property ใหม่ → เลือก Data Stream เป็น **Web** → ใส่ URL เว็บไซต์ **เชื่อมกับ Google Ads:** GA4 → Admin → **Google Ads Links** → Link → เลือก Google Ads Account ที่สร้างไว้ การเชื่อมนี้ทำให้ **ข้อมูลไหลระหว่าง 2 ระบบ** — เห็น Audience ใน Google Ads และเห็นข้อมูลแคมเปญใน GA4

---

=== CARD 8 ===
Q: Conversion Tracking ใน Google Ads ตั้งค่าอย่างไร?
A: **(1)** Google Ads → Tools → Conversions → **New Conversion Action** **(2)** เลือก **Website** → ใส่ URL ของ Thank You Page **(3)** ตั้งชื่อให้เข้าใจ เช่น "Lead Form Submission" **(4)** เลือก Category เป็น **Lead** **(5)** ตั้ง Value เป็น 1 **(6)** Count เลือก **One conversion per click** (นับ Lead ไม่ใช่ Transaction) **(7)** Install Tag ผ่าน GTM → สร้าง Conversion Linker Tag + Conversion Tracking Tag

---

=== CARD 9 ===
Q: ทำไมต้องเลือก "One conversion per click" สำหรับ Youtube Ads Campaign?
A: เพราะเราต้องการ **นับ Lead ไม่ใช่นับ Transaction** ถ้าคนๆ เดียวกรอกฟอร์ม 3 ครั้ง (จาก 3 คลิก) ในโหมด **One per click** จะนับเป็น 1 Conversion (เพราะเป็นคนเดียวกัน) แต่ถ้าใช้ **Every conversion** จะนับเป็น 3 ซึ่งทำให้ข้อมูลบิดเบือน สำหรับ Lead Generation ต้องใช้ **One per click** เสมอ

---

=== CARD 10 ===
Q: ระบบ Billing ของ Google Ads ทำงานอย่างไร?
A: Google Ads ใช้ระบบ **Automatic Payments** คือเก็บเงินหลังจากใช้งาน โดยจะเก็บเมื่อถึง **Threshold** (ปกติเริ่มที่ **1,000 บาท**) หรือ **ทุก 30 วัน** แล้วแต่อันไหนถึงก่อน สำหรับประเทศไทยรองรับ **Visa และ Mastercard** ทั้งบัตรเครดิตและบัตรเดบิต ตั้งค่าที่ Tools → Billing → Payment Methods

---

=== CARD 11 ===
Q: ทำไมควรใช้ Google Account เดียวจัดการเครื่องมือทั้งหมด?
A: เพราะเครื่องมือทั้ง 4 ตัว (Google Ads, Youtube, GTM, GA4) เป็นของ **Google ทั้งหมด** การใช้ Account เดียวทำให้ **(1)** เชื่อมเครื่องมือได้ง่าย ไม่ต้องขอ Permission ข้ามบัญชี **(2)** ข้อมูลไหลระหว่างระบบได้สะดวก **(3)** จัดการ Billing จากที่เดียว **(4)** ไม่สับสนว่า Account ไหนเชื่อมกับอะไร

---

=== CARD 12 ===
Q: สรุป Checklist 6 ข้อที่ต้องทำให้ครบก่อนไปตอนต่อไป?
A: **(1) Google Ads Account** — สร้างแล้ว Expert Mode, Time Zone Bangkok, Currency THB **(2) Youtube Channel** — เชื่อมกับ Google Ads แล้ว **(3) GTM** — สร้าง Container + ติดตั้งโค้ดบนเว็บแล้ว **(4) GA4** — สร้าง Property + เชื่อมกับ Google Ads แล้ว **(5) Conversion Tracking** — สร้าง Conversion Action + Install Tag แล้ว **(6) Billing** — ใส่บัตรชำระเงินแล้ว ถ้ายังไม่ครบ **อย่าเพิ่งไปตอน YTCAMP-005**

---

> ทบทวนต่อ: **YTCAMP-005** — ขั้นตอนเตรียมเครื่องมือ 2
> Series: SWP3 Ch19 Youtube Ads Campaign
> PinkCastle Academy © 2026
