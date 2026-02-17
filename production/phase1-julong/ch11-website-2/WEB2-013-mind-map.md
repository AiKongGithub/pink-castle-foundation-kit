# Mind Map: วิธีการตั้งค่า UpdraftPlus — WEB2-013
> **Format:** Mind Map (Text-based)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 13
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

```mermaid
mindmap
  root((UpdraftPlus Backup))
    ทำไมต้อง Backup
      อัปเดตผิดพลาดเว็บพัง
      ถูกแฮก มัลแวร์
      ความผิดพลาดมนุษย์ ลบไฟล์ผิด
      โฮสติ้งล่ม server เสีย
      ไม่ใช่ ถ้า แต่เป็น เมื่อไร
    Backup Schedule
      Database Backup
        Daily ทุกวัน
        เปลี่ยนบ่อย comment/order/บทความ
      Files Backup
        Weekly ทุกสัปดาห์
        ปลั๊กอิน ธีม ไม่ค่อยเปลี่ยน
      Retain
        เก็บ 4-7 ชุดย้อนหลัง
        มีหลายจุดให้กู้คืน
    Remote Storage
      Google Drive
        ฟรี 15 GB
        เชื่อมต่อง่าย แนะนำมากสุด
      Dropbox
      Amazon S3
        เหมาะเว็บใหญ่
      Email
        ไม่แนะนำ ไฟล์ใหญ่เกิน
    สิ่งที่ Backup
      Database หัวใจของเว็บ
      Plugins ปลั๊กอินทั้งหมด
      Themes ธีมทั้งหมด
      Uploads รูปภาพ วิดีโอ PDF
      Others ไฟล์อื่นๆ
    Restore กู้คืน
      เลือกชุด Backup
      เลือกส่วนที่จะ Restore
      คลิกเดียว ระบบจัดการให้
      เก็บเวอร์ชันก่อน Restore ไว้
    Migrate Clone
      ย้ายโฮสติ้งใหม่
      สร้าง staging site
      Free ทำด้วยตนเอง
      Premium มี Migrator tool
    ทดสอบ Backup
      ทดสอบ 3-6 เดือนครั้ง
      สร้าง staging แล้วลอง Restore
      Backup ที่ Restore ไม่ได้ไม่มีค่า
    กฎ 3-2-1
      สำรอง 3 ชุด
      บน 2 สื่อต่างกัน
      1 ชุดนอกสถานที่
```

---

## Center Node: UpdraftPlus Backup

### Branch 1: ทำไมต้อง Backup
- อัปเดตผิดพลาด — ปลั๊กอิน/ธีม/WordPress ทำเว็บพัง
- ถูกแฮก — เว็บ WordPress หลายหมื่นเว็บต่อปี
- ความผิดพลาดมนุษย์ — ลบไฟล์ผิด แก้โค้ดผิด
- ปัญหาโฮสติ้ง — server ล่ม ฮาร์ดดิสก์เสีย

### Branch 2: Backup Schedule
- Database Backup = Daily (เปลี่ยนบ่อย)
- Files Backup = Weekly (ไม่ค่อยเปลี่ยน)
- Retain 4-7 ชุดย้อนหลัง

### Branch 3: Remote Storage
- Google Drive (แนะนำ ฟรี 15 GB)
- Dropbox, Amazon S3
- อย่าใช้ Email (ไฟล์ใหญ่เกิน)
- อย่าเก็บบน server เดียวกับเว็บ

### Branch 4: สิ่งที่ Backup (5 ส่วน)
- Database, Plugins, Themes, Uploads, Others

### Branch 5: Restore กู้คืน
- เลือกชุด Backup > เลือกส่วน > คลิก Restore
- เก็บเวอร์ชันก่อน Restore ไว้เป็น safety net

### Branch 6: Migrate/Clone
- ย้ายโฮสติ้ง / สร้าง staging site
- Free ทำด้วยตนเอง / Premium มี Migrator tool

### Branch 7: ทดสอบ Backup
- ทดสอบ 3-6 เดือนครั้ง
- Backup ที่ Restore ไม่ได้ = ไม่มีค่า

### Branch 8: กฎ 3-2-1
- 3 ชุด / 2 สื่อต่างกัน / 1 ชุดนอกสถานที่

---

**จำนวน Nodes ทั้งหมด: 42 nodes**

| ระดับ | จำนวน |
|-------|-------|
| Center Node | 1 |
| Branch (ระดับ 1) | 8 |
| Sub-branch (ระดับ 2) | 21 |
| Leaf (ระดับ 3) | 12 |
| **รวม** | **42** |
