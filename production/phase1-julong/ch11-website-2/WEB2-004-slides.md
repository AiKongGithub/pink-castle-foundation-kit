# Slides: วิธีการปรับแต่ง Style Layout — WEB2-004
> **Format:** Slide Outline (12 Slides)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 4
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## SLIDE 1: หน้าปก (Title Slide)

- **วิธีการปรับแต่ง Style Layout**
- SWP3 บทที่ 11: สร้างเว็บไซต์ Part 2 — ตอนที่ 4
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- เลือก Page Layout ให้เหมาะกับแต่ละหน้า
- สร้าง Typography System ที่อ่านง่าย
- กำหนด Color Palette ครบ 3 ระดับ
- ออกแบบ Button Styles และ Hover Effect
- สร้าง Design Consistency ทั้งเว็บ

---

## SLIDE 3: Page Layout — เลือกให้เหมาะกับเป้าหมาย

| รูปแบบ | ลักษณะ | เหมาะกับ |
|--------|--------|---------|
| Full-width | เต็มหน้าจอ | Landing Page, Sales Page |
| Boxed | มีขอบสองข้าง | เว็บข้อมูล, Corporate |
| Sidebar Right | มีแถบด้านขวา | บทความบล็อก |
| Sidebar Left | มีแถบด้านซ้าย | เว็บ Documentation |

- **Content Width มาตรฐาน: 1200 พิกเซล**

---

## SLIDE 4: Typography System — ขนาดและระยะห่าง

- **Heading H1-H6** — ลดหลั่นชัดเจน
  - H1: หัวข้อหลัก (ใหญ่ที่สุด)
  - H2: หัวข้อรอง
  - H3-H6: หัวข้อย่อย (ลดลงตามลำดับ)
- **Line-height ที่แนะนำ:**
  - Body text: **1.5 - 1.7**
  - Heading: **1.2 - 1.3**
- เลือกฟอนต์ที่ดูดีด้วยกัน (Serif + Sans-serif)

---

## SLIDE 5: จับคู่ฟอนต์อย่างมืออาชีพ (Font Pairing)

- **หลักการ:** เลือกฟอนต์ที่สไตล์ต่างกัน
  - Heading: **Serif** (มีหาง เช่น Georgia, Playfair Display)
  - Body: **Sans-serif** (ไม่มีหาง เช่น Open Sans, Roboto)
- สร้างความโดดเด่นแต่กลมกลืน
- อย่าใช้ฟอนต์ที่คล้ายกันเกินไป — แยกไม่ออก
- ทดสอบกับเนื้อหาจริง ไม่ใช่แค่ Lorem Ipsum

---

## SLIDE 6: Color Palette — ระบบสี 3 ระดับ

- **Primary Color** — สีหลักของแบรนด์
  - ใช้มากที่สุด: Header, ปุ่มหลัก, ลิงก์
- **Secondary Color** — สีรอง
  - ใช้เสริม: Background, Divider, Icons
- **Accent Color** — สีเน้น
  - ใช้สำหรับ CTA: ปุ่ม "สมัครเลย", "ซื้อเลย"
- ทั้ง 3 สีต้องทำงานร่วมกันอย่างกลมกลืน

---

## SLIDE 7: Button Styles — ปุ่มที่ช่วยขาย

- กำหนด 5 อย่างให้ชัดเจน:
  - **สีปกติ** (Normal State)
  - **สี Hover** (เมาส์ชี้ — เปลี่ยนสี/ขนาด/เงา)
  - **Border** (ขอบปุ่ม)
  - **Size** (ขนาด — Small, Medium, Large)
  - **Border Radius** (มุมปุ่ม — มน หรือ เหลี่ยม)
- สไตล์ต้องสม่ำเสมอทั้งเว็บ

---

## SLIDE 8: Hover Effect — เพิ่ม Conversion

- **Hover Effect คือ** เอฟเฟกต์เมื่อเอาเมาส์ไปวาง
- ตัวอย่าง:
  - เปลี่ยนสีปุ่ม (เข้มขึ้น/อ่อนลง)
  - ขยายขนาดเล็กน้อย (Scale 1.05)
  - เพิ่มเงา (Box Shadow)
- **ทำไมสำคัญ:** บอกผู้ใช้ "อันนี้คลิกได้"
- ช่วยลดความสับสน กระตุ้นการคลิก

---

## SLIDE 9: Spacing Standards — ระยะห่างมาตรฐาน

- **Section Spacing** — ระยะห่างระหว่าง Section ใหญ่
- **Element Spacing** — ระยะห่างระหว่างองค์ประกอบ
- **Padding** — ระยะห่างภายในกล่อง
- **กฎ: สม่ำเสมอทั้งเว็บ**
  - บางจุดห่างมาก + บางจุดชิด = ดูไม่เรียบร้อย
  - กำหนดค่ามาตรฐานแล้วใช้ให้ตรงทุกหน้า

---

## SLIDE 10: Image Styles — สไตล์รูปภาพ

- **Border** — ขอบรูป (มี/ไม่มี ความหนาเท่าไร)
- **Shadow** — เงา (มี/ไม่มี ความเข้มเท่าไร)
- **Aspect Ratio** — อัตราส่วน (16:9, 4:3, 1:1)
- **กฎ: สไตล์เดียวกันทุกรูปทั้งเว็บ**
- รูปคนละสไตล์ = ดูรก ไม่เป็นมืออาชีพ
- เลือก 1 สไตล์ แล้วใช้ให้สม่ำเสมอ

---

## SLIDE 11: Design Consistency — กุญแจสำคัญ

- **ทุกหน้าต้องใช้:**
  - สีเดียวกัน
  - ฟอนต์เดียวกัน
  - สไตล์ปุ่มเดียวกัน
  - ระยะห่างเดียวกัน
  - สไตล์รูปภาพเดียวกัน
- ความไม่สม่ำเสมอ = ลดความน่าเชื่อถือ
- **สร้าง Style Guide** บันทึกทุกค่า ใช้อ้างอิงตลอด

---

## SLIDE 12: สรุปและก้าวต่อไป (Summary & Next Steps)

- Style Layout = การสร้าง Design System ครบวงจร
- 6 ด้าน: Layout, Typography, Colors, Buttons, Spacing, Images
- **Hover Effect** ช่วยเพิ่ม Conversion
- **Design Consistency** คือสิ่งที่แยกมืออาชีพจากมือใหม่
- สร้าง Style Guide แล้วใช้ให้สม่ำเสมอทุกหน้า
- **จบบทเรียน Ch11 สร้างเว็บไซต์ Part 2**

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
