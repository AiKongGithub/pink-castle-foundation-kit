# Slides: วิธีการตั้งค่า UpdraftPlus — WEB2-013
> **Format:** Slide Outline (12 Slides)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 13
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## SLIDE 1: หน้าปก (Title Slide)

- **วิธีการตั้งค่า UpdraftPlus**
- SWP3 บทที่ 11: สร้างเว็บไซต์ Part 2 — ตอนที่ 13
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)

- เข้าใจความสำคัญของการ Backup เว็บไซต์
- ตั้งค่า Backup Schedule แยก Database กับ Files
- เลือก Remote Storage ที่เหมาะสม
- รู้จักสิ่งที่ UpdraftPlus สำรองข้อมูล (5 ส่วน)
- Restore กู้คืนและ Migrate/Clone เว็บไซต์
- ทดสอบ Backup เป็นประจำ

---

## SLIDE 3: ทำไมต้อง Backup?

- **ไม่ใช่ "ถ้า" แต่เป็น "เมื่อไร"** เว็บจะมีปัญหา
- 4 สาเหตุหลักที่เว็บพัง:
  - อัปเดตปลั๊กอิน/ธีม ผิดพลาด
  - ถูกแฮก/มัลแวร์
  - ลบไฟล์ผิด/แก้โค้ดผิด
  - โฮสติ้งล่ม/ฮาร์ดดิสก์เสีย
- **ไม่มี Backup = เริ่มใหม่ตั้งแต่ศูนย์**

---

## SLIDE 4: UpdraftPlus คืออะไร?

- ปลั๊กอิน Backup **อันดับ 1** ของ WordPress
- **ฟีเจอร์หลัก:**
  - ตั้ง Schedule อัตโนมัติ
  - เก็บบน Remote Storage
  - Restore กู้คืนคลิกเดียว
  - Migrate/Clone เว็บไซต์
- มีทั้ง **Free** (เพียงพอสำหรับเว็บทั่วไป) และ **Premium**

---

## SLIDE 5: ตั้งค่า Backup Schedule

| ประเภท | ความถี่ | เหตุผล |
|--------|---------|--------|
| Database | **Daily** (ทุกวัน) | เปลี่ยนบ่อย (comment, order, บทความ) |
| Files | **Weekly** (ทุกสัปดาห์) | ไม่ค่อยเปลี่ยน (ปลั๊กอิน, ธีม) |
| Retain | **4-7 ชุด** | มีหลาย version ย้อนหลัง |

- เว็บ E-commerce: ตั้ง Database เป็นทุก 4-12 ชั่วโมง

---

## SLIDE 6: Remote Storage — อย่าเก็บไว้ที่เดียว!

- **ห้ามเก็บ Backup บน server เดียวกับเว็บ!**
  - server พัง = เว็บ + Backup หายทั้งคู่
- **ตัวเลือก Remote Storage:**

| Storage | ข้อดี | ข้อจำกัด |
|---------|-------|----------|
| Google Drive | ฟรี 15 GB, เชื่อมง่าย | พื้นที่จำกัด |
| Dropbox | ฟรี 2 GB | พื้นที่น้อย |
| Amazon S3 | น่าเชื่อถือสูง | มีค่าใช้จ่าย |
| Email | ส่งอัตโนมัติ | ไฟล์ใหญ่เกิน ไม่แนะนำ |

---

## SLIDE 7: 5 ส่วนที่ Backup

| ส่วน | เนื้อหา | ความสำคัญ |
|------|---------|----------|
| Database | บทความ, หน้า, comment, การตั้งค่า | สูงสุด (หัวใจเว็บ) |
| Plugins | ปลั๊กอินที่ติดตั้งทั้งหมด | สูง |
| Themes | ธีมทั้งหมด | สูง |
| Uploads | รูปภาพ, วิดีโอ, PDF | สูง (กู้คืนยากที่สุด) |
| Others | ไฟล์อื่นๆ | ปานกลาง |

---

## SLIDE 8: Manual Backup — ทำเมื่อไร?

- **ก่อนอัปเดต** WordPress / ปลั๊กอิน / ธีม
- **ก่อนเปลี่ยนธีม** หรือแก้ไขโค้ด
- **ก่อนติดตั้งปลั๊กอินใหม่** ที่ไม่แน่ใจ
- **ก่อนทำ Database Cleanup** ด้วย WP-Rocket
- วิธีทำ: ไปที่ UpdraftPlus > กดปุ่ม **"Backup Now"**

---

## SLIDE 9: Restore กู้คืน — ง่ายคลิกเดียว

- **ขั้นตอน:**
  1. ไปที่แท็บ **Existing Backups**
  2. เลือกชุด Backup ที่ต้องการ
  3. กด **Restore**
  4. เลือกส่วนที่จะ Restore (หรือทั้งหมด)
  5. กด **Restore** อีกครั้ง > เสร็จ!
- **Safety Net:** เก็บเวอร์ชันก่อน Restore ไว้
- ถ้า Restore แล้วมีปัญหา กลับเวอร์ชันก่อนหน้าได้

---

## SLIDE 10: Migrate / Clone เว็บไซต์

- **ใช้กรณี:**
  - ย้ายเว็บไปโฮสติ้งใหม่
  - สร้าง Staging site สำหรับทดสอบ
  - Clone เว็บเป็น template
- **Free:** Backup จากเว็บเก่า > Upload ไป Restore บนเว็บใหม่
- **Premium:** Migrator tool ย้ายอัตโนมัติ

---

## SLIDE 11: ทดสอบ Backup — อย่าลืม!

- **Backup ที่ Restore ไม่ได้ = ไม่มีค่า**
- ทดสอบ **อย่างน้อย 3-6 เดือนครั้ง**
- วิธีทดสอบ:
  1. สร้าง Staging site
  2. ลอง Restore Backup ล่าสุด
  3. ตรวจสอบว่าเว็บทำงานครบถ้วน
- ปัญหาที่อาจพบ:
  - ไฟล์ corrupt
  - Backup ไม่ครบ
  - Remote Storage เต็ม

---

## SLIDE 12: สรุปและก้าวต่อไป (Summary & Next Steps)

- **Backup = ประกันชีวิตเว็บไซต์** ต้องมีทุกเว็บ
- ตั้ง Schedule: Database Daily / Files Weekly / Retain 4-7 ชุด
- Remote Storage: Google Drive (ฟรี 15 GB)
- Backup 5 ส่วน: Database, Plugins, Themes, Uploads, Others
- Restore ง่ายคลิกเดียว + Safety net
- **ทดสอบ Backup เป็นประจำ!**
- **กฎ 3-2-1:** 3 ชุด / 2 สื่อ / 1 นอกสถานที่
- **Action Item:** ติดตั้ง UpdraftPlus + ตั้งค่า + Backup ครั้งแรกวันนี้

---

*จำนวน Slides ทั้งหมด: 12 สไลด์*
