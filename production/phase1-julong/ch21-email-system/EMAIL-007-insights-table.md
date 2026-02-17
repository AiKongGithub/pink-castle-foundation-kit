# ใส่อีเมลที่ Gateway ใน Sequences — EMAIL-007
> **Format:** Insights Table (Structured Data Tables)
> **Source:** SWP3 Ch21 ระบบอีเมล ตอนที่ 7
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## ตาราง 1: ข้อมูลอ้างอิงบทเรียน (Reference Table)

| รายการ | รายละเอียด |
|--------|-----------|
| ชื่อบทเรียน | ใส่อีเมลที่ Gateway ใน Sequences |
| หลักสูตร | SWP3 Ch21 ระบบอีเมล ตอนที่ 7 |
| ความยาว | 0:07:45 (7 นาที 45 วินาที) |
| ระดับความยาก | กลาง (Intermediate) |
| เครื่องมือที่ใช้ | cPanel, แพลตฟอร์ม Email Marketing, DNS Zone Editor |
| สิ่งที่ต้องเตรียม | อีเมลโดเมน (จาก EMAIL-005) + แพลตฟอร์ม Email Marketing |
| ผลลัพธ์ | ส่งอีเมลอัตโนมัติจากโดเมนตัวเองได้ |

---

## ตาราง 2: SMTP Settings ที่ต้องตั้งค่า (Reference Table)

| รายการ | คำอธิบาย | ตัวอย่าง | หาได้จาก |
|--------|---------|---------|---------|
| SMTP Host | ที่อยู่เซิร์ฟเวอร์ส่งอีเมล | mail.yourdomain.com | ข้อมูลจากโฮสติ้ง |
| SMTP Port (SSL) | พอร์ตเข้ารหัส SSL | 465 | มาตรฐาน |
| SMTP Port (TLS) | พอร์ตเข้ารหัส TLS | 587 | มาตรฐาน (แนะนำ) |
| Username | อีเมลเต็มรูปแบบ | info@yourdomain.com | อีเมลที่สร้างใน cPanel |
| Password | รหัสผ่านอีเมล | (รหัสจาก cPanel) | ตั้งตอนสร้างอีเมล |
| Encryption | ประเภทการเข้ารหัส | SSL หรือ TLS | ขึ้นอยู่กับ Port |

---

## ตาราง 3: เปรียบเทียบ Gateway เริ่มต้น vs Custom Gateway (Comparison Table)

| เกณฑ์ | Gateway เริ่มต้นของแพลตฟอร์ม | Custom Gateway (โดเมนตัวเอง) |
|-------|---------------------------|---------------------------|
| การตั้งค่า | ไม่ต้องตั้งค่า (พร้อมใช้) | ต้องตั้ง SMTP + DNS Records |
| แสดงผลผู้ส่ง | "via thirdparty.com" | yourdomain.com ตรงๆ |
| Deliverability | ปานกลาง (ใช้ IP ร่วม) | สูง (โดเมนผ่าน Authentication) |
| Sender Reputation | ใช้ร่วมกับผู้ใช้คนอื่น | สร้างของตัวเอง ควบคุมได้ |
| ความเป็นมืออาชีพ | ต่ำ | สูง |
| ค่าใช้จ่ายเพิ่ม | ไม่มี | ไม่มี (ใช้ cPanel เดิม) |
| ความซับซ้อน | ง่ายมาก | ปานกลาง |
| แนะนำสำหรับ | ทดสอบเบื้องต้น | ใช้งานจริงจัง |

---

## ตาราง 4: ขั้นตอนตั้งค่า Email Gateway (Process Table)

| ขั้นตอน | สิ่งที่ทำ | รายละเอียด | เวลาโดยประมาณ |
|---------|---------|-----------|-------------|
| 1 | เข้าแพลตฟอร์ม Email Marketing | ไปที่ส่วน SMTP/Custom Domain | 1 นาที |
| 2 | ใส่ SMTP Settings | Host, Port, Username, Password | 3 นาที |
| 3 | ทดสอบการเชื่อมต่อ | กด Test Connection | 1 นาที |
| 4 | เพิ่ม DNS Records | SPF, DKIM, CNAME ใน cPanel | 10 นาที |
| 5 | รอ DNS Propagation | 24-48 ชม. (มักเร็วกว่า) | 1-48 ชม. |
| 6 | กด Verify Domain | ยืนยันในแพลตฟอร์ม | 1 นาที |
| 7 | ส่ง Test Email | ทดสอบส่งจาก Sequence | 5 นาที |
| **รวม** | | | **~20 นาที + รอ DNS** |

---

## ตาราง 5: ตาราง Warm-up โดเมนใหม่ (Process Table)

| สัปดาห์ | จำนวนอีเมล/วัน | จำนวนอีเมล/สัปดาห์ | กิจกรรม |
|---------|---------------|-------------------|--------|
| 1 | 20-50 | 140-350 | ส่งไปหาสมาชิกที่ active ที่สุด |
| 2 | 100 | 700 | ขยายไปกลุ่มที่ engage ดี |
| 3 | 200-500 | 1,400-3,500 | เพิ่มกลุ่มปกติ |
| 4 | 500-1,000 | 3,500-7,000 | ดู Reputation ก่อนเพิ่ม |
| 5 | 1,000-2,000 | 7,000-14,000 | เข้าสู่ปริมาณปกติ |
| 6+ | ตามความต้องการ | - | รักษา Reputation สม่ำเสมอ |

**กฎสำคัญ:** ห้ามเพิ่มเกิน 2 เท่าจากสัปดาห์ก่อน

---

## ตาราง 6: ปัจจัยที่ส่งผลต่อ Sender Reputation (Reference Table)

| ปัจจัย | ค่าที่ดี | ค่าที่แย่ | ผลกระทบ |
|--------|--------|--------|---------|
| Bounce Rate | ต่ำกว่า 2% | สูงกว่า 5% | Bounce สูง = Reputation ตก |
| Spam Complaints | ต่ำกว่า 0.1% | สูงกว่า 0.5% | คนกด Spam = ถูกบล็อก |
| Open Rate | สูงกว่า 20% | ต่ำกว่า 10% | Engagement ต่ำ = ดูเหมือน Spam |
| Click Rate | สูงกว่า 2% | ต่ำกว่า 0.5% | ยืนยันว่าผู้รับสนใจเนื้อหา |
| Unsubscribe Rate | ต่ำกว่า 0.5% | สูงกว่า 2% | คนยกเลิกเยอะ = เนื้อหาไม่ตรงกลุ่ม |

---

## ตาราง 7: Spam Triggers ที่ต้องหลีกเลี่ยง (Reference Table)

| ประเภท | ตัวอย่าง | ทำไมเป็นปัญหา |
|--------|---------|-------------|
| คำเกินจริง | "ฟรี!!!", "รวยทันที!!!", "ซื้อเดี๋ยวนี้!!!" | ระบบกรองมองว่าเป็นโฆษณาหลอก |
| ตัวพิมพ์ใหญ่ทั้งหมด | "FREE MONEY NOW" | ดูเหมือนตะโกน = Spam |
| ลิงก์มากเกินไป | ใส่ลิงก์ 10+ ลิงก์ในอีเมลเดียว | ดูเหมือนฟิชชิ่ง |
| ภาพเยอะ ข้อความน้อย | อีเมลเป็นภาพทั้งหมด | ระบบกรองอ่านข้อความไม่ได้ |
| Sender ไม่ตรง | From แสดง Gmail แต่ส่งจากโดเมนอื่น | ล้มเหลว SPF/DKIM check |
| ไม่มีปุ่ม Unsubscribe | ไม่มีลิงก์ยกเลิกสมาชิก | ผิดกฎหมาย + ถูกกด Spam |

---

## ตาราง 8: ตำแหน่ง SMTP Settings ในแพลตฟอร์มยอดนิยม (Reference Table)

| แพลตฟอร์ม | เส้นทางตั้งค่า | หมายเหตุ |
|-----------|-------------|---------|
| Systeme.io | Settings > Emails | ตั้ง Custom Domain ได้ |
| ActiveCampaign | Settings > Advanced > Custom Mail Server | รองรับ SMTP เต็มรูปแบบ |
| Mailchimp | Settings > Verified Domains | เน้น Domain Verification |
| GetResponse | Tools > Custom SMTP | รองรับ SMTP ของตัวเอง |
| ConvertKit | Settings > Email | Domain Authentication |
| AWeber | Account Settings > Email Server | SMTP Configuration |

---

> **จำนวนตารางทั้งหมด:** 8 ตาราง
> **ประเภท:** Reference (4), Process (2), Comparison (1), Feature-Reference (1)
