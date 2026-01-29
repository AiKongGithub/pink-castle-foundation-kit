# Video Summary: ทดลองส่งอีเมลจากระบบ Cpanel

> **Format:** Video Summary Script
> **Source:** SWP3 - Email Marketing: ทดลองส่งอีเมลจากระบบ Cpanel
> **Duration:** ~5-7 minutes
> **Production ID:** EMAIL-020-VIDEO

---

## Video Script

### [INTRO - 0:00-0:30]

**On Screen:** ทดลองส่งอีเมลจากระบบ Cpanel

**Narrator:** หลังจากสร้าง Email Account แล้ว ขั้นตอนสำคัญคือการทดสอบ วันนี้เราจะมาดูวิธีทดสอบ Email และแก้ปัญหาที่พบบ่อย

---

### [SECTION 1 - 0:30-2:00] Login Webmail

**Steps:**
- ไปที่ yourdomain.com/webmail
- Login ด้วย email และ password
- เลือก Roundcube

**Visual:** Screen recording การ login webmail

---

### [SECTION 2 - 2:00-3:30] ทดสอบส่ง Email

| Test | From | To | Check |
|------|------|----|----- |
| 1 | Cpanel Email | Gmail | Inbox ไม่ใช่ Spam |
| 2 | Cpanel Email | Yahoo | Inbox ไม่ใช่ Spam |
| 3 | Gmail | Cpanel Email | รับได้ถูกต้อง |

**Visual:** แสดงการส่ง email และเช็คว่าถึง

---

### [SECTION 3 - 3:30-5:00] เช็ค Email Headers

**How to check:**
1. เปิด email ที่ได้รับ
2. คลิก "Show Original" (Gmail)
3. ดู SPF, DKIM, DMARC results
4. ต้องเป็น PASS ทั้งหมด

**Visual:** แสดง email header และ authentication results

---

### [SECTION 4 - 5:00-6:00] Troubleshooting

**Common Issues:**
- Email เข้า Spam → ตั้งค่า SPF, DKIM
- ส่งไม่ได้ → เช็ค SMTP Port 465/587
- รับไม่ได้ → เช็ค IMAP Port 993
- Error timeout → เปิด SSL/TLS

---

### [OUTRO - 6:00-6:30]

**Call to Action:**
- ลองทดสอบ email ของตัวเอง
- ถ้าเข้า Spam ให้ดูตอน SPF/DKIM setup
- Subscribe เพื่อดูตอนต่อไป

---

## Production Notes

- Screen recording ตลอดการทดสอบ
- Highlight ส่วน Pass/Fail ใน headers
- ใส่ timestamps สำหรับ troubleshooting

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
