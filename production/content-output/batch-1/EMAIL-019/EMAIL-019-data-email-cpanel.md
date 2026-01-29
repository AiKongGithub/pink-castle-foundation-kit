# Data Table: สร้างอีเมลในระบบ Cpanel

> **Format:** Data Tables & Reference
> **Source:** SWP3 - Email Marketing: สร้างอีเมลในระบบ Cpanel
> **Production ID:** EMAIL-019-DATA

---

## Table 1: Cpanel Access Methods

| Method | URL Format | Port | Security |
|--------|-----------|------|----------|
| Standard | yourdomain.com/cpanel | 2083 | HTTPS |
| Direct Port | yourdomain.com:2083 | 2083 | HTTPS |
| WHM Access | yourdomain.com/whm | 2087 | HTTPS |
| Webmail | yourdomain.com/webmail | 2096 | HTTPS |

---

## Table 2: Email Account Fields

| Field | Description | Example | Required |
|-------|-------------|---------|----------|
| Username | ส่วนหน้า @ | info, contact, sales | Yes |
| Domain | ชื่อโดเมน | yourdomain.com | Yes |
| Password | รหัสผ่าน | Strong12Char$! | Yes |
| Quota | พื้นที่เก็บ | 1000 MB (1 GB) | Yes |
| Send Limit | จำกัดการส่ง/ชม. | 500 emails | Optional |

---

## Table 3: Email Protocols Comparison

| Feature | IMAP | POP3 | Description |
|---------|------|------|-------------|
| Port (SSL) | 993 | 995 | Secure connection |
| Port (No SSL) | 143 | 110 | Not recommended |
| Storage | Server | Local | Where emails stored |
| Sync | All devices | Single | Access across devices |
| Offline | Limited | Full | Read without internet |
| Best For | Most users | Limited storage | Use case |

---

## Table 4: SMTP Settings

| Setting | Value | Notes |
|---------|-------|-------|
| Server | mail.yourdomain.com | หรือ smtp.yourdomain.com |
| Port (SSL) | 465 | Implicit TLS |
| Port (TLS) | 587 | STARTTLS |
| Authentication | Required | Username + Password |
| Username | Full email address | email@yourdomain.com |

---

## Table 5: Webmail Comparison

| Feature | Roundcube | Horde | SquirrelMail |
|---------|-----------|-------|--------------|
| Interface | Modern | Classic | Simple |
| Speed | Fast | Medium | Fastest |
| Calendar | Plugin | Built-in | No |
| Contacts | Advanced | Advanced | Basic |
| Search | Full-text | Full-text | Limited |
| Mobile | Responsive | Partial | No |
| Recommend | Most Users | Power Users | Quick Access |

---

## Table 6: Password Requirements

| Requirement | Minimum | Recommended | Example |
|-------------|---------|-------------|---------|
| Length | 8 chars | 12+ chars | StrongPass123! |
| Lowercase | 1 | 3+ | a, b, c |
| Uppercase | 1 | 2+ | A, B, C |
| Numbers | 1 | 2+ | 0-9 |
| Symbols | 0 | 2+ | !@#$%^& |
| Strength Score | 50 | 80+ | Green bar |

---

## Table 7: Common Email Accounts to Create

| Email | Purpose | Priority |
|-------|---------|----------|
| info@ | General inquiries | High |
| contact@ | Contact form | High |
| sales@ | Sales inquiries | High |
| support@ | Customer support | High |
| admin@ | Administration | Medium |
| noreply@ | Automated emails | Medium |
| newsletter@ | Email marketing | Medium |
| hello@ | Friendly contact | Low |

---

## Table 8: Email Quota Guidelines

| Business Size | Recommended Quota | Notes |
|---------------|-------------------|-------|
| Personal | 500 MB - 1 GB | Basic usage |
| Small Business | 1 - 2 GB | Regular email |
| Medium Business | 2 - 5 GB | Heavy email |
| Enterprise | 5 - 10 GB | With attachments |
| Unlimited | Max available | If hosting allows |

---

## Quick Reference Card

### Access URLs
```
Cpanel: yourdomain.com/cpanel (or :2083)
Webmail: yourdomain.com/webmail (or :2096)
```

### Server Settings
```
IMAP: mail.yourdomain.com:993 (SSL)
POP3: mail.yourdomain.com:995 (SSL)
SMTP: mail.yourdomain.com:465 (SSL)
```

### Create Account Checklist
```
[ ] Username chosen
[ ] Strong password created
[ ] Quota set
[ ] Test email sent
```

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
