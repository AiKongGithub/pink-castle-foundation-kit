# Slides: แนะนำ cPanel และติดตั้ง WordPress — WEB1-006
> **Format:** Slide Outline (14 Slides)
> **Source:** SWP3 Ch10 สร้างเว็บไซต์ Part 1 ตอนที่ 6
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## SLIDE 1: หน้าปก (Title Slide)
─────────────────

- **แนะนำ cPanel และติดตั้ง WordPress**
- SWP3 บทที่ 10: วิธีการสร้างเว็บไซต์ Part 1 — ตอนที่ 6
- PinkCastle Academy
- วันที่: 17 กุมภาพันธ์ 2569

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)
─────────────────

- เข้าใจว่า cPanel คืออะไรและใช้งานอย่างไร
- รู้จักหมวดหมู่หลักใน cPanel
- ติดตั้ง WordPress ด้วย Softaculous ได้
- ตั้งค่าเริ่มต้นที่สำคัญของ WordPress ได้
- เข้าสู่ WordPress Admin Dashboard และใช้งานเมนูหลักได้

---

## SLIDE 3: cPanel คืออะไร? (What is cPanel?)
─────────────────

- แผงควบคุมเว็บโฮสติ้งแบบกราฟิก (GUI) ที่นิยมที่สุดในโลก
- เปรียบเสมือน **ห้องควบคุมของบ้าน** — จัดการทุกอย่างจากที่เดียว
- **ไม่ต้องพิมพ์คำสั่ง** — ทุกอย่างเป็นไอคอนให้คลิก
- เข้าผ่าน: **yourdomain.com:2083** หรือลิงก์จากอีเมลโฮสติ้ง
- ล็อกอินด้วย username/password ที่ได้มาตอนซื้อโฮสติ้ง

---

## SLIDE 4: หมวดหมู่หลักใน cPanel (Main Categories)
─────────────────

| หมวด | ฟีเจอร์ | ใช้สำหรับ |
|------|---------|----------|
| **Files** | File Manager | อัปโหลด/จัดการไฟล์ |
| **Databases** | MySQL | ฐานข้อมูลสำหรับ WordPress |
| **Domains** | Subdomains, DNS | จัดการโดเมน |
| **Email** | Email Accounts | สร้างอีเมลธุรกิจ (info@domain.com) |
| **Security** | SSL/TLS | ใบรับรองความปลอดภัย |
| **Software** | Softaculous | ติดตั้ง WordPress! |

---

## SLIDE 5: Softaculous — เครื่องมือติดตั้ง WordPress (Auto Installer)
─────────────────

- เครื่องมือติดตั้งแอปพลิเคชันอัตโนมัติใน cPanel
- รองรับ WordPress และแอปอื่นๆ กว่า 400 รายการ
- ติดตั้ง **แบบ one-click** — ไม่ต้องเขียนโค้ด
- สร้างฐานข้อมูลให้อัตโนมัติ
- หาได้ที่: หมวด Software > Softaculous Apps Installer

---

## SLIDE 6: ขั้นตอนที่ 1 — เปิด Softaculous (Step 1)
─────────────────

- ล็อกอินเข้า cPanel
- มองหาไอคอน **Softaculous Apps Installer** หรือ **WordPress**
- อยู่ในหมวด **Software**
- คลิกเข้าไป จะเห็น WordPress พร้อมปุ่ม **Install**
- กดปุ่ม **Install** เพื่อเริ่มขั้นตอนการกรอกข้อมูล

---

## SLIDE 7: ขั้นตอนที่ 2 — กรอกข้อมูลการติดตั้ง (Installation Settings)
─────────────────

- **Protocol:** เลือก **https://** (ต้องมี SSL)
- **Domain:** เลือกโดเมนที่ต้องการติดตั้ง
- **In Directory:** **ลบให้เป็นช่องว่าง** = WordPress เป็นหน้าหลัก
  - พิมพ์ "blog" = ติดตั้งที่ yourdomain.com/blog
- **Table Prefix:** เปลี่ยนจาก wp_ เป็นค่าอื่น เช่น **pc_** (ความปลอดภัย)

---

## SLIDE 8: ขั้นตอนที่ 3 — Site Settings & Admin Account
─────────────────

**Site Settings:**
- Site Name = ชื่อเว็บไซต์ (เปลี่ยนได้ทีหลัง)
- Site Description = คำอธิบายสั้นๆ

**Admin Account (สำคัญมาก!):**
- Username: **ห้ามใช้ "admin"** — ใช้ชื่ออื่นที่เดาได้ยาก
- Password: **แข็งแรง** — ตัวเล็ก ตัวใหญ่ ตัวเลข สัญลักษณ์
- Email: ใส่อีเมลที่ใช้งานจริง

**ภาษา:** เลือก **Thai** สำหรับคนไทย

---

## SLIDE 9: ขั้นตอนที่ 4 — กด Install และรอ (Install & Wait)
─────────────────

- กดปุ่ม **Install** ที่ด้านล่างของฟอร์ม
- รอประมาณ **1-2 นาที** ระบบทำงานอัตโนมัติ
- เมื่อเสร็จจะได้ **2 ลิงก์สำคัญ:**
  - **หน้าเว็บ:** yourdomain.com (สิ่งที่ผู้เข้าชมเห็น)
  - **Admin Dashboard:** yourdomain.com/wp-admin (แผงควบคุม)
- **บันทึก username/password ไว้ในที่ปลอดภัย!**

---

## SLIDE 10: WordPress Admin Dashboard — ศูนย์บัญชาการ
─────────────────

- ล็อกอินที่ **yourdomain.com/wp-admin**
- เมนูด้านซ้าย = เครื่องมือทั้งหมด

| เมนู | หน้าที่ |
|------|---------|
| **Posts** | เขียนบทความ/ข่าว |
| **Pages** | สร้างหน้าเว็บ (เกี่ยวกับเรา, ติดต่อ) |
| **Appearance** | เปลี่ยนธีม/ดีไซน์ |
| **Plugins** | เพิ่มฟีเจอร์ (SEO, Security, Forms) |
| **Media** | จัดการรูปภาพ/วิดีโอ |
| **Settings** | ตั้งค่าทั่วไป |

---

## SLIDE 11: ตั้งค่าสำคัญทันทีหลังติดตั้ง (Essential Settings)
─────────────────

**1. Permalink Structure (สำคัญที่สุด!)**
- ไปที่ Settings > Permalinks
- เลือก **Post Name**
- URL: yourdomain.com/**how-to-start-business** (อ่านง่าย ดี SEO)
- แทนที่: yourdomain.com/?p=123 (อ่านไม่รู้เรื่อง)

**2. ภาษา**
- Settings > General > Site Language = Thai

**3. ตั้งเวลา**
- Settings > General > Timezone = Bangkok (UTC+7)

---

## SLIDE 12: เคล็ดลับความปลอดภัย (Security Tips)
─────────────────

- **Admin Username** — ห้ามใช้ "admin" ใช้ชื่อที่เดาได้ยาก
- **Password** — ตัวเล็ก+ใหญ่+เลข+สัญลักษณ์ อย่างน้อย 12 ตัว
- **Table Prefix** — เปลี่ยนจาก wp_ เป็นค่าอื่น
- **อัปเดตสม่ำเสมอ** — WordPress, Themes, Plugins ให้ up-to-date
- **Plugin ความปลอดภัย** — ติดตั้ง Wordfence หรือ Sucuri เป็นอันดับแรก

---

## SLIDE 13: สรุปขั้นตอนทั้งหมด (Complete Process)
─────────────────

```
1. ล็อกอินเข้า cPanel (domain:2083)
   ↓
2. เปิด Softaculous (หมวด Software)
   ↓
3. กรอกข้อมูล (URL, ชื่อเว็บ, Admin)
   ↓
4. กด Install (รอ 1-2 นาที)
   ↓
5. ล็อกอิน wp-admin
   ↓
6. ตั้งค่า Permalink = Post Name
   ↓
7. เว็บไซต์พร้อมใช้งาน!
```

**เวลารวม: 8-10 นาที | ไม่ต้องเขียนโค้ด**

---

## SLIDE 14: สรุปและก้าวต่อไป (Summary & Next Steps)
─────────────────

- **cPanel** = แผงควบคุมโฮสติ้ง ใช้งานง่ายเหมือนสมาร์ทโฟน
- **Softaculous** = ติดตั้ง WordPress แบบ one-click ใน 10 นาที
- **ตั้งค่าสำคัญ:** Permalink Post Name, Admin ไม่ใช่ "admin", เปลี่ยน Table Prefix
- ตอนนี้คุณมีครบ: **โดเมน + โฮสติ้ง + WordPress**
- **ก้าวต่อไป:** เลือกธีม ออกแบบหน้าตา และเริ่มสร้างเนื้อหา!

---

*จำนวน Slides ทั้งหมด: 14 สไลด์*
