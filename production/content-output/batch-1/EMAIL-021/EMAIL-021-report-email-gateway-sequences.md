# Research Report: ใส่อีเมลที่ Gateway ใน Sequences

> **Format:** Executive Summary Report
> **Source:** SWP3 - Email Marketing: ใส่อีเมลที่ Gateway ใน Sequences
> **Production ID:** EMAIL-021-REPORT

---

## Executive Summary

การเชื่อมต่อ Email Gateway กับ Sequences เป็นขั้นตอนสำคัญในการสร้างระบบ Email Automation ที่มีประสิทธิภาพ รายงานนี้ครอบคลุมความเข้าใจเกี่ยวกับ Gateway, ประเภทของ Sequences และขั้นตอนการตั้งค่าอย่างละเอียด

---

## Key Findings

### 1. Email Gateway คืออะไร?

| Component | Description | Purpose |
|-----------|-------------|---------|
| SMTP Gateway | จุดเชื่อมต่อส่ง email | ส่ง email ผ่าน server ของคุณ |
| Authentication | ยืนยันตัวตน | ป้องกัน spam & misuse |
| Connection | เชื่อมต่อกับ Sequence | Enable automation |
| Deliverability | ส่ง email สำเร็จ | Email ถึงผู้รับ |

**Insight:** Gateway ทำหน้าที่เป็น "สะพาน" เชื่อมระบบ Automation กับ Email Server ของคุณ

### 2. ประเภทของ Email Sequences

**5 Common Sequence Types:**

1. **Welcome Sequence**
   - Trigger: New subscriber
   - Length: 5-7 emails
   - Goal: Build relationship
   - Conversion: 50-80% open rate

2. **Nurture Sequence**
   - Trigger: After welcome
   - Length: Ongoing
   - Goal: Provide value
   - Conversion: Maintain engagement

3. **Sales Sequence**
   - Trigger: Page visit / Cart abandon
   - Length: 3-5 emails
   - Goal: Convert to sale
   - Conversion: 5-15%

4. **Re-engagement Sequence**
   - Trigger: 30-90 days inactive
   - Length: 3-5 emails
   - Goal: Win back
   - Conversion: 10-20%

5. **Post-purchase Sequence**
   - Trigger: After purchase
   - Length: 3-7 emails
   - Goal: Onboard & upsell
   - Conversion: Build loyalty

---

## Technical Specifications

### SMTP Gateway Settings

| Setting | Value | Notes |
|---------|-------|-------|
| Host | mail.yourdomain.com | หรือ smtp.yourdomain.com |
| Port (SSL) | 465 | Implicit TLS |
| Port (TLS) | 587 | STARTTLS |
| Username | email@yourdomain.com | Full email address |
| Password | Your email password | Keep secure |
| From Name | Your Name/Business | Display name |
| Reply-To | Same or different email | For responses |

### Sequence Configuration

| Setting | Recommended | Reason |
|---------|-------------|--------|
| Send Limit | 100-500/day | Warm up new domain |
| Time Between | 2-3 days | Not too frequent |
| Send Time | 9-11 AM local | Highest open rates |
| Timezone | Subscriber's | Personalization |

---

## Implementation Guide

### Step 1: Configure Gateway

```
Settings → Email → SMTP Gateway
    │
    ├── Host: mail.yourdomain.com
    ├── Port: 465 (SSL)
    ├── Username: email@yourdomain.com
    ├── Password: ********
    └── Click "Test Connection"
```

### Step 2: Create Sequence

```
Automation → Sequences → Create New
    │
    ├── Name: Welcome Sequence
    ├── Trigger: On Subscribe
    └── Add Emails:
        ├── Email 1: Welcome (Day 0)
        ├── Email 2: Value (Day 2)
        ├── Email 3: Story (Day 4)
        └── Email 4: Offer (Day 7)
```

### Step 3: Connect & Test

```
Sequence Settings → Send From → Select Gateway
    │
    ├── Send Test Email
    ├── Verify Received
    └── Activate Sequence
```

---

## Recommendations

### For Setup:
1. ใช้ SMTP จาก Cpanel email ที่สร้างไว้
2. ทดสอบ Gateway ก่อน activate sequence
3. เริ่มจาก Welcome Sequence ก่อน
4. Monitor open/click rates

### For Optimization:
1. ส่ง email ในช่วงเวลาที่ผู้รับ active
2. ใช้ Personalization (ชื่อ, สนใจอะไร)
3. A/B Test subject lines
4. Track & improve continuously

---

## Conclusion

การตั้งค่า Email Gateway และเชื่อมต่อกับ Sequences เป็นรากฐานของ Email Automation ที่มีประสิทธิภาพ เมื่อตั้งค่าถูกต้อง ระบบจะทำงานให้อัตโนมัติ ช่วยสร้าง relationship กับ subscribers และเพิ่ม conversion

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
