# วิธีปรับแต่ง Email Header — EMAIL-002
> **Format:** Mind Map (Text-based)
> **Source:** SWP3 Ch21 ระบบอีเมล ตอนที่ 2
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

```
                   ปรับแต่ง Email Header
                   (Email Header Design)
                            |
        ┌───────────────────┼───────────────────┐
        |                   |                   |
   [Header Design]    [การตั้งค่าผู้ส่ง]    [Footer & Format]
        |                   |                   |
   ┌────┼────┐         ┌───┼───┐          ┌────┼────┐
```

## Center Node: ปรับแต่ง Email Header (Email Header Design)

### Branch 1: Header Design (การออกแบบส่วนหัว)
- โลโก้ (Logo)
  - ตำแหน่ง: ตรงกลางหรือมุมซ้ายบน
  - ขนาดเหมาะสม ไม่ใหญ่เกินไป
  - คมชัด ดูดีทั้ง Desktop และ Mobile
- สีแบรนด์ (Brand Colors)
  - ใช้เป็นพื้นหลังหรือเส้นคั่น
  - ตรงกับสีบนเว็บไซต์
  - สม่ำเสมอทุกอีเมล
- ลิงก์นำทาง (Navigation Links)
  - ลิงก์ไปเว็บไซต์หลัก
  - ลิงก์ไปบล็อก
  - ลิงก์ Social Media
  - ไม่เกิน 3-4 ลิงก์
- Pre-header Text
  - ข้อความ 40-100 ตัวอักษร
  - เสริม Subject Line ไม่ใช่ซ้ำ
  - สร้างความอยากรู้

### Branch 2: การตั้งค่าผู้ส่ง (Sender Settings)
- From Name
  - ใช้ชื่อจริง + ชื่อแบรนด์
  - ตัวอย่าง: "สมชาย จาก PinkCastle"
  - ห้ามใช้ "noreply"
- From Email
  - อีเมลมืออาชีพ (ไม่ใช่ Gmail)
  - ตัวอย่าง: newsletter@pinkcastle.com
  - ใช้โดเมนของแบรนด์
- Reply-to Address
  - อาจเหมือนหรือต่างจาก From Email
  - ส่งไปทีมที่เหมาะสม
  - ตัวอย่าง: support@pinkcastle.com

### Branch 3: Footer (ส่วนท้าย)
- ข้อกำหนดทางกฎหมาย
  - Unsubscribe Link (บังคับ)
  - ที่อยู่ทางกายภาพ (บังคับ)
  - Privacy Policy Link (แนะนำ)
- CAN-SPAM Act
  - ต้องมีลิงก์ยกเลิกสมาชิก
  - ต้องดำเนินการภายใน 10 วัน
  - ฝ่าฝืนมีค่าปรับ
- องค์ประกอบเสริม
  - ลิงก์ Social Media
  - ข้อความลิขสิทธิ์
  - ข้อมูลติดต่อเพิ่มเติม

### Branch 4: HTML vs Plain Text
- HTML Email
  - มีสี รูปภาพ ปุ่ม CTA
  - ดูเป็นมืออาชีพ
  - เหมาะกับ Newsletter / โปรโมชัน
  - อาจเข้า Promotion tab
- Plain Text Email
  - ข้อความล้วน
  - ดูจริงใจ เหมือนเขียนถึงเอง
  - เหมาะกับ Follow-up ส่วนตัว
  - มักเข้า Primary inbox

### Branch 5: Mobile Responsive
- ความสำคัญ
  - คน 60%+ เปิดอีเมลบนมือถือ
  - แสดงผลไม่ดี = ลบทิ้งทันที
- สิ่งที่ต้องทำ
  - Header ปรับขนาดอัตโนมัติ
  - ปุ่ม CTA ใหญ่พอกดด้วยนิ้ว
  - ตัวอักษร 14px ขึ้นไป
  - คอลัมน์เดียวบนมือถือ
- การทดสอบ
  - ส่งอีเมลทดสอบให้ตัวเอง
  - เปิดดูทั้ง Desktop และ Mobile
  - ทดสอบหลาย email client

### Branch 6: Brand Consistency (ความสม่ำเสมอ)
- หลักการ
  - ใช้โลโก้เดียวกันทุกอีเมล
  - สีแบรนด์เดียวกัน
  - ฟอนต์สไตล์เดียวกัน
  - น้ำเสียงสื่อสารเดียวกัน
- ผลลัพธ์
  - คนจำแบรนด์ได้ทันที
  - สร้างความไว้วางใจ
  - ไม่ถูกมองว่าเป็นสแปม
- วิธีทำ
  - สร้าง Email Template มาตรฐาน
  - สร้าง Brand Guidelines สำหรับอีเมล
  - ใช้ Template เดียวกันทุกฉบับ

---

**จำนวน Nodes ทั้งหมด: 48 nodes**

| ระดับ | จำนวน |
|-------|-------|
| Center Node | 1 |
| Branch (ระดับ 1) | 6 |
| Sub-branch (ระดับ 2) | 20 |
| Leaf (ระดับ 3) | 21 |
| **รวม** | **48** |
