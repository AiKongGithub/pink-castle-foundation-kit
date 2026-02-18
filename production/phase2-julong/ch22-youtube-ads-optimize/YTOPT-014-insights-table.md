# วิธีปรับแต่งแคมเปญ Advance ตอน 1 — YTOPT-014 Insights Table
> **Format:** Insights Table
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 14
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:50:18

---

## ตาราง 10 Insights สำคัญ

| # | Insight | Detail | Application | Impact Level |
|---|---------|--------|-------------|--------------|
| 1 | รอ 7 วันก่อนปรับแคมเปญ ข้อมูลน้อยกว่านี้ไม่ Reliable | Learning Phase ต้องใช้เวลาอย่างน้อย 7 วันเพื่อให้ระบบเรียนรู้ว่าโฆษณาเหมาะกับใคร การปรับเร็วเกินไปทำให้ได้ข้อมูลผิดเพี้ยน เหมือนปลูกต้นไม้แล้วขุดดูรากทุกวัน | ตั้งกฎเหล็กว่าห้ามปรับก่อน 7 วัน ทำเครื่องหมายในปฏิทินว่าวันไหนครบ 7 วัน ถ้าไม่แน่ใจให้รอเพิ่ม ยิ่งมีข้อมูลเยอะยิ่งตัดสินใจแม่นยำ | สูงมาก |
| 2 | วิเคราะห์ 3 Metrics: Conversion Rate, Cost per Conversion, ROAS | ไม่ใช่แค่ดู CTR หรือ Views เท่านั้น ต้องดูว่าคนทำ Conversion ไหม (Conversion Rate) ต้นทุนต่อ Conversion เท่าไร (Cost per Conversion) และได้กลับมาคุ้มไหม (ROAS) ข้อมูลเหล่านี้บอกได้ว่าแคมเปญทำเงินได้จริงหรือแค่มีคนดู | เข้า Campaign → ดู Conversion columns ถ้า Conversion Rate ต่ำ = โฆษณาหรือ Landing Page มีปัญหา ถ้า Cost per Conversion สูง = ต้องปรับ Bidding/Audience ถ้า ROAS ต่ำ = ต้องทบทวนทั้งระบบ | สูงมาก |
| 3 | ต้องเจาะลึกตาม Ad Group, Audience, Device ไม่ใช่ดูแค่ภาพรวม | ภาพรวมอาจดูดี แต่ซ่อนปัญหาไว้ เช่น Ad Group A อาจมี ROAS 5x แต่ Ad Group B มี ROAS 0.5x ค่าเฉลี่ยรวมดูพอไปได้ แต่จริงๆ เสียเงินไปกับ B โดยไม่รู้ตัว | ดูข้อมูลใน Tab "Ad Groups", "Audiences", "Devices" แยกวิเคราะห์ทีละ Dimension หาจุดที่ดีเพื่อขยาย หาจุดที่ไม่ดีเพื่อตัด | สูงมาก |
| 4 | เปลี่ยนจาก Manual CPC เป็น Target CPA เมื่อมี 30-50 Conversions | Manual CPC ดีตอนเริ่มเพราะควบคุมได้ แต่เมื่อมี Conversion พอ Target CPA จะ Optimize ได้ดีกว่าเพราะใช้ Machine Learning เงื่อนไขคือต้องมี 30-50 Conversions ใน 30 วัน น้อยกว่านี้ระบบจะ Optimize ผิดทิศ | นับ Conversions ใน 30 วัน ถ้าถึง 30-50 ให้เปลี่ยน Bidding Strategy ตั้ง Target CPA = Cost per Conversion ปัจจุบัน แล้วค่อยๆ ลด 10-15% ต่อสัปดาห์ | สูงมาก |
| 5 | Audience ที่ไม่มี Conversion ต้อง Exclude ไม่ใช่แค่ลด Bid | หลายคนแค่ลด Bid สำหรับ Audience ที่ไม่ดี แต่ยังเสียเงินอยู่ การ Exclude ออกไปเลยหยุดเสียเงินทันที และให้งบไปกับ Audience ที่ดีแทน | ดู Audience Segments ที่มี 0 Conversions หลัง 14 วัน ให้ Exclude ออก สร้าง Ad Group ใหม่เจาะ Audience ที่ Conversion Rate สูง เพิ่มงบให้ | สูง |
| 6 | Similar Audiences ช่วยขยาย Reach โดยยังรักษาคุณภาพ | Google จะหาคนที่มีลักษณะคล้ายกับคนที่ Converted แล้ว เหมือน Lookalike Audience ของ Facebook ช่วยขยายกลุ่มเป้าหมายโดยไม่ต้องเดา | สร้าง Remarketing List จากคนที่ Converted เลือก "Similar to" ใน Google Ads เริ่มทดสอบด้วยงบน้อยก่อน เปรียบเทียบกับ Audience เดิม | สูง |
| 7 | A/B Testing ต้องเปลี่ยนแค่ 1 อย่าง รอ 2 สัปดาห์ | ถ้าเปลี่ยนหลายอย่างพร้อมกัน จะไม่รู้ว่าอะไรทำให้ดีขึ้นหรือแย่ลง ต้องควบคุมตัวแปร เปลี่ยนแค่ Headline หรือ CTA หรือวิดีโอ อย่างใดอย่างหนึ่ง แล้วรอข้อมูลเพียงพอ | สร้าง 2 Ad Variants ใน Ad Group เดียวกัน ต่างกันแค่ 1 จุด รอ 2 สัปดาห์ ตัวไหนดีกว่าปิดอีกตัว สร้าง Variant ใหม่ทดสอบต่อ วนซ้ำ | สูง |
| 8 | Responsive Ads ให้ Google ผสมคอมบิเนชันที่ดีที่สุดเอง | แทนที่จะเดาว่า Headline ไหนคู่กับ Description ไหนดีที่สุด ให้ใส่หลายตัวเลือกแล้ว Machine Learning ทำงานให้ ระบบจะเรียนรู้ว่าแต่ละกลุ่มคนตอบสนองกับคอมบิเนชันไหนดีที่สุด | ใส่ Headlines 3-5 ตัว Description 2-3 ตัว ให้หลากหลาย อย่าซ้ำกัน ดู Asset Performance Report ว่าตัวไหนทำงานได้ดี ตัวไหนต้องเปลี่ยน | ปานกลาง-สูง |
| 9 | Mobile มี Traffic สูง แต่ Desktop อาจมี Conversion Rate สูงกว่า | ในตลาดไทย Mobile มีคนใช้มากที่สุด แต่คนมักจะ Research บน Mobile แล้ว Convert บน Desktop เพราะสะดวกกรอกฟอร์มหรือชำระเงินมากกว่า ถ้าไม่แยก Device ดูจะเสียเงินไปกับ Mobile โดยไม่ได้ Conversion | ไปที่ Tab "Devices" ดู Conversion Rate ตาม Device ปรับ Bid Adjustment เช่น Desktop +20-30% ถ้า Conversion Rate สูง Mobile -10-20% ถ้า Performance ต่ำกว่า | ปานกลาง-สูง |
| 10 | Schedule Optimization ประหยัดงบได้ 20-30% | โฆษณาไม่จำเป็นต้องแสดงตลอด 24 ชั่วโมง บางช่วงเวลาคนไม่สนใจเลย เช่น ตี 2-5 การหยุดแสดงช่วงนี้ประหยัดงบโดยไม่เสีย Conversion และเพิ่ม Bid ในช่วงเวลาทองเพื่อชนะ Auction มากขึ้น | ดู Report ตาม Day of Week และ Hour of Day หาช่วงเวลาที่ CTR และ Conversion Rate สูง/ต่ำ ปรับ Ad Schedule เพิ่ม Bid ช่วงดี ลด/หยุดช่วงไม่ดี | ปานกลาง-สูง |

---

### สรุป Impact Level

| Level | จำนวน Insights |
|-------|---------------|
| สูงมาก | 4 |
| สูง | 3 |
| ปานกลาง-สูง | 3 |

---

> ทบทวนต่อ: **YTOPT-015** — วิธีปรับแต่งแคมเปญ Advance ตอน 2
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*Insights count: 10 | Focus: Advanced Campaign Optimization — Analysis, Bidding, Audience, Creative, Device, Schedule*
