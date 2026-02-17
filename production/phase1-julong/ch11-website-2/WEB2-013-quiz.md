# Quiz: วิธีการตั้งค่า UpdraftPlus — WEB2-013
> **Format:** Multiple Choice Quiz (10 Questions)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 13
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## คำชี้แจง
- ข้อ 1-6: เลือกคำตอบที่ถูกต้องที่สุดเพียงข้อเดียว (Multiple Choice)
- ข้อ 7-9: ตอบ ถูก (True) หรือ ผิด (False)
- ข้อ 10: เติมคำตอบ (Fill in the blank)

---

### ข้อ 1: เหตุผลหลักที่ทำไมทุกเว็บไซต์ต้องมี Backup คืออะไร?

A) เพราะ Google กำหนดให้เว็บไซต์ต้องมี Backup
B) เพราะปัญหาเกิดขึ้นได้ตลอดเวลา ไม่ว่าจะอัปเดตผิดพลาด ถูกแฮก หรือโฮสติ้งล่ม
C) เพราะ Backup ช่วยให้เว็บไซต์โหลดเร็วขึ้น
D) เพราะ Backup ช่วยป้องกันไม่ให้เว็บถูกแฮก

---

### ข้อ 2: ทำไมต้องตั้ง Backup Schedule แยกระหว่าง Database กับ Files?

A) เพราะ UpdraftPlus ไม่สามารถ Backup ทั้งสองพร้อมกันได้
B) เพราะ Database เปลี่ยนแปลงบ่อยกว่า Files จึงต้อง Backup ถี่กว่า
C) เพราะ Database มีขนาดใหญ่กว่า Files
D) เพราะ Files สำคัญกว่า Database จึงต้อง Backup บ่อยกว่า

---

### ข้อ 3: ควรตั้ง Backup Schedule อย่างไรสำหรับเว็บทั่วไป?

A) Database = Weekly, Files = Monthly
B) Database = Daily, Files = Weekly
C) Database = Monthly, Files = Daily
D) Database = Hourly, Files = Hourly

---

### ข้อ 4: Remote Storage ที่แนะนำมากที่สุดสำหรับ UpdraftPlus คืออะไร?

A) Email เพราะส่งอัตโนมัติ
B) Google Drive เพราะฟรี 15 GB และเชื่อมต่อง่าย
C) USB Drive เพราะเก็บได้มาก
D) เก็บบน server เดียวกับเว็บเพราะสะดวก

---

### ข้อ 5: UpdraftPlus สำรองข้อมูลกี่ส่วน อะไรบ้าง?

A) 3 ส่วน: Database, Plugins, Themes
B) 4 ส่วน: Database, Plugins, Themes, Uploads
C) 5 ส่วน: Database, Plugins, Themes, Uploads, Others
D) 2 ส่วน: Database, Files

---

### ข้อ 6: กฎ 3-2-1 ของ Backup หมายถึงอะไร?

A) Backup 3 ครั้งต่อวัน เก็บ 2 สัปดาห์ ลบ 1 ชุด
B) สำรอง 3 ชุด บน 2 สื่อต่างกัน 1 ชุดนอกสถานที่
C) ใช้ปลั๊กอิน 3 ตัว เก็บใน 2 cloud 1 USB
D) ทดสอบ 3 เดือนครั้ง ใช้ 2 เครื่องมือ เก็บ 1 ปี

---

### ข้อ 7: (True/False) UpdraftPlus จะเก็บเวอร์ชันก่อน Restore ไว้ ถ้า Restore แล้วมีปัญหาสามารถกลับไปเวอร์ชันก่อนหน้าได้

---

### ข้อ 8: (True/False) เก็บ Backup ไว้บน server เดียวกับเว็บไซต์ก็เพียงพอแล้ว ไม่จำเป็นต้องใช้ Remote Storage

---

### ข้อ 9: (True/False) ควรทดสอบการ Restore จาก Backup อย่างน้อย 3-6 เดือนครั้ง เพื่อให้แน่ใจว่า Backup ใช้งานได้จริง

---

### ข้อ 10: (Fill in the blank) UpdraftPlus สำรองข้อมูลได้ 5 ส่วน ได้แก่ Database, Plugins, Themes, ________ และ Others

---

## เฉลย (Answer Key)

| ข้อ | คำตอบ | คำอธิบาย |
|-----|-------|----------|
| 1 | **B** | Backup สำคัญเพราะปัญหาเกิดได้ตลอด ไม่ใช่ข้อกำหนดของ Google และไม่ได้ช่วยเรื่องความเร็วหรือป้องกันแฮก |
| 2 | **B** | Database เปลี่ยนทุกครั้งที่มี comment/order/บทความใหม่ จึงต้อง Backup ถี่กว่า Files ที่ไม่ค่อยเปลี่ยน |
| 3 | **B** | Database = Daily (เปลี่ยนบ่อย) Files = Weekly (ไม่ค่อยเปลี่ยน) เป็นค่าที่แนะนำสำหรับเว็บทั่วไป |
| 4 | **B** | Google Drive ฟรี 15 GB เชื่อมต่อง่าย เพียงพอสำหรับเว็บส่วนใหญ่ อย่าเก็บบน server เดียวกับเว็บ |
| 5 | **C** | 5 ส่วน: Database, Plugins, Themes, Uploads (สื่อ) และ Others (ไฟล์อื่นๆ) ครอบคลุมเว็บทั้งหมด |
| 6 | **B** | 3-2-1 = สำรอง 3 ชุด บน 2 สื่อต่างกัน (เช่น server + cloud) และ 1 ชุดนอกสถานที่ (off-site) |
| 7 | **True** | UpdraftPlus เก็บ Backup ของเดิมไว้ก่อน Restore ถ้ามีปัญหาสามารถกลับไปเวอร์ชันก่อน Restore ได้ |
| 8 | **False** | ถ้า server พัง ทั้งเว็บและ Backup จะหายไปด้วย ต้องใช้ Remote Storage เช่น Google Drive เก็บที่อื่นเสมอ |
| 9 | **True** | Backup ที่ Restore ไม่ได้ไม่มีค่า ต้องทดสอบเป็นประจำโดยสร้าง staging site แล้วลอง Restore |
| 10 | **Uploads** | 5 ส่วน: Database, Plugins, Themes, Uploads (รูปภาพ วิดีโอ PDF) และ Others |

---

**เกณฑ์การประเมิน:**
| คะแนน | ระดับ | คำแนะนำ |
|--------|-------|---------|
| 9-10 | ดีเยี่ยม | พร้อมไปตอนถัดไป |
| 7-8 | ดี | ทบทวนจุดที่พลาดเล็กน้อย |
| 5-6 | พอใช้ | ควรทบทวนเนื้อหาอีกครั้ง |
| ต่ำกว่า 5 | ต้องปรับปรุง | แนะนำให้ดูวิดีโอซ้ำและอ่าน Executive Summary |
