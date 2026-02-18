# Email Marketing ตอนที่ 2 — EMKTG-002 Insights Table
> **Format:** Insights Table (Structured Data Tables)
> **Source:** SWP3 Ch24 Email Marketing Mastery ตอนที่ 2
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 1:18:44

---

## ตาราง 1: ข้อมูลอ้างอิงบทเรียน (Reference Table)

| รายการ | รายละเอียด |
|--------|-----------|
| ชื่อหลักสูตร | Speed Wealth Project รุ่นที่ 3 (SWP3) |
| บทที่ | 24 — Email Marketing Mastery ตอนที่ 2 |
| ความยาว | 1:18:44 (1 ชั่วโมง 18 นาที) |
| ลำดับในหลักสูตร | บทที่ 24 (ตอน 2/4) |
| ประเภท | Intermediate Strategy — Segmentation & Optimization |
| เป้าหมาย | เพิ่มประสิทธิภาพ Email Marketing ด้วย Segmentation, Personalization, A/B Testing |

---

## ตาราง 2: โครงสร้างเนื้อหาตอนที่ 2 (Content Structure)

| ลำดับ | หัวข้อ | เนื้อหาหลัก | ระดับความสำคัญ |
|-------|--------|-------------|---------------|
| 1 | ทบทวนตอนที่ 1 | สรุปพื้นฐาน: List Building, Welcome Sequence, Metrics | ปานกลาง |
| 2 | Segmentation | แบ่ง List ตาม Behavior, Purchase, Engagement, Tags | สูงมาก |
| 3 | Personalization | ชื่อผู้รับ, Dynamic Content, Product Recommendations | สูงมาก |
| 4 | A/B Testing | ทดสอบ Subject Line, Send Time, CTA, Layout | สูงมาก |
| 5 | Deliverability | SPF/DKIM/DMARC, Warm up IP, Clean List, Spam Words | สูงมาก |
| 6 | Re-engagement Campaign | Win-back, Special Offer, Last Chance | สูง |
| 7 | Email Analytics | Open Rate, Click Rate, Conversion, Revenue, Growth | สูง |

---

## ตาราง 3: 4 วิธี Segmentation (Process Table)

| ประเภท | เกณฑ์การแบ่ง | ตัวอย่าง | ข้อมูลที่ต้องเก็บ |
|--------|-------------|---------|-----------------|
| Behavior | พฤติกรรมการเปิด/คลิก | คนที่เปิดอ่านทุกฉบับ vs คนที่ไม่เคยเปิด | Open/Click tracking |
| Purchase History | ประวัติการซื้อ | ลูกค้าที่ซื้อแล้ว vs ยังไม่ซื้อ | Order data |
| Engagement Level | ระดับความ Active | Active (7 วัน) / Semi (30 วัน) / Inactive (90+ วัน) | Last activity date |
| Tags | หัวข้อที่สนใจ | สนใจ Marketing / สนใจ Finance / สนใจ AI | Survey, click behavior |

**ผลลัพธ์**: Open Rate +14%, Click Rate +100% เมื่อเทียบกับส่งแบบหว่าน

---

## ตาราง 4: 4 ระดับ Personalization (Process Table)

| ระดับ | วิธีการ | ความซับซ้อน | ผลกระทบ | เครื่องมือที่ต้องใช้ |
|-------|---------|-----------|---------|-------------------|
| 1 | ชื่อผู้รับใน Subject/เนื้อหา | ง่าย | Open Rate +10% | Merge tags ทุก platform มี |
| 2 | เนื้อหาต่างกันตาม Segment | ปานกลาง | Click Rate +25% | Segment + multiple templates |
| 3 | Dynamic Content ในอีเมลเดียว | ยาก | Conversion +20% | ActiveCampaign, HubSpot |
| 4 | Product Recommendations | ยากมาก | Revenue +30% | AI/ML recommendation engine |

---

## ตาราง 5: A/B Testing Framework (Process Table)

| ตัวแปร | ทดสอบอะไร | วัดผลด้วย | เวลารอผล | ส่งกลุ่มทดสอบ |
|--------|----------|----------|---------|-------------|
| Subject Line | หัวเรื่อง 2 แบบ | Open Rate | 2-4 ชั่วโมง | 10% + 10% |
| Send Time | เวลาส่ง 2 ช่วง | Open Rate | 24 ชั่วโมง | 10% + 10% |
| CTA | ปุ่ม/ข้อความ 2 แบบ | Click Rate | 2-4 ชั่วโมง | 10% + 10% |
| Layout | การจัดวาง 2 แบบ | Click Rate | 2-4 ชั่วโมง | 10% + 10% |

**กฎทอง**: เปลี่ยนทีละ 1 ตัวแปร → ทดสอบ 20% → ส่งตัวชนะให้ 80%

---

## ตาราง 6: Deliverability — 5 ปัจจัยหลัก (Comparison Table)

| ปัจจัย | รายละเอียด | สิ่งที่ต้องทำ | ผลถ้าไม่ทำ |
|--------|-----------|-------------|-----------|
| SPF/DKIM/DMARC | DNS Authentication | ตั้งค่าที่ DNS ของ domain | อีเมลเข้า Spam |
| Warm up IP | ค่อยๆ เพิ่มจำนวนส่ง | 100 → 500 → 1,000 → เป้าหมาย | ถูก flag เป็น spammer |
| Clean List | ลบ bounce/inactive | ทำทุก 3-6 เดือน | Bounce Rate สูง → Reputation ตก |
| Spam Words | คำที่ trigger spam filter | หลีกเลี่ยง "ฟรี!!!" "รวยทันที" | อีเมลถูกบล็อก |
| Sender Reputation | คะแนนความน่าเชื่อถือ | Open Rate > 20%, Complaint < 0.1% | ถูก blacklist |

---

## ตาราง 7: Re-engagement Campaign 3 ขั้นตอน (Process Table)

| ขั้นตอน | อีเมล | เนื้อหา | Timing | เป้าหมาย |
|---------|--------|---------|--------|---------|
| 1 | Win-back | "เราคิดถึงคุณ! ยังสนใจอยู่ไหม?" | หลัง inactive 90 วัน | กระตุ้นให้กลับมา |
| 2 | Special Offer | ส่วนลดพิเศษ/ของฟรี exclusive | 3-5 วันหลังอีเมล 1 | ล่อด้วยสิ่งจูงใจ |
| 3 | Last Chance | "ถ้าไม่ตอบ เราจะลบคุณออก" | 5-7 วันหลังอีเมล 2 | สร้าง urgency |

**หลังจบ 3 ขั้น**: ใครยังเงียบ → ลบออกจาก List → List สะอาด → Deliverability ดีขึ้น

---

## ตาราง 8: Email Analytics — 5 Metrics สำคัญ (Reference Table)

| Metric | ความหมาย | สูตรคำนวณ | เป้าหมาย | ถ้าต่ำกว่าเป้า |
|--------|---------|----------|---------|--------------|
| Open Rate | % คนที่เปิดอ่าน | (เปิดอ่าน / ส่งสำเร็จ) x 100 | > 20% | ปรับ Subject Line |
| Click Rate | % คนที่คลิกลิงก์ | (คลิก / เปิดอ่าน) x 100 | > 2.5% | ปรับ CTA/เนื้อหา |
| Conversion Rate | % คนที่ทำ action | (ซื้อหรือสมัคร / คลิก) x 100 | > 1% | ปรับ landing page |
| Revenue per Email | รายได้ต่อ 1 ฉบับ | รายได้รวม / จำนวนอีเมลส่ง | เพิ่มทุกเดือน | ปรับ offer/segment |
| List Growth Rate | อัตราเติบโต List | ((สมาชิกใหม่ - unsubscribe) / สมาชิกทั้งหมด) x 100 | > 2%/เดือน | เพิ่ม Lead Magnet |

---

## ตาราง 9: เปรียบเทียบก่อน-หลังทำ Segmentation (Comparison Table)

| ตัวชี้วัด | ก่อน (ส่งแบบหว่าน) | หลัง (Segmented) | การเปลี่ยนแปลง |
|----------|-------------------|-----------------|--------------|
| Open Rate | 15-18% | 25-30% | +14% |
| Click Rate | 1.5-2% | 3-5% | +100% |
| Conversion Rate | 0.5-1% | 1.5-3% | +200% |
| Unsubscribe Rate | 0.5-1% | 0.1-0.3% | -70% |
| Spam Complaint | 0.1-0.3% | < 0.05% | -80% |

---

## ตาราง 10: แผนปฏิบัติ 4 สัปดาห์สำหรับ Email Optimization (Process Table)

| สัปดาห์ | กิจกรรม | เป้าหมาย | ตัวชี้วัด |
|---------|---------|---------|---------|
| สัปดาห์ 1 | แบ่ง Segment 3 กลุ่ม + ตรวจ SPF/DKIM/DMARC | จัดระเบียบ List + ยืนยันตัวตน | Segment สร้างเสร็จ 3 กลุ่ม |
| สัปดาห์ 2 | ทำ A/B Testing Subject Line + เริ่ม Personalization ระดับ 2 | ทดสอบและเรียนรู้ | Open Rate ของตัวชนะ > 25% |
| สัปดาห์ 3 | สร้าง Re-engagement Campaign 3 ฉบับ | ดึงคนกลับมา + Clean List | จำนวน Inactive ลดลง 20% |
| สัปดาห์ 4 | วิเคราะห์ Analytics 5 Metrics + วาง baseline | มีข้อมูลเปรียบเทียบ | Dashboard สร้างเสร็จ |

**หลังจาก 4 สัปดาห์**: มี baseline ครบ + List สะอาด + พร้อมเข้าสู่ Automation ในตอนที่ 3

---

> **จำนวนตารางทั้งหมด:** 10 ตาราง
> **ประเภท:** Reference (2), Process (5), Comparison (3)

---

> ทบทวนต่อ: **EMKTG-003** — Email Marketing ตอนที่ 3
> Series: SWP3 Ch24 Email Marketing Mastery
> PinkCastle Academy © 2026
