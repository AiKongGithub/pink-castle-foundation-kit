# Slide Deck: ทดลองส่งอีเมลจากระบบ Cpanel

> **Format:** Presentation Slides
> **Source:** SWP3 - Email Marketing: ทดลองส่งอีเมลจากระบบ Cpanel
> **Total Slides:** 10
> **Production ID:** EMAIL-020-SLIDE

---

## Slide 1: Title Slide

**ทดลองส่งอีเมลจากระบบ Cpanel**

Testing & Troubleshooting Guide

---

## Slide 2: Why Test?

**ทำไมต้องทดสอบ?**

- 20% ของ Email ใหม่มีปัญหา
- Email อาจเข้า Spam โดยไม่รู้ตัว
- Configuration อาจผิดพลาด
- ป้องกันปัญหาก่อนใช้งานจริง

---

## Slide 3: Access Webmail

**เข้า Webmail**

1. ไปที่ `yourdomain.com/webmail`
2. Login ด้วย Email + Password
3. เลือก Roundcube
4. พร้อมทดสอบ

---

## Slide 4: Testing Matrix

**ทดสอบ 6 ขั้นตอน**

| # | Test | Expected Result |
|---|------|-----------------|
| 1 | ส่งไป Gmail | เข้า Inbox |
| 2 | ส่งไป Yahoo | เข้า Inbox |
| 3 | ส่งไป Hotmail | เข้า Inbox |
| 4 | รับจาก Gmail | ได้รับถูกต้อง |
| 5 | Reply Test | Reply สำเร็จ |
| 6 | Attachment | รับไฟล์ได้ |

---

## Slide 5: Email Authentication

**3 ปัจจัยสำคัญ**

| Record | Purpose | Check |
|--------|---------|-------|
| SPF | Verify sender | Pass |
| DKIM | Digital signature | Pass |
| DMARC | Policy control | Pass |

**All must be PASS!**

---

## Slide 6: Check Headers

**วิธีดู Authentication Result**

1. เปิด email ที่ได้รับใน Gmail
2. คลิก 3 dots menu
3. เลือก "Show original"
4. หา "Authentication-Results"
5. ดูว่า SPF, DKIM, DMARC = Pass

---

## Slide 7: Common Issues

**ปัญหาที่พบบ่อย**

| Problem | Cause | Solution |
|---------|-------|----------|
| เข้า Spam | ไม่มี SPF/DKIM | ตั้งค่า Records |
| ส่งไม่ได้ | SMTP Error | Port 465/587 |
| รับไม่ได้ | IMAP Error | Port 993 |

---

## Slide 8: Mail-Tester

**ใช้ mail-tester.com**

1. ไปที่ mail-tester.com
2. Copy email address ที่แสดง
3. ส่ง test email ไป
4. กลับมาดูคะแนน

**Target Score: 10/10**

---

## Slide 9: Troubleshooting Flow

**ขั้นตอนแก้ปัญหา**

```
ส่งไม่ได้? → เช็ค SMTP Settings
    ↓
รับไม่ได้? → เช็ค IMAP Settings
    ↓
เข้า Spam? → ตั้งค่า SPF/DKIM
    ↓
ยังไม่หาย? → ติดต่อ Hosting
```

---

## Slide 10: Checklist Complete

**Checklist สำเร็จ**

- ☐ ส่งไป 3 providers แล้ว
- ☐ รับ email ได้แล้ว
- ☐ Reply test ผ่าน
- ☐ SPF/DKIM/DMARC Pass
- ☐ Mail-tester score 8+

**Ready to use!**

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
