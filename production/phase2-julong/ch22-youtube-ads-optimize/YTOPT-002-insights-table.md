# ตรวจสอบเมนูแคมเปญ — YTOPT-002
> **Format:** Insights Table
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 2
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

## ตาราง 10 Insights สำคัญ

| # | Insight | Detail | Application | Impact Level |
|---|---------|--------|-------------|--------------|
| 1 | เมนู 6 ส่วนครอบคลุมทุกมุมมองการจัดการแคมเปญ | Overview, Campaigns, Ad Groups, Ads, Keywords, Audiences แต่ละเมนูแสดงข้อมูลคนละระดับ ตั้งแต่ภาพรวมไปจนถึงรายละเอียดชิ้นงาน | ทำความรู้จักทุกเมนูก่อน อย่าดูแค่ Overview เมนู Ad Groups และ Ads ช่วยให้เห็นว่าจุดไหนต้องปรับ | สูงมาก |
| 2 | ดูแนวโน้มสำคัญกว่าดูตัวเลขวันเดียว | ตัวเลขวันเดียวผันผวนได้ตามปกติ แต่แนวโน้มที่ลดลงต่อเนื่องบ่งบอก Ad Fatigue หรือคู่แข่งเข้ามาแย่งตลาด | ใช้ Date Range Comparison ทุกครั้ง เปรียบเทียบ This Week vs Last Week, This Month vs Last Month เสมอ | สูงมาก |
| 3 | Filters ตาม Device เผยความแตกต่างที่ซ่อนอยู่ | Mobile vs Desktop มักให้ผลลัพธ์ต่างกันมาก บางแคมเปญ Mobile CTR สูงกว่า 2 เท่า แต่ถ้าดูรวมจะไม่เห็น | กรองตาม Device เป็นอันดับแรก แล้วปรับ Bid Adjustment เพิ่ม Bid สำหรับอุปกรณ์ที่ทำผลงานดี | สูงมาก |
| 4 | การกรองตาม Time ช่วยประหยัดงบได้ 20-40% | ข้อมูล Time Segment ช่วยระบุช่วงเวลาที่คนดูเยอะ คลิกเยอะ สามารถตั้ง Ad Schedule ยิงเฉพาะช่วงที่มีประสิทธิภาพ | วิเคราะห์ Time Segment 2 สัปดาห์ แล้วตั้ง Ad Schedule ตามข้อมูล หยุดยิงช่วงที่ไม่มีคนดู | สูง |
| 5 | Custom Views ประหยัดเวลา 5-10 นาทีทุกครั้งที่เข้าดู | การปรับคอลัมน์ใหม่ทุกครั้งเสียเวลา แต่ถ้าบันทึกเป็น Custom View จะโหลดคอลัมน์ที่ต้องการทันที | สร้าง 2 Views: Quick Check (5 Metrics หลัก) และ Deep Analysis (รวม Conversion + Quality) บันทึกไว้ครั้งเดียว | สูง |
| 6 | Network Segment บอกว่าควรเน้นช่องทางไหน | YouTube Search, YouTube Videos, Display Network ให้ผลลัพธ์ต่างกัน YouTube Videos มักให้ View Rate ดีกว่า Search | กรองตาม Network เปรียบเทียบผลลัพธ์ ถ้า Network ไหนไม่ดีเลยให้ Exclude ออกเพื่อไม่เสียงบ | สูง |
| 7 | Location Segment ช่วยปรับ Geo-Targeting | ไม่ใช่ทุกจังหวัดจะตอบรับเท่ากัน บางพื้นที่ Convert ดีกว่ามาก ข้อมูล Location ช่วยจัดสรรงบได้ตรงจุด | ดู Location Report ทุกสัปดาห์ เพิ่มงบในพื้นที่ที่ Convert ดี ลดงบในพื้นที่ที่ไม่ตอบรับ | สูง |
| 8 | Status Icons ต้องสแกนทุกครั้งก่อนออกจาก Dashboard | แคมเปญที่ Paused หรือ Limited อาจเสียโอกาสโดยไม่รู้ตัว Enabled + Limited อาจหมายถึงงบหมดหรือ Bid ต่ำเกินไป | สแกนสถานะทุกแคมเปญเป็นกิจวัตร ถ้าเห็น Limited ให้กดดูรายละเอียดแล้วแก้ไขทันที | ปานกลาง-สูง |
| 9 | Quick Actions ลดขั้นตอนการจัดการ 50% | เปลี่ยน Budget, Pause/Enable, Edit Settings ได้จากหน้ารายการ ไม่ต้องเข้าไปในแคมเปญทุกครั้ง ประหยัดเวลาและคลิก | ใช้ Quick Actions สำหรับการเปลี่ยนแปลงเล็กน้อย เข้าไปในแคมเปญเฉพาะเมื่อต้อง Optimize ระดับลึก | ปานกลาง-สูง |
| 10 | ความสัมพันธ์ระหว่าง Metrics บอกปัญหาได้ตรงจุด | Impressions เพิ่ม + Clicks ไม่เพิ่ม = โฆษณาไม่ดึงดูด, Clicks เพิ่ม + Conversions ไม่เพิ่ม = Landing Page มีปัญหา | อ่าน Metrics แบบจับคู่เสมอ ไม่ใช่ดูทีละตัว จะระบุจุดที่ต้องแก้ได้แม่นยำกว่า | ปานกลาง |

---

### สรุป Impact Level

| Level | จำนวน Insights |
|-------|---------------|
| สูงมาก | 3 |
| สูง | 4 |
| ปานกลาง-สูง | 2 |
| ปานกลาง | 1 |

---

> ทบทวนต่อ: **YTOPT-003** — ลิงก์ช่อง Youtube กับ Google Ads
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*Insights count: 10 | Focus: Campaign Menu Navigation & Data Filtering*
