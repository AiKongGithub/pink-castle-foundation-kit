# Set Conversion — YTOPT-009 Insights Table
> **Format:** Insights Table
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 9
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:11:11

---

## ตาราง 10 Insights สำคัญ

| # | Insight | Detail | Application | Impact Level |
|---|---------|--------|-------------|--------------|
| 1 | ไม่มี Conversion Tracking = ยิงโฆษณาตาบอด | ถ้าไม่ตั้ง Conversion Tracking เราจะไม่รู้เลยว่าคนที่เห็นโฆษณาทำอะไรต่อ กรอกฟอร์มหรือเปล่า ซื้อหรือเปล่า ทำให้ไม่สามารถ Optimize แคมเปญได้ | ตั้ง Conversion Tracking ก่อนเริ่มยิงโฆษณาทุกครั้ง ห้ามลงโฆษณาก่อนตั้ง Conversion เด็ดขาด เพราะข้อมูลที่ขาดหายจะเอากลับมาไม่ได้ | สูงมาก |
| 2 | Website Actions เป็นประเภท Conversion ที่ใช้บ่อยสุด | ใน 4 ประเภท (Website, Phone, App, Import) ผู้ประกอบการไทยส่วนใหญ่ที่ทำ Landing Page หรือ Sales Funnel ใช้ Website Actions เช่น กรอกฟอร์ม Lead หรือสั่งซื้อบน Thank You Page | เริ่มจาก Website Conversion ก่อน ตั้ง Conversion Action สำหรับกรอกฟอร์ม/สั่งซื้อ แล้วค่อยเพิ่ม Phone Calls หรือ Import ทีหลัง | สูงมาก |
| 3 | Count (Every vs One) เลือกผิดทำให้ข้อมูลบิดเบือน | Every นับทุกครั้งที่เกิด Conversion (ลูกค้า 1 คนซื้อ 3 ครั้ง = 3 Conversions) One นับแค่ครั้งเดียวต่อคน (ลูกค้า 1 คนสมัคร 3 ครั้ง = 1 Conversion) | E-commerce ใช้ Every เพราะทุกรายการสั่งซื้อมีมูลค่า Lead Generation ใช้ One เพราะสนใจแค่ว่าเป็น Lead ใหม่หรือไม่ | สูงมาก |
| 4 | Conversion Window ต้องตรงกับพฤติกรรมลูกค้า | ถ้าตั้ง Window สั้นเกินไป จะนับ Conversion ไม่ครบ (ลูกค้าตัดสินใจช้ากว่า Window) ถ้ายาวเกินไป จะนับ Conversion ที่ไม่เกี่ยวข้องกับโฆษณา | สินค้าราคาถูก/ตัดสินใจเร็ว → 7-14 วัน สินค้าราคาสูง/ต้องคิดนาน → 30-90 วัน ไม่แน่ใจเริ่มที่ 30 วัน (ค่าเริ่มต้น) | สูง |
| 5 | Attribution Model มีผลต่อการวิเคราะห์ช่องทาง | แต่ละ Model ให้เครดิตกับจุดสัมผัสต่างกัน Last Click ให้เครดิตคลิกสุดท้าย Data-driven ให้ Google ML วิเคราะห์ ทำให้ข้อมูลที่เห็นต่างกันอย่างมาก | ผู้เริ่มต้นใช้ Last Click เพราะเข้าใจง่าย พอมีข้อมูลมากขึ้นให้เปลี่ยนเป็น Data-driven เพื่อให้ Google วิเคราะห์ได้แม่นยำกว่า | สูง |
| 6 | Conversion Tag ต้องวางบน Thank You Page เท่านั้น | หลายคนพลาดวาง Tag บนหน้าแรกหรือหน้าสินค้า ทำให้นับ Conversion ผิด ทุกคนที่เข้าหน้านั้นจะถูกนับเป็น Conversion หมด ข้อมูลเสียทั้งระบบ | วาง Conversion Tag เฉพาะหน้าที่แสดงหลังทำ Action สำเร็จ เช่น /thank-you, /order-confirmation ตรวจสอบด้วย Tag Assistant ว่ายิงถูกหน้า | สูง |
| 7 | Google Tag Manager ดีกว่าวางโค้ดตรง | GTM ช่วยจัดการ Tag หลายตัวจากที่เดียว แก้ไขได้โดยไม่ต้องแก้โค้ดเว็บ มี Version Control และ Preview Mode ตรวจสอบก่อน Publish | ติดตั้ง GTM Container บนเว็บไซต์ครั้งเดียว จากนั้นจัดการ Tag ทั้งหมดผ่าน GTM Dashboard ทั้ง Google Ads, Analytics, Facebook Pixel | ปานกลาง-สูง |
| 8 | Conversion Value ช่วยให้ Google Optimize งบอัตโนมัติ | เมื่อกำหนด Value ให้แต่ละ Conversion Google จะรู้ว่า Conversion ไหนมีมูลค่ามากกว่า ช่วยจัดสรรงบไปที่ Conversion มูลค่าสูงให้อัตโนมัติ | ตั้ง Value ที่สะท้อนมูลค่าจริง เช่น Lead 1 คน = 500 บาท, Purchase = ราคาสินค้า สำหรับ E-commerce ใช้ Dynamic Value ส่งราคาจริงมาได้ | ปานกลาง-สูง |
| 9 | สถานะ Inactive ต้องแก้ไขทันที | Inactive หมายถึง Conversion Tag ไม่ทำงาน ทำให้สูญเสียข้อมูลทุกวันที่ไม่แก้ไข Google ไม่สามารถ Optimize แคมเปญให้ได้อย่างถูกต้อง | ตรวจสอบ 4 จุด — Tag วางถูกหน้าไหม, Tag Assistant ตรวจผ่านไหม, Conversion ID/Label ถูกไหม, ลองทำ Test Conversion ด้วยตัวเอง | ปานกลาง-สูง |
| 10 | ทำ Test Conversion ก่อนเริ่มลงโฆษณาจริง | หลังติดตั้ง Tag เสร็จ ต้องทดสอบด้วยตัวเอง เข้าเว็บจากโฆษณาทดสอบ กรอกฟอร์มจริง แล้วดูว่า Conversion ถูกบันทึกหรือไม่ ไม่ควรเดาว่าทำงานถูกต้อง | สร้างโฆษณาทดสอบ คลิกเข้าเว็บ กรอกฟอร์ม/สั่งซื้อจริง รอ 24-48 ชั่วโมง ตรวจสอบว่า Conversion ปรากฏในรายงาน Google Ads | ปานกลาง |

---

### สรุป Impact Level

| Level | จำนวน Insights |
|-------|---------------|
| สูงมาก | 3 |
| สูง | 3 |
| ปานกลาง-สูง | 3 |
| ปานกลาง | 1 |

---

> ทบทวนต่อ: **YTOPT-010** — Google กับ Kartra ทำงานร่วมกัน
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*Insights count: 10 | Focus: Conversion Tracking Setup & Validation*
