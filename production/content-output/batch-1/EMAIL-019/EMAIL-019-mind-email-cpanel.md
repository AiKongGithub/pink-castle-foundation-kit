# Mind Map: สร้างอีเมลในระบบ Cpanel

> **Format:** Visual Mind Map (Text-based)
> **Source:** SWP3 - Email Marketing: สร้างอีเมลในระบบ Cpanel
> **Production ID:** EMAIL-019-MIND

---

## Central Theme: Cpanel Email Setup

```
                         ┌─────────────────────────────────┐
                         │      CPANEL EMAIL SETUP         │
                         │      สร้างอีเมลในระบบ           │
                         └──────────────┬──────────────────┘
                                        │
          ┌─────────────────────────────┼─────────────────────────────┐
          │                             │                             │
          ▼                             ▼                             ▼
┌─────────────────┐          ┌─────────────────┐          ┌─────────────────┐
│   เข้าระบบ      │          │   สร้าง Email   │          │   ตั้งค่า       │
│   Cpanel        │          │   Account       │          │   Client        │
└────────┬────────┘          └────────┬────────┘          └────────┬────────┘
         │                            │                            │
    ┌────┴────┐               ┌───────┼───────┐              ┌─────┴─────┐
    │         │               │       │       │              │           │
    ▼         ▼               ▼       ▼       ▼              ▼           ▼
┌───────┐ ┌───────┐    ┌──────┐ ┌──────┐ ┌──────┐    ┌───────────┐ ┌───────────┐
│URL    │ │Port   │    │User  │ │Pass  │ │Quota │    │ Webmail   │ │ Desktop   │
│/cpanel│ │ 2083  │    │name  │ │word  │ │      │    │ IMAP/POP3 │ │ Outlook   │
└───────┘ └───────┘    └──────┘ └──────┘ └──────┘    └───────────┘ └───────────┘
```

---

## Branch Details

### 1. เข้าระบบ Cpanel
- **URL ปกติ:** yourdomain.com/cpanel
- **URL Port:** yourdomain.com:2083
- **Credentials:** จาก Hosting provider
- **Security:** ใช้ HTTPS เสมอ

### 2. สร้าง Email Account
- **Username:** ส่วนหน้า @ เช่น info, contact, support
- **Domain:** เลือก domain ที่ต้องการ
- **Password:** อย่างน้อย 12 ตัวอักษร ผสม a-z, A-Z, 0-9, สัญลักษณ์
- **Quota:** พื้นที่เก็บ email (แนะนำ 1-5GB)

### 3. ตั้งค่า Email Client
- **Webmail:** Roundcube, Horde, SquirrelMail
- **IMAP:** Sync ทุกอุปกรณ์ (Port 993 SSL)
- **POP3:** Download ลงเครื่อง (Port 995 SSL)
- **SMTP:** ส่ง email (Port 465 SSL)

---

## Key Connections

```
Create Account ─────► Configure Client ─────► Ready to Use
      │                      │                      │
      ▼                      ▼                      ▼
  Username            IMAP/SMTP Settings       Send & Receive
  Password            Port Numbers             Professional Email
```

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
