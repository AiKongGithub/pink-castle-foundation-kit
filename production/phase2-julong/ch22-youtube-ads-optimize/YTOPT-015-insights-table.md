# วิธีปรับแต่งแคมเปญ Advance ตอน 2 — YTOPT-015 Insights Table
> **Format:** Insights Table
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 15
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:52:20

---

## ตาราง 10 Insights สำคัญ

| # | Insight | Detail | Application | Impact Level |
|---|---------|--------|-------------|--------------|
| 1 | Remarketing มี Conversion Rate สูงกว่าคนใหม่ 3-5 เท่า | คนที่เคยดูวิดีโอ เข้าเว็บ หรือ Subscribe รู้จักเราแล้ว ความไว้วางใจสูงกว่า ต้นทุนต่ำกว่า เหมือนไปจีบคนที่เคยยิ้มให้เราแล้ว โอกาสสำเร็จสูงกว่าจีบคนแปลกหน้า | เข้า Tools & Settings → Audience Manager → สร้าง YouTube Users Audience เลือกประเภท (Viewed, Subscribed, Visited) ตั้ง Membership Duration 30-90 วัน สร้างแคมเปญ Remarketing แยกจากแคมเปญปกติ | สูงมาก |
| 2 | Video Remarketing Lists แยกตามระดับความสนใจได้ | คนดูจนจบมีความตั้งใจสูงกว่าคนดูแค่ 5 วินาที คนที่ Subscribe สนใจมากกว่าคนที่แค่ดู การแยก List ตามพฤติกรรมทำให้ปรับ Message ได้ตรงจุด เช่น คนดูจนจบอาจพร้อมซื้อ แต่คนดู 5 วินาทีต้อง Educate เพิ่ม | สร้าง Remarketing List หลายตัวแยกตามพฤติกรรม — Viewed any video, Viewed to completion, Subscribed, Visited website สร้าง Ad ที่แตกต่างกันสำหรับแต่ละ List | สูงมาก |
| 3 | Custom Intent Audiences นำ Search Intent มาใช้กับ Video Ads | คนที่พิมพ์ค้นหา Keywords เฉพาะใน Google แสดงความตั้งใจชัดเจน เราสามารถแสดง YouTube Ads ให้คนกลุ่มนี้ได้ เท่ากับจับ Intent จาก Search มาใช้ใน Video Channel | สร้าง Custom Segments → เลือก "People who searched for any of these terms" ใส่ Keywords ที่เกี่ยวข้อง เริ่มด้วยงบน้อยก่อน เพราะ Audience อาจกว้างกว่าที่คิด ดู Performance 2 สัปดาห์ | สูงมาก |
| 4 | ใส่ URL Competitor ใน Custom Intent เพื่อดึง Audience คู่แข่ง | Google จะหาคนที่มีพฤติกรรมคล้ายผู้เข้าชมเว็บไซต์ Competitor แล้วแสดงโฆษณาให้เรา เป็นกลยุทธ์ Competitive Targeting ที่ทรงพลัง ไม่ต้องสร้าง Audience จากศูนย์ | ไปที่ Custom Segments → ใส่ URL ของคู่แข่ง 3-5 เว็บ ผสมกับ Keywords ที่เกี่ยวข้อง แยก Ad Group เพื่อดู Performance ของ URL-based vs Keyword-based | สูง |
| 5 | Performance Max ต้องมี Conversion Data เดิมก่อน อย่างน้อย 30/เดือน | PMax ใช้ AI จัดการทุกอย่าง แต่ AI ต้องมีข้อมูลเรียนรู้ ถ้าเริ่มจาก PMax เลยโดยไม่มี Conversion Data ระบบจะไม่รู้ว่าต้องหาคนแบบไหน ผลลัพธ์จะไม่ดี ต้องรันแคมเปญปกติจนมีข้อมูลก่อน | ตรวจสอบว่ามี Conversion อย่างน้อย 30 ครั้งต่อเดือนจากแคมเปญปกติ ถ้าถึงแล้วค่อยเปิด PMax เพิ่ม ใส่ Assets ให้เยอะที่สุด — Headlines 5-15, Description 2-5, รูป/วิดีโอหลายตัว | สูงมาก |
| 6 | PMax แสดงในทุก Channel แต่ควบคุมไม่ได้ว่าไปที่ไหน | ข้อดีคือ Reach กว้าง (YouTube, Search, Display, Gmail, Maps) ข้อเสียคือไม่รู้ว่าโฆษณาไปแสดงที่ไหน Audience ไหนเห็น ทำให้วิเคราะห์ยาก เหมาะสำหรับคนที่ต้องการ Volume มากกว่าการควบคุม | ใช้ PMax เป็นแคมเปญเสริม ไม่ใช่แคมเปญหลัก ยังคงรันแคมเปญ YouTube ปกติที่ควบคุมได้ เปรียบเทียบ ROAS ระหว่าง PMax กับแคมเปญปกติ | สูง |
| 7 | Looker Studio Dashboard อัพเดทอัตโนมัติ แชร์ทีมได้ | ไม่ต้อง Export ไฟล์ ไม่ต้องเข้า Google Ads ทุกวัน ทีมทุกคนเห็นข้อมูลเดียวกัน เหมาะสำหรับการรายงานผลให้ผู้บริหารหรือลูกค้า มี Date Range Filter เปรียบเทียบ Period ได้ง่าย | เชื่อมต่อ Looker Studio กับ Google Ads ใส่ Metrics หลัก: Spend, Impressions, Views, CTR, Conversions, Cost per Conversion, ROAS แยกตามแคมเปญ ใส่ Date Range Filter | ปานกลาง-สูง |
| 8 | เพิ่มงบทีละ 20-30% ต่อสัปดาห์ เพิ่มมากกว่านี้จะ Reset Learning Phase | ระบบ Machine Learning เรียนรู้จากข้อมูลปัจจุบัน ถ้าเปลี่ยนงบมากเกินไปทีเดียว (เช่น +100%) ระบบจะถือว่าเป็นสถานการณ์ใหม่ ต้อง Learn ใหม่ Performance จะตกชั่วคราว ค่อยๆ เพิ่มทำให้ระบบปรับตัวได้ | เมื่อแคมเปญมี ROAS ดี เพิ่มงบ 20-30% ต่อสัปดาห์ Monitor Cost per Conversion ทุกสัปดาห์ ถ้า CPC เพิ่มเกิน 20% จากเดิม ให้หยุด Scale แล้ว Optimize ก่อน | สูงมาก |
| 9 | Plateau Effect — ทุกแคมเปญมีจุดที่เพิ่มงบแล้วไม่คุ้ม | เมื่อ Audience เริ่มอิ่มตัว เพิ่มงบไปก็ได้แค่ Impressions ซ้ำคนเดิม Cost per Conversion จะสูงขึ้นเรื่อยๆ ทางออกคือขยาย Audience ใหม่ หรือสร้างแคมเปญใหม่ ไม่ใช่เทงบลงแคมเปญเดิมเรื่อยๆ | เมื่อ Cost per Conversion เพิ่มขึ้นเรื่อยๆ ถึงแม้เพิ่มงบไม่มาก ให้ Clone แคมเปญ เปลี่ยน Audience เป็น Similar/Custom Intent ใหม่ หรือเปลี่ยน Creative เพื่อเข้าถึงคนกลุ่มใหม่ | สูง |
| 10 | Chapter 22 ครบ 15 ตอน = พร้อมจัดการ YouTube Ads อย่างมืออาชีพ | จาก Beginner (ตอน 1-5 พื้นฐาน) สู่ Intermediate (ตอน 6-10 เครื่องมือ) สู่ Pre-Advanced (ตอน 11-13 ปฏิบัติจริง) สู่ Advanced (ตอน 14-15 Optimization + Scaling) ครบทุกทักษะที่ต้องใช้ในการจัดการแคมเปญ YouTube Ads | ทบทวนเนื้อหาทั้ง 15 ตอน สร้าง Checklist จากแต่ละตอน ลงมือทำจริงกับแคมเปญจริง บันทึกผลลัพธ์และ Learnings กลับมาทบทวนเมื่อเจอปัญหา | สูง |

---

### สรุป Impact Level

| Level | จำนวน Insights |
|-------|---------------|
| สูงมาก | 4 |
| สูง | 4 |
| ปานกลาง-สูง | 2 |

---

> จบ Chapter 22: วิธีปรับแต่งแคมเปญ Youtube Ads — 15 ตอน
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*Insights count: 10 | Focus: Remarketing, Custom Intent, Performance Max, Reporting, Scaling Strategy*
