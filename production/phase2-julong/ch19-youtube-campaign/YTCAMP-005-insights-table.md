# ขั้นตอนเตรียมเครื่องมือ 2 — YTCAMP-005 Insights Table
> Format: Insights Table (10 rows)
> Source: SWP3 Ch19 Youtube Ads Campaign ตอนที่ 5
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 0:06:09

---

| # | Insight | รายละเอียด | ระดับสำคัญ | การนำไปใช้ |
|---|---------|-----------|-----------|-----------|
| 1 | **Remarketing เพิ่มโอกาสซื้อ 3-5 เท่า** | คนที่เคยมีปฏิสัมพันธ์กับเราแล้ว (เข้าเว็บ ดูวิดีโอ เป็นลูกค้าเดิม) มีโอกาสซื้อสูงกว่าคนใหม่ 3-5 เท่า ต้องสร้าง Remarketing Lists ไว้ตั้งแต่ก่อนปล่อยแคมเปญ เพราะระบบจะเริ่มเก็บข้อมูลทันที ยิ่งเริ่มเร็วยิ่งมี Audience พร้อมใช้มาก | Critical | สร้าง Remarketing Lists ทั้ง 3 แบบ (Website Visitors, Video Viewers, Customer Lists) วันนี้เลย อย่ารอจนปล่อยแคมเปญ |
| 2 | **Remarketing 3 แบบ ใช้คนละจังหวะ** | Website Visitors สำหรับ Retargeting คนเข้าเว็บ (ต้องมี GTM+GA4 พร้อม) Video Viewers สำหรับคนดูวิดีโอ (ต้อง Link Youtube Channel แล้ว) Customer Lists สำหรับ Upsell ลูกค้าเดิม (อัปโหลด CSV) แต่ละแบบเหมาะกับกลยุทธ์ต่างกัน | High | เลือกแบบที่เหมาะกับเป้าหมาย ถ้าเพิ่งเริ่มให้เน้น Video Viewers ก่อนเพราะตั้งค่าง่ายที่สุด |
| 3 | **Custom Intent = Bottom Funnel, Custom Affinity = Top Funnel** | Custom Intent Audience คือคนที่กำลังค้นหาสิ่งที่เกี่ยวกับสินค้าเรา เหมาะกับ Bottom Funnel คนพร้อมซื้อ ส่วน Custom Affinity คือคนที่มีไลฟ์สไตล์ตรงกับแบรนด์ เหมาะกับ Top Funnel สร้าง Awareness ใช้ร่วมกันจะครอบคลุมทุกขั้น Funnel | Critical | สร้างทั้ง Custom Intent (ใส่ Keywords/URL เกี่ยวกับสินค้า) และ Custom Affinity (ใส่ Interest/ไลฟ์สไตล์ของกลุ่มเป้าหมาย) |
| 4 | **Youtube Channel ต้อง Optimize ไม่ใช่แค่มี** | Channel Art ต้องสื่อสารชัด About ต้องมี Keywords Links ต้องใส่ครบ และที่สำคัญที่สุดคือ Featured Video สำหรับคนที่ยังไม่ Subscribe เพราะคนที่คลิกจาก Ads แล้วเข้า Channel จะเห็นวิดีโอนี้เป็นอันดับแรก ต้องประทับใจตั้งแต่วินาทีแรก | High | Optimize ทั้ง 4 จุด: Channel Art + About + Links + Featured Video ก่อนปล่อย Ads |
| 5 | **70% ดู Youtube บนมือถือ Landing Page ต้อง Mobile-First** | คนส่วนใหญ่ดู Youtube บนมือถือ ถ้า Landing Page ไม่ Mobile-Responsive งบโฆษณาทั้งหมดสูญเปล่า ต้องทดสอบบนมือถือจริง ไม่ใช่แค่ดูบน Desktop แล้วคิดว่าพอ ถ้าโหลดช้าเกิน 3 วินาที มากกว่า 50% กดปิดทิ้ง | Critical | ทดสอบ Landing Page บนมือถือจริง + Google PageSpeed Insights คะแนนต้องเกิน 70 |
| 6 | **GTM Preview Mode = ด่านตรวจสุดท้ายก่อนปล่อย Ads** | ถ้า Tag ไม่ Fire ข้อมูลก็ไม่เข้า Conversion ก็นับไม่ได้ เงินจ่ายแต่วัดผลไม่ได้ GTM Preview Mode แสดงว่า Tag ไหน Fire แล้ว Tag ไหนยังไม่ Fire ต้องทดสอบทั้ง Homepage (Container Tag) และ Thank You Page (Conversion Tag) ใช้ร่วมกับ Google Tag Assistant เสริมความมั่นใจ | Critical | ก่อนปล่อยแคมเปญทุกครั้ง ต้องเข้า GTM Preview Mode + Tag Assistant ตรวจสอบว่า Tag ทุกตัว Fire ถูกต้อง |
| 7 | **Thumbnail ต้องอ่านง่ายแม้ขนาดเล็ก** | Video Thumbnail บน Youtube แสดงเป็นรูปเล็กๆ ต้องใช้ข้อความสั้น ตัวอักษรใหญ่ สีตัดกับพื้นหลัง ถ้าใส่ข้อความเยอะหรือตัวเล็กจะอ่านไม่ออก Thumbnail ที่ดีเพิ่ม Click-Through Rate ได้ 2-3 เท่า | High | ออกแบบ Thumbnail ด้วยหลัก: ข้อความสั้น + ตัวใหญ่ + สีตัดกัน ทดสอบดูบนมือถือว่าอ่านออกหรือไม่ |
| 8 | **Companion Banner 300x60 เล็กมาก อย่าใส่เยอะ** | Companion Banner ขนาด 300x60 px แสดงข้างวิดีโอบน Desktop เท่านั้น ไม่แสดงบนมือถือ เนื่องจากขนาดเล็กมากจึงควรใส่แค่โลโก้กับข้อความหลัก 1 บรรทัด ใส่เยอะเกินจะอ่านไม่ออกและดูรก | Medium | ออกแบบ Companion Banner 300x60 ใส่แค่โลโก้ + ข้อความสั้น 1 บรรทัด |
| 9 | **Budget ต้องแบ่งตาม Funnel ไม่ใช่เท่ากันหมด** | หลักการคือจ่ายมากที่ Top Funnel (Awareness) เพื่อเข้าถึงคนมากที่สุด แล้วค่อยลดลงตาม Funnel ตัวอย่าง: Awareness 50% Consideration 33% Conversion 17% และต้องเผื่อ A/B Testing 10-20% เพื่อทดสอบว่า Creative ไหนดีกว่า | Critical | วาง Budget Plan ล่วงหน้า แบ่งตาม Funnel Stage เผื่อ A/B Testing 10-20% อย่าใช้งบเท่ากันทุกแคมเปญ |
| 10 | **รวม 2 ตอน = เครื่องมือ 13 รายการต้องครบ** | YTCAMP-004 เตรียมไว้ 6 รายการ (Google Ads, Youtube Link, GTM, GA4, Conversion Tracking, Billing) YTCAMP-005 เตรียมเพิ่ม 7 รายการ (Remarketing, Custom Audiences, Channel Optimize, Landing Page, Pixel Check, Creative Assets, Budget Plan) รวม 13 รายการต้องครบก่อนสร้าง Campaign จริง | Critical | ตรวจ Checklist ทั้ง 13 ข้อ (6 จาก YTCAMP-004 + 7 จาก YTCAMP-005) ให้ครบก่อนไป YTCAMP-006 |

---

## สรุป Priority Actions

| Priority | Action | Timeline |
|----------|--------|----------|
| P1 | สร้าง Remarketing Lists ทั้ง 3 แบบ (Website, Video, Customer) | วันนี้ |
| P2 | ตั้งค่า Custom Intent + Custom Affinity Audiences | วันนี้ |
| P3 | Optimize Youtube Channel (Art, About, Links, Featured Video) + เตรียม Landing Page | วันที่ 2 |
| P4 | ตรวจสอบ Pixel/Tag ด้วย GTM Preview Mode + เตรียม Creative Assets | วันที่ 3 |
| P5 | วาง Budget Plan แบ่งตาม Funnel + เผื่อ A/B Testing | วันที่ 3 |

---

> ทบทวนต่อ: **YTCAMP-006** — วิธีสร้าง Youtube Ads Campaign 1
> Series: SWP3 Ch19 Youtube Ads Campaign
> PinkCastle Academy © 2026
