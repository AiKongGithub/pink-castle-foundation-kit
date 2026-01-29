# Slide Deck: สร้างอีเมลในระบบ Cpanel

> **Format:** Presentation Slides
> **Source:** SWP3 - Email Marketing: สร้างอีเมลในระบบ Cpanel
> **Total Slides:** 10
> **Production ID:** EMAIL-019-SLIDE

---

## Slide 1: Title Slide

**สร้างอีเมลในระบบ Cpanel**

Professional Email Setup Guide

---

## Slide 2: Why Professional Email?

**ทำไมต้องใช้ Email โดเมนตัวเอง?**

| Free Email | Professional Email |
|------------|-------------------|
| john@gmail.com | john@company.com |
| ดูไม่เป็นมืออาชีพ | น่าเชื่อถือ +40% |
| Platform ควบคุม | คุณควบคุม |

---

## Slide 3: Access Cpanel

**วิธีเข้า Cpanel**

- URL: `yourdomain.com/cpanel`
- หรือ: `yourdomain.com:2083`
- ใช้ HTTPS เพื่อความปลอดภัย
- Login ด้วย credentials จาก hosting

---

## Slide 4: Navigate to Email

**ไปที่ Email Accounts**

1. Login เข้า Cpanel
2. หา Section "EMAIL"
3. คลิก "Email Accounts"
4. พร้อมสร้าง email ใหม่

---

## Slide 5: Create Account

**สร้าง Email Account**

| Field | Example |
|-------|---------|
| Username | info |
| Domain | @yourdomain.com |
| Password | Strong12Char$! |
| Quota | 1 GB |

---

## Slide 6: Password Security

**Password ที่แข็งแรง**

- อย่างน้อย 12 ตัวอักษร
- ผสม a-z, A-Z
- ใส่ตัวเลข 0-9
- มีสัญลักษณ์ !@#$
- อย่าใช้ข้อมูลส่วนตัว

---

## Slide 7: Email Protocols

**IMAP vs POP3**

| | IMAP | POP3 |
|--|------|------|
| Storage | Server | Local |
| Sync | ทุกอุปกรณ์ | เครื่องเดียว |
| Port | 993 SSL | 995 SSL |
| Recommend | ✓ | - |

---

## Slide 8: Server Settings

**ค่า Server สำหรับ Email Client**

```
Incoming (IMAP): mail.yourdomain.com:993
Outgoing (SMTP): mail.yourdomain.com:465
Username: email@yourdomain.com
Password: your-password
```

---

## Slide 9: Webmail Options

**3 Webmail ใน Cpanel**

1. **Roundcube** - Interface สวย (แนะนำ)
2. **Horde** - Features เยอะ
3. **SquirrelMail** - เบา เร็ว

เข้าใช้: `yourdomain.com/webmail`

---

## Slide 10: Next Steps

**สิ่งที่ต้องทำต่อ**

1. ☐ สร้าง Email Account สำเร็จ
2. ☐ ทดสอบส่ง email (ตอนถัดไป)
3. ☐ ตั้งค่า Email Client
4. ☐ ตั้งค่า SPF, DKIM, DMARC

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
