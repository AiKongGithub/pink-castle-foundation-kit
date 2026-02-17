# Slides: วิธีการติดตั้ง Plugin ตอนที่ 2 — WEB1-009
> **Format:** Slide Outline (14 Slides)
> **Source:** SWP3 Ch10 สร้างเว็บไซต์ Part 1 ตอนที่ 9
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## SLIDE 1: หน้าปก (Title Slide)
─────────────────

- **วิธีการติดตั้ง Plugin ตอนที่ 2 — Plugin ขั้นสูง**
- SWP3 บทที่ 10: สร้างเว็บไซต์ Part 1 — ตอนที่ 9
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)
─────────────────

- รู้จัก Plugin เร่งความเร็ว (Caching + Image Optimization)
- เข้าใจ Social Sharing และ Email Subscription Plugin
- เปรียบเทียบ Page Builder: Elementor vs Thrive
- รู้จัก WooCommerce สำหรับ E-commerce
- จัดการ Plugin Conflict และเลือก Premium vs Free

---

## SLIDE 3: Performance — Caching Plugin
─────────────────

- **ทำไมความเร็วสำคัญ?**
  - เว็บโหลด > 3 วินาที = สูญเสียผู้เข้าชม 50%+
  - Google ใช้ Page Speed เป็น Ranking Factor

- **Caching Plugin แนะนำ:**
  - WP Super Cache — ง่าย เหมาะมือใหม่
  - W3 Total Cache — ครบวงจร เหมาะผู้มีประสบการณ์

- หลักการ: เก็บสำเนาหน้าเว็บ → ไม่ต้องสร้างใหม่ทุกครั้ง

---

## SLIDE 4: Performance — Image Optimization
─────────────────

- **รูปภาพ = ตัวการหลักที่ทำให้เว็บช้า**
- **Plugin แนะนำ:**
  - ShortPixel — บีบอัด + แปลง WebP
  - Smush — บีบอัดอัตโนมัติ
- **WebP ดีกว่า JPG อย่างไร?**
  - ขนาดเล็กกว่า 25-35%
  - คุณภาพเทียบเท่ากัน
  - Browser สมัยใหม่รองรับทั้งหมด

---

## SLIDE 5: Social Sharing Plugin
─────────────────

- **หน้าที่:** เพิ่มปุ่มแชร์ Social Media บนหน้าเนื้อหา
- **แชร์ไปยัง:** Facebook, LINE, Twitter, Pinterest
- **Plugin แนะนำ:**
  - Social Warfare — ฟีเจอร์ครบ
  - AddToAny — เบา ไม่กระทบ Performance
  - Shareaholic — ปุ่มสวย มี Analytics
- **ข้อควรระวัง:** เลือกตัวที่เบา ไม่โหลด JS หนัก

---

## SLIDE 6: Email Subscription Plugin
─────────────────

- **ทำไมต้องสร้าง Email List?**
  - เป็นทรัพย์สินที่มีค่าที่สุดในธุรกิจออนไลน์
  - สื่อสารตรง ไม่ต้องพึ่งอัลกอริทึม Social Media
  - Social Media เปลี่ยนกฎได้ตลอด แต่ Email List เป็นของเรา

- **Plugin แนะนำ:**
  - MailChimp for WP — มีแผนฟรี เหมาะเริ่มต้น
  - OptinMonster — Popup + Exit Intent ขั้นสูง

---

## SLIDE 7: Exit Intent คืออะไร?
─────────────────

- **Exit Intent** = แสดง Popup เมื่อผู้ใช้กำลังจะปิดหน้าเว็บ
- เป็นโอกาสสุดท้ายในการเปลี่ยนผู้เข้าชมเป็นผู้สมัคร
- **วิธีใช้ให้ได้ผล:**
  - นำเสนอ Lead Magnet (ของฟรีแลกอีเมล)
  - eBook ฟรี / Checklist / ส่วนลดพิเศษ
  - ข้อความสั้น กระชับ มี CTA ชัดเจน

---

## SLIDE 8: Page Builder — Elementor
─────────────────

- **Elementor** — Page Builder ยอดนิยมที่สุด
- ระบบ **ลากวาง** (Drag & Drop)
- เทมเพลตสำเร็จรูปจำนวนมาก
- ใช้ได้กับทุกประเภทเว็บไซต์
- ไม่ต้องเขียนโค้ดเลย
- มีเวอร์ชัน Free และ Pro

---

## SLIDE 9: Page Builder — Thrive Architect
─────────────────

- **Thrive Architect** — Page Builder เน้น Conversion
- ออกแบบมาให้คนกดซื้อ / กดสมัคร / กด CTA
- เหมาะสำหรับ:
  - Landing Page
  - หน้าขายสินค้า
  - Sales Funnel
- **ข้อควรรู้ทั้ง Elementor และ Thrive:**
  - เพิ่ม Code มากลงในเว็บ
  - เปลี่ยน Page Builder ภายหลังยุ่งยากมาก
  - เลือกให้เหมาะตั้งแต่แรก

---

## SLIDE 10: E-commerce — WooCommerce
─────────────────

- **WooCommerce** = Plugin E-commerce อันดับ 1 ของโลก
- เปลี่ยน WordPress เป็นร้านค้าออนไลน์เต็มรูปแบบ
- ฟีเจอร์: ตะกร้าสินค้า / ชำระเงิน / จัดการสินค้า / จัดส่ง
- **ฟรี** แต่อาจต้องซื้อ Extension เพิ่ม
- **ข้อควรรู้:**
  - ทำให้เว็บหนักขึ้นมาก (เพิ่มตาราง DB)
  - ไม่ควรติดตั้งถ้าไม่ได้จะขายของจริงจัง

---

## SLIDE 11: Plugin Conflict — วิธีแก้ปัญหา
─────────────────

- **อาการของ Conflict:**
  - เว็บแสดงผลผิดปกติ
  - หน้าจอขาว (White Screen of Death)
  - ฟีเจอร์บางอย่างไม่ทำงาน

- **วิธีแก้:**
  1. สำรองข้อมูลก่อน
  2. Deactivate Plugin ทีละตัว
  3. ตรวจสอบเว็บหลัง Deactivate แต่ละตัว
  4. เมื่อเว็บกลับปกติ = พบตัวปัญหา
  5. หาทางเลือกอื่นหรือติดต่อผู้พัฒนา

---

## SLIDE 12: การอัปเดต Plugin อย่างปลอดภัย
─────────────────

- **ทำไมต้องอัปเดต?**
  - แก้ช่องโหว่ด้านความปลอดภัย
  - รองรับ WordPress เวอร์ชันใหม่
  - เพิ่มฟีเจอร์ใหม่

- **กฎการอัปเดต:**
  - สำรองข้อมูลก่อนอัปเดต **เสมอ**
  - อัปเดตทีละตัว ไม่ใช่ทั้งหมดพร้อมกัน
  - ตรวจสอบเว็บหลังอัปเดตทุกครั้ง
  - ถ้ามีปัญหา → กู้คืน Backup → รอแก้ไข

---

## SLIDE 13: Premium vs Free Plugin
─────────────────

| เกณฑ์ | Free | Premium |
|-------|------|---------|
| ราคา | ฟรี | มีค่าใช้จ่าย |
| ฟีเจอร์ | พื้นฐาน | ครบครัน ขั้นสูง |
| Support | Community | ทีมเฉพาะ |
| อัปเดต | ไม่แน่นอน | สม่ำเสมอ |

- **เริ่มต้น:** ใช้ฟรีก่อน
- **ควรลงทุน Premium ก่อน:** Security + Backup
- **ค่อยอัปเกรด:** เมื่อธุรกิจเติบโต

---

## SLIDE 14: สรุปและก้าวต่อไป (Summary & Next Steps)
─────────────────

- **Plugin ขั้นสูง 5 ประเภท:**
  1. Performance (Caching + Image Optimization)
  2. Social Sharing (ปุ่มแชร์ Social Media)
  3. Email Subscription (สร้าง Email List)
  4. Page Builder (Elementor / Thrive)
  5. E-commerce (WooCommerce)

- จัดการ Conflict: Deactivate ทีละตัว
- อัปเดตปลอดภัย: สำรองก่อนเสมอ
- **หลักทอง:** ลงเฉพาะที่จำเป็น อย่าลงเพราะอยากลอง

---

*จำนวน Slides ทั้งหมด: 14 สไลด์*
