# Executive Summary: วิธีการตั้งค่า UpdraftPlus — WEB2-013
> **Format:** Executive Summary
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 13
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## บทสรุปผู้บริหาร

### ภาพรวม

UpdraftPlus เป็นปลั๊กอิน Backup ยอดนิยมอันดับ 1 ของ WordPress ช่วยสำรองข้อมูลเว็บไซต์ทั้งหมดได้อย่างอัตโนมัติ รองรับการตั้ง Backup Schedule แยกระหว่าง Files กับ Database การเลือก Remote Storage หลายประเภท (Google Drive, Dropbox, Amazon S3) การ Restore กู้คืนด้วยคลิกเดียว และการ Migrate/Clone เว็บไซต์ไปยัง server ใหม่ การสำรองข้อมูลไม่ใช่ทางเลือกแต่เป็นสิ่งจำเป็น เพราะปัญหาเกิดขึ้นได้ตลอดเวลา ไม่ว่าจะเป็นการอัปเดตที่ผิดพลาด การถูกแฮก ความผิดพลาดของมนุษย์ หรือปัญหาจากโฮสติ้ง

### ประเด็นสำคัญ (Key Findings)

**1. Backup คือ "เมื่อไร" ไม่ใช่ "ถ้า"**

ปัญหาเว็บไซต์เกิดขึ้นได้จากหลายสาเหตุ ได้แก่ การอัปเดตปลั๊กอิน/ธีม/WordPress ที่ทำให้เว็บพัง (สาเหตุที่พบบ่อยที่สุด) การถูกแฮก (เว็บ WordPress หลายหมื่นเว็บต่อปี) ความผิดพลาดของมนุษย์ (ลบไฟล์ผิด แก้โค้ดผิด) และปัญหาจากโฮสติ้ง (server ล่ม ฮาร์ดดิสก์เสีย) หากไม่มี Backup จะต้องเริ่มสร้างเว็บใหม่ตั้งแต่ศูนย์

**2. ตั้ง Schedule แยก Database กับ Files**

Database เปลี่ยนแปลงบ่อยกว่า (ทุกครั้งที่มี comment, บทความ, order ใหม่) จึงควร Backup เป็น Daily ส่วน Files (ปลั๊กอิน ธีม รูปภาพ) ไม่ค่อยเปลี่ยน ตั้งเป็น Weekly เพียงพอ ตั้ง Retain 4-7 ชุดเพื่อมี version ย้อนหลังหลายจุด

**3. Remote Storage คือหัวใจของการ Backup**

การเก็บ Backup บน server เดียวกับเว็บไซต์ไม่ปลอดภัย หาก server พัง ทั้งเว็บและ Backup หายไปด้วย UpdraftPlus รองรับ Remote Storage หลายตัว โดย Google Drive แนะนำมากที่สุดเพราะฟรี 15 GB และเชื่อมต่อง่าย

**4. Backup ครอบคลุม 5 ส่วน — Restore ง่ายคลิกเดียว**

UpdraftPlus สำรองข้อมูล 5 ส่วน ได้แก่ Database, Plugins, Themes, Uploads และ Others การ Restore ทำได้จากหน้า Existing Backups เลือกชุดที่ต้องการ เลือกส่วนที่จะ Restore แล้วคลิก ระบบจัดการทั้งหมดให้ พร้อมเก็บ Backup เวอร์ชันก่อน Restore ไว้เป็น safety net

### เปรียบเทียบ Free vs Premium

| เกณฑ์ | Free | Premium |
|-------|------|---------|
| Backup Schedule | ได้ | ได้ |
| Remote Storage | Google Drive, Dropbox ฯลฯ | เพิ่มตัวเลือก |
| Restore | ได้ | ได้ |
| Incremental Backup | ไม่มี | มี (Backup เฉพาะไฟล์ที่เปลี่ยน) |
| Migrator Tool | ต้องทำเอง | อัตโนมัติ |
| เหมาะกับ | เว็บทั่วไป | เว็บใหญ่/ธุรกิจ |

### ข้อเสนอแนะ (Recommendations)

**สำหรับทุกเว็บไซต์:** ติดตั้ง UpdraftPlus ทันที ตั้ง Database Backup เป็น Daily และ Files Backup เป็น Weekly เลือก Google Drive เป็น Remote Storage ตั้ง Retain 4-7 ชุด

**สำหรับเว็บ E-commerce:** พิจารณาใช้ Premium เพราะข้อมูล order/ลูกค้าสำคัญมาก ตั้ง Database Backup บ่อยขึ้น (ทุก 4-12 ชั่วโมง) และใช้ Remote Storage ที่น่าเชื่อถือสูง เช่น Amazon S3

**สำหรับทุกคน:** ทดสอบ Restore อย่างน้อย 3-6 เดือนครั้ง โดยสร้าง staging site แล้วลอง Restore ดู Backup ที่ Restore ไม่ได้ไม่มีค่าอะไรเลย การทดสอบเป็นสิ่งจำเป็นที่ขาดไม่ได้

### หลักการสำคัญ

Backup คือประกันชีวิตของเว็บไซต์ ตั้งค่าให้ครบ (Schedule + Remote Storage + Retention) ทดสอบให้แน่ใจว่า Restore ได้จริง และอย่าเก็บ Backup ไว้ที่เดียวกับเว็บ กฎทองของ Backup คือ 3-2-1: สำรองไว้ 3 ชุด บน 2 สื่อที่ต่างกัน และ 1 ชุดอยู่นอกสถานที่

---

*สิ้นสุดบทสรุปผู้บริหาร — ประมาณ 550 คำ*
