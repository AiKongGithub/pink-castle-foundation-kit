# Mind Map: ทดลองส่งอีเมลจากระบบ Cpanel

> **Format:** Visual Mind Map (Text-based)
> **Source:** SWP3 - Email Marketing: ทดลองส่งอีเมลจากระบบ Cpanel
> **Production ID:** EMAIL-020-MIND

---

## Central Theme: Email Testing & Troubleshooting

```
                         ┌─────────────────────────────────┐
                         │      EMAIL TESTING              │
                         │      ทดลองส่งอีเมล              │
                         └──────────────┬──────────────────┘
                                        │
          ┌─────────────────────────────┼─────────────────────────────┐
          │                             │                             │
          ▼                             ▼                             ▼
┌─────────────────┐          ┌─────────────────┐          ┌─────────────────┐
│   ทดสอบส่ง      │          │   ทดสอบรับ      │          │   Troubleshoot  │
│   Outgoing      │          │   Incoming      │          │   แก้ปัญหา      │
└────────┬────────┘          └────────┬────────┘          └────────┬────────┘
         │                            │                            │
    ┌────┴────┐               ┌───────┼───────┐              ┌─────┴─────┐
    │         │               │       │       │              │           │
    ▼         ▼               ▼       ▼       ▼              ▼           ▼
┌───────┐ ┌───────┐    ┌──────┐ ┌──────┐ ┌──────┐    ┌───────────┐ ┌───────────┐
│Gmail  │ │Yahoo  │    │Gmail │ │Yahoo │ │Hotmail│   │ Spam Issue│ │Port Issue │
│Test   │ │Test   │    │Reply │ │Reply │ │Reply │    │ SPF/DKIM  │ │SSL/TLS    │
└───────┘ └───────┘    └──────┘ └──────┘ └──────┘    └───────────┘ └───────────┘
```

---

## Branch Details

### 1. ทดสอบส่ง (Outgoing)
- **ส่งไป Gmail:** ดูว่าเข้า Inbox หรือ Spam
- **ส่งไป Yahoo:** ทดสอบกับ provider อื่น
- **ส่งไป Hotmail:** ครอบคลุม major providers
- **เช็ค Headers:** SPF, DKIM, DMARC Pass

### 2. ทดสอบรับ (Incoming)
- **รับจาก Gmail:** ยืนยันว่ารับได้
- **รับจาก Yahoo:** ทดสอบ compatibility
- **Reply Test:** ตอบกลับได้ถูกต้อง
- **Attachment Test:** รับไฟล์แนบได้

### 3. Troubleshooting
- **Spam Issue:** ตั้งค่า SPF, DKIM, DMARC
- **Port Issue:** ใช้ Port ถูกต้อง
- **SSL Error:** เปิด SSL/TLS
- **Authentication:** Username/Password ถูกต้อง

---

## Key Connections

```
Send Test ─────► Check Inbox ─────► Verify Headers
     │                │                    │
     ▼                ▼                    ▼
 SMTP Works      No Spam             SPF/DKIM Pass
                     │                    │
                     ▼                    ▼
              Receive Test ────► Email Ready to Use
```

---

## Troubleshooting Flow

```
Problem?
    │
    ├─── Email เข้า Spam? ──► ตั้งค่า SPF, DKIM, DMARC
    │
    ├─── ส่งไม่ได้? ──► เช็ค SMTP: Port 465/587, SSL
    │
    ├─── รับไม่ได้? ──► เช็ค IMAP: Port 993, SSL
    │
    └─── Timeout? ──► เปลี่ยน Port, เช็ค Firewall
```

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
