# Insights Table: วิธีการตั้งค่า UpdraftPlus — WEB2-013
> **Format:** Insights Table (10 Rows)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 13
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

| # | Insight (ข้อค้นพบ) | Detail (รายละเอียด) | Application (การนำไปใช้) | Impact Level (ระดับผลกระทบ) |
|---|---|---|---|---|
| 1 | Backup ไม่ใช่ทางเลือก แต่เป็นสิ่งจำเป็น | ปัญหาเว็บไซต์เกิดจากหลายสาเหตุ: อัปเดตผิดพลาด ถูกแฮก ความผิดพลาดมนุษย์ โฮสติ้งล่ม ถ้าไม่มี Backup ต้องเริ่มใหม่จากศูนย์ | ติดตั้ง UpdraftPlus ทันทีหลังสร้างเว็บ WordPress อย่ารอจนมีปัญหาก่อนค่อยทำ Backup | สูง |
| 2 | ตั้ง Schedule แยก Database กับ Files | Database เปลี่ยนบ่อย (comment, order, บทความใหม่) ส่วน Files (ปลั๊กอิน ธีม) ไม่ค่อยเปลี่ยน การ Backup แยกช่วยประหยัดพื้นที่และเวลา | ตั้ง Database Backup = Daily, Files Backup = Weekly เว็บ E-commerce อาจตั้ง Database เป็นทุก 4-12 ชั่วโมง | สูง |
| 3 | Retain หลายชุดป้องกันปัญหาที่ไม่รู้ตัว | บางปัญหาเช่นมัลแวร์อาจแฝงตัวอยู่หลายวัน ถ้ามีแค่ Backup ชุดเดียวอาจเป็นชุดที่ติดมัลแวร์แล้ว | ตั้ง Retain 4-7 ชุด เพื่อมี version ย้อนหลังหลายจุด สามารถเลือกจุดที่สะอาดที่สุดได้ | กลาง |
| 4 | Remote Storage คือหัวใจของ Backup | Backup ที่เก็บบน server เดียวกับเว็บ จะหายไปพร้อมเว็บถ้า server พัง ต้องเก็บที่อื่นเสมอ | เลือก Google Drive เป็น Remote Storage (ฟรี 15 GB เชื่อมต่อง่าย) อย่าใช้ Email เพราะไฟล์ใหญ่เกิน | สูง |
| 5 | Backup ครอบคลุม 5 ส่วนหลักของ WordPress | Database (หัวใจ), Plugins (ปลั๊กอิน), Themes (ธีม), Uploads (สื่อ), Others (อื่นๆ) ทุกส่วนสำคัญต่อการทำงานของเว็บ | Backup ทุกส่วนเสมอ โดยเฉพาะ Database และ Uploads ที่กู้คืนยากที่สุดถ้าหาย | สูง |
| 6 | Restore ง่ายคลิกเดียวพร้อม safety net | UpdraftPlus เก็บเวอร์ชันก่อน Restore ไว้ ถ้า Restore แล้วมีปัญหาก็กลับไปเวอร์ชันก่อนหน้าได้ | ใช้ Restore อย่างมั่นใจ เลือก Restore ได้ทั้งทีเดียวทั้งหมดหรือเฉพาะบางส่วน เช่น เฉพาะ Database | กลาง |
| 7 | Migrate/Clone เว็บไซต์ได้ง่าย | ใช้ Backup จาก UpdraftPlus ย้ายเว็บไปโฮสติ้งใหม่หรือสร้างเว็บทดสอบ (Staging) ได้ เวอร์ชัน Premium มี Migrator tool อัตโนมัติ | ใช้ UpdraftPlus เมื่อต้องย้ายโฮสติ้ง แทนการใช้เครื่องมือ migrate แยก หรือใช้สร้าง staging site สำหรับทดสอบ | กลาง |
| 8 | ทดสอบ Backup เป็นประจำเป็นสิ่งจำเป็น | Backup ที่ Restore ไม่ได้ = ไม่มีค่า ปัญหาที่พบบ่อย: ไฟล์ corrupt, Backup ไม่ครบ, Remote Storage เต็ม | ทดสอบ Restore อย่างน้อย 3-6 เดือนครั้ง สร้าง staging site แล้วลอง Restore ตรวจสอบว่าเว็บทำงานครบ | สูง |
| 9 | เวอร์ชันฟรีเพียงพอสำหรับเว็บทั่วไป | Free มี Schedule, Remote Storage, Restore ครบ Premium เพิ่ม Incremental Backup, Migrator และ Storage เพิ่ม | เว็บทั่วไปใช้ Free เว็บ E-commerce หรือเว็บใหญ่พิจารณา Premium เพื่อ Incremental Backup ที่ประหยัดพื้นที่ | กลาง |
| 10 | กฎ 3-2-1 คือมาตรฐานทองของ Backup | สำรอง 3 ชุด บน 2 สื่อต่างกัน และ 1 ชุดนอกสถานที่ ป้องกันการสูญเสียข้อมูลทุกกรณี รวมถึงภัยธรรมชาติ | ใช้ UpdraftPlus Backup ไป Google Drive (off-site) + เก็บบน server (on-site) ก็ครบตามกฎ 3-2-1 แล้ว | สูง |

---

## สรุปตาม Impact Level

| ระดับ | จำนวน Insights | หัวข้อหลัก |
|-------|:---:|---|
| สูง | 6 | Backup จำเป็น, Schedule แยก, Remote Storage, 5 ส่วน Backup, ทดสอบ Restore, กฎ 3-2-1 |
| กลาง | 4 | Retain หลายชุด, Restore safety net, Migrate/Clone, Free vs Premium |
| ต่ำ | 0 | — |

---

*จำนวน Insights ทั้งหมด: 10 รายการ*
