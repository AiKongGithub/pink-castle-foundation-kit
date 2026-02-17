# Insights Table: วิธีปรับแต่ง Blog Settings — WEB2-005
> **Format:** Insights Table (10 Rows)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 5
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

| # | Insight (ข้อค้นพบ) | Detail (รายละเอียด) | Application (การนำไปใช้) | Impact Level (ระดับผลกระทบ) |
|---|---|---|---|---|
| 1 | Layout ที่เลือกส่งผลต่อพฤติกรรมผู้อ่าน | Grid Layout ดึงดูดด้วยภาพ ผู้อ่านจะ scan ด้วยสายตา / List Layout เหมาะกับการอ่านเนื้อหา ผู้อ่านจะอ่านจากบนลงล่าง / Masonry เหมาะกับเนื้อหาหลากหลาย | เลือก Layout ตามประเภทเนื้อหาหลักของบล็อก ถ้าเน้นภาพใช้ Grid ถ้าเน้นบทความใช้ List | สูง |
| 2 | Post Excerpt ที่เหมาะสมช่วยเพิ่ม CTR | ข้อความสรุปที่สั้นเกินจะไม่ดึงดูด ยาวเกินจะทำให้หน้ารก ความยาว 20-55 คำคือจุดที่เหมาะสมที่สุด | กำหนดความยาว Excerpt ผ่าน Theme Customizer หรือ functions.php ตรวจสอบผลลัพธ์บนหน้าจอจริง | กลาง |
| 3 | Featured Image จำเป็นสำหรับทุกบทความ | บทความที่มี Featured Image ได้ engagement สูงกว่า 2-3 เท่า เมื่อแชร์ใน Social Media จะมีรูปแสดง เพิ่มโอกาสคลิก | สร้างนิสัยตั้ง Featured Image ทุกครั้งที่เขียนบทความ เตรียม template รูปภาพไว้ล่วงหน้าเพื่อความสม่ำเสมอ | สูง |
| 4 | Category และ Tag ช่วยทั้ง UX และ SEO | Category จัดกลุ่มบทความเป็นหมวดหมู่ใหญ่ Tag เชื่อมบทความข้ามหมวดหมู่ ทั้งสองสร้าง internal link structure ที่ Google ชอบ | แสดง Category และ Tag บนหน้าบล็อก วางแผนโครงสร้าง Category ให้ชัดเจน ใช้ Tag ไม่เกิน 5-10 ต่อบทความ | สูง |
| 5 | Author Info สร้าง E-E-A-T | Google ใช้ E-E-A-T (Experience, Expertise, Authoritativeness, Trustworthiness) ในการจัดอันดับ การแสดงข้อมูลผู้เขียนช่วยยืนยันความเชี่ยวชาญ | เปิด Author Info ใส่ประวัติและรูปจริง ลิงก์ไปยัง Social Media ของผู้เขียน โดยเฉพาะเว็บที่มีหลายนักเขียน | กลาง |
| 6 | Related Posts ลด Bounce Rate ได้ 15-25% | เมื่อผู้อ่านเห็นบทความที่เกี่ยวข้องท้ายบทความ จะมีโอกาสคลิกอ่านต่อสูง ทำให้ Pageviews เพิ่มขึ้นและเวลาที่อยู่ในเว็บนานขึ้น | เปิดใช้ Related Posts แสดงท้ายทุกบทความ เลือกแสดง 3-6 บทความ พร้อมรูป Thumbnail | สูง |
| 7 | Social Sharing เลือกน้อยแต่ตรงจุดดีกว่า | ปุ่มแชร์เยอะเกินไปทำให้ผู้อ่านตัดสินใจไม่ได้ (Paradox of Choice) เลือก 3-5 แพลตฟอร์มที่กลุ่มเป้าหมายใช้จริง | สำหรับตลาดไทยใช้ Facebook + LINE + Twitter เป็นหลัก วางปุ่มท้ายบทความ พิจารณา Floating Sidebar สำหรับบทความยาว | กลาง |
| 8 | Comments Section ต้องมี Moderation | คอมเมนต์ที่ไม่ควบคุมจะมี spam และคอมเมนต์ที่ไม่เหมาะสม ส่งผลเสียต่อภาพลักษณ์เว็บไซต์และ SEO | เปิด Comment Moderation ให้ต้องอนุมัติก่อนแสดง ใช้ Threaded Comments เพื่อการสนทนาที่เป็นระเบียบ | กลาง |
| 9 | Sidebar ที่ดีใส่ Widget ไม่เกิน 4-5 ตัว | Sidebar ที่มี Widget เยอะเกินไปทำให้ผู้อ่านเสียสมาธิ Widget ที่จำเป็นที่สุดคือ Search Bar และ Recent Posts | เลือก Widget ที่ผู้อ่านจะใช้จริงเท่านั้น จัดลำดับ Search Bar ไว้บนสุด ตามด้วย Recent Posts และ Categories | กลาง |
| 10 | Numbered Pagination ดีที่สุดสำหรับ SEO | Google Bot สามารถ crawl หน้าที่มี Numbered Pagination ได้ดีกว่า Infinite Scroll ส่งผลให้บทความทุกชิ้นถูก index ครบถ้วน | ใช้ Numbered Pagination เป็นค่าเริ่มต้น แสดง 10-15 บทความต่อหน้า พิจารณา Load More สำหรับ Mobile | สูง |

---

## สรุปตาม Impact Level

| ระดับ | จำนวน Insights | หัวข้อหลัก |
|-------|:---:|---|
| สูง | 5 | Layout, Featured Image, Category/Tag, Related Posts, Pagination |
| กลาง | 5 | Post Excerpt, Author Info, Social Sharing, Comments, Sidebar |
| ต่ำ | 0 | — |

---

*จำนวน Insights ทั้งหมด: 10 รายการ*
