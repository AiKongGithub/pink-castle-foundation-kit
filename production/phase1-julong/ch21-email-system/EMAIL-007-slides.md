# ใส่อีเมลที่ Gateway ใน Sequences — EMAIL-007
> **Format:** Slide Outline (12 Slides)
> **Source:** SWP3 Ch21 ระบบอีเมล ตอนที่ 7
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## SLIDE 1: หน้าปก (Title Slide)

- **ใส่อีเมลที่ Gateway ใน Sequences**
- SWP3 บทที่ 21: ระบบอีเมล — ตอนที่ 7
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- Email Gateway คืออะไร ทำไมต้องตั้งค่า
- SMTP Settings ที่ต้องใส่ในแพลตฟอร์ม
- การยืนยันโดเมน (Domain Verification)
- กระบวนการ Warm-up โดเมนใหม่
- การดูแล Sender Reputation

---

## SLIDE 3: Email Gateway คืออะไร?

- **โครงสร้างพื้นฐาน** ในการส่งอีเมล
- เปรียบเหมือน **"ไปรษณีย์"** ที่พาจดหมายไปถึงผู้รับ
- เชื่อมต่ออีเมลโดเมนตัวเองเข้ากับแพลตฟอร์ม Email Marketing
- ทำให้อีเมลอัตโนมัติส่ง **จากโดเมนของเรา** ไม่ใช่จากแพลตฟอร์ม

---

## SLIDE 4: Gateway เริ่มต้น vs Custom Gateway

| เกณฑ์ | Gateway เริ่มต้น | Custom Gateway |
|-------|:---:|:---:|
| แสดงผลผู้ส่ง | "via thirdparty.com" | yourdomain.com |
| Deliverability | ปานกลาง | สูง |
| Reputation | ใช้ร่วมกับคนอื่น | ของตัวเอง |
| ความเป็นมืออาชีพ | ต่ำ | สูง |

- **สรุป:** Custom Gateway คือสิ่งที่ต้องทำเมื่อใช้งานจริงจัง

---

## SLIDE 5: SMTP Settings — 4 ข้อมูลสำคัญ

- **SMTP Host:** mail.yourdomain.com (ที่อยู่เซิร์ฟเวอร์)
- **SMTP Port:** 465 (SSL) หรือ **587 (TLS)** — แนะนำ
- **Username:** info@yourdomain.com (อีเมลเต็มรูปแบบ)
- **Password:** รหัสผ่านที่ตั้งใน cPanel
- ใส่ข้อมูลเหล่านี้ในส่วน SMTP/Custom Domain ของแพลตฟอร์ม

---

## SLIDE 6: ตำแหน่ง SMTP ในแพลตฟอร์มยอดนิยม

| แพลตฟอร์ม | เส้นทาง |
|-----------|--------|
| Systeme.io | Settings > Emails |
| ActiveCampaign | Settings > Advanced > Custom Mail Server |
| Mailchimp | Settings > Verified Domains |
| GetResponse | Tools > Custom SMTP |

- แต่ละแพลตฟอร์มมีขั้นตอนต่างกันเล็กน้อย
- หลักการเดียวกัน: ใส่ SMTP 4 ข้อมูล

---

## SLIDE 7: Domain Verification — ยืนยันโดเมน

- ยืนยันกับแพลตฟอร์มว่า **เราเป็นเจ้าของโดเมนจริง**
- เพิ่ม **DNS Records** ใน cPanel:
  - SPF Record
  - DKIM Record
  - CNAME Record (เฉพาะแพลตฟอร์ม)
- รอ **DNS Propagation** (24-48 ชั่วโมง แต่มักเร็วกว่า)
- กลับมากด **Verify** ในแพลตฟอร์ม

---

## SLIDE 8: Domain Warm-up — ค่อยๆ สร้างชื่อเสียง

| สัปดาห์ | จำนวน/วัน | หมายเหตุ |
|---------|----------|---------|
| 1 | 20-50 | ส่งหา Active subscribers |
| 2 | 100 | กลุ่มที่ Engage ดี |
| 3 | 200-500 | ขยายไปกลุ่มปกติ |
| 4+ | เพิ่มตามแผน | ดู Reputation ก่อน |

- **กฎทอง:** ห้ามเพิ่มเกิน 2 เท่าจากสัปดาห์ก่อน
- ส่งเยอะทันที = ถูกบล็อก

---

## SLIDE 9: Sender Reputation — ดูแลชื่อเสียงโดเมน

- **Sender Reputation** = ชื่อเสียงโดเมนในสายตา Gmail/Outlook
- ตรวจสอบด้วย **Google Postmaster Tools**
- ปัจจัยสำคัญ:
  - **Bounce Rate** — ต้องต่ำกว่า 2%
  - **Spam Complaints** — ต้องต่ำกว่า 0.1%
  - **Open Rate** — ควรสูงกว่า 20%
- Reputation ดี = อีเมลเข้า Inbox ทุกครั้ง

---

## SLIDE 10: หลีกเลี่ยง Spam Triggers

- **คำเกินจริง:** "ฟรี!!!", "รวยทันที!!!", "ซื้อเดี๋ยวนี้!!!"
- **ตัวพิมพ์ใหญ่ทั้งหมด:** "FREE MONEY NOW"
- **ลิงก์มากเกินไป:** 10+ ลิงก์ในอีเมลเดียว
- **ภาพเยอะ ข้อความน้อย:** ระบบกรองอ่านไม่ได้
- **ไม่มีปุ่ม Unsubscribe:** ผิดกฎหมาย
- **ทางแก้:** เขียนเนื้อหาที่มีคุณค่า ใช้ภาษาธรรมชาติ

---

## SLIDE 11: ขั้นตอนหลังตั้ง Gateway เสร็จ

1. **ส่ง Test Email** จาก Sequence ดูว่าถึง Inbox
2. **เริ่ม Warm-up** — 20-50 ฉบับ/วัน สัปดาห์แรก
3. **สมัคร Google Postmaster Tools** ติดตาม Reputation
4. **ดู Analytics** — Open Rate, Click Rate, Bounce Rate
5. **ค่อยๆ เพิ่ม** ตามตาราง Warm-up

---

## SLIDE 12: สรุปและก้าวต่อไป (Summary & Next Steps)

- Email Gateway = สะพานเชื่อมอีเมลโดเมนกับแพลตฟอร์ม
- ตั้ง SMTP Settings + Verify Domain
- **Warm-up โดเมนใหม่** — ค่อยๆ เพิ่ม ห้ามกระโดด
- ดูแล **Sender Reputation** สม่ำเสมอ
- หลีกเลี่ยง **Spam Triggers** ในเนื้อหา
- **ขั้นตอนถัดไป:** Q&A ตอบคำถามเรื่อง Email Marketing (EMAIL-008)

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
