# Video Summary: ใส่อีเมลที่ Gateway ใน Sequences

> **Format:** Video Summary Script
> **Source:** SWP3 - Email Marketing: ใส่อีเมลที่ Gateway ใน Sequences
> **Duration:** ~5-7 minutes
> **Production ID:** EMAIL-021-VIDEO

---

## Video Script

### [INTRO - 0:00-0:30]

**On Screen:** ใส่อีเมลที่ Gateway ใน Sequences

**Narrator:** วันนี้เราจะมาเรียนรู้การเชื่อมต่อ Email Gateway กับ Sequences เพื่อสร้างระบบ Email Automation ที่ทำงานให้คุณ 24/7

---

### [SECTION 1 - 0:30-1:30] ทำความเข้าใจ Gateway

**What is Gateway?**

```
Your Email (SMTP) ──► Gateway ──► Sequence System ──► Subscribers
```

**Key Components:**
- SMTP Host: mail.yourdomain.com
- Port: 465 (SSL) หรือ 587 (TLS)
- Username: email@yourdomain.com
- Password: your email password

---

### [SECTION 2 - 1:30-3:00] ทำความเข้าใจ Sequences

| Sequence Type | Trigger | Example |
|---------------|---------|---------|
| Welcome | Signup | Day 1, 3, 5, 7 emails |
| Nurture | Time-based | Weekly content |
| Sales | Page visit | Product pitch |
| Re-engagement | Inactivity | Win-back offer |

**Visual:** Animation แสดง email flow

---

### [SECTION 3 - 3:00-5:00] ตั้งค่า Gateway

**Step-by-Step:**

1. ไปที่ Settings → Email → SMTP Gateway
2. กรอก SMTP Host: `mail.yourdomain.com`
3. กรอก Port: `465` (SSL)
4. กรอก Username: full email address
5. กรอก Password: email password
6. คลิก "Test Connection"
7. Save Settings

**Visual:** Screen recording การตั้งค่า

---

### [SECTION 4 - 5:00-6:00] เชื่อมต่อกับ Sequences

**Steps:**
1. ไปที่ Automation → Sequences
2. เลือก Sequence ที่ต้องการ
3. ตั้งค่า "Send From" เป็น Gateway
4. ทดสอบส่ง email แรก
5. Activate Sequence

---

### [OUTRO - 6:00-6:30]

**Call to Action:**
- ตั้งค่า Gateway ของตัวเอง
- สร้าง Welcome Sequence แรก
- Subscribe เพื่อดูตอนต่อไป

---

## Production Notes

- Screen recording ตลอดการตั้งค่า
- Animation แสดง email flow
- Highlight ปุ่มที่ต้องคลิก

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
