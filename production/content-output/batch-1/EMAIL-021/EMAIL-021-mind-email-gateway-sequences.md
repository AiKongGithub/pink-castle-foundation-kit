# Mind Map: ใส่อีเมลที่ Gateway ใน Sequences

> **Format:** Visual Mind Map (Text-based)
> **Source:** SWP3 - Email Marketing: ใส่อีเมลที่ Gateway ใน Sequences
> **Production ID:** EMAIL-021-MIND

---

## Central Theme: Email Gateway & Sequences

```
                         ┌─────────────────────────────────┐
                         │    EMAIL GATEWAY & SEQUENCES    │
                         │    Email Automation Setup       │
                         └──────────────┬──────────────────┘
                                        │
          ┌─────────────────────────────┼─────────────────────────────┐
          │                             │                             │
          ▼                             ▼                             ▼
┌─────────────────┐          ┌─────────────────┐          ┌─────────────────┐
│   Gateway       │          │   Sequences     │          │   Integration   │
│   Configuration │          │   Types         │          │   Steps         │
└────────┬────────┘          └────────┬────────┘          └────────┬────────┘
         │                            │                            │
    ┌────┴────┐               ┌───────┼───────┐              ┌─────┴─────┐
    │         │               │       │       │              │           │
    ▼         ▼               ▼       ▼       ▼              ▼           ▼
┌───────┐ ┌───────┐    ┌──────┐ ┌──────┐ ┌──────┐    ┌───────────┐ ┌───────────┐
│SMTP   │ │Auth   │    │Welcome│ │Nurture│ │Sales │    │ Connect   │ │ Test      │
│Host   │ │Creds  │    │Series │ │Series │ │Funnel│    │ Gateway   │ │ & Launch  │
└───────┘ └───────┘    └──────┘ └──────┘ └──────┘    └───────────┘ └───────────┘
```

---

## Branch Details

### 1. Gateway Configuration
- **SMTP Host:** mail.yourdomain.com
- **Port:** 465 (SSL) หรือ 587 (TLS)
- **Username:** email@yourdomain.com
- **Password:** email password
- **Encryption:** SSL/TLS required

### 2. Sequence Types
- **Welcome Series:** ส่งเมื่อ subscribe (5-7 emails)
- **Nurture Series:** ส่งต่อเนื่องสร้าง relationship
- **Sales Funnel:** ส่งเมื่อ trigger action
- **Re-engagement:** ส่งเมื่อ inactive
- **Post-purchase:** ส่งหลังซื้อ

### 3. Integration Steps
- **Step 1:** Configure SMTP Gateway
- **Step 2:** Test connection
- **Step 3:** Create Sequence
- **Step 4:** Link Gateway to Sequence
- **Step 5:** Test & Activate

---

## Key Connections

```
SMTP Settings ─────► Gateway Configured ─────► Sequence Ready
      │                      │                      │
      ▼                      ▼                      ▼
  Credentials          Connection Test         Automation Active
      │                      │                      │
      └──────────────────────┴──────────────────────┘
                             │
                             ▼
                    24/7 Email Automation
```

---

## Sequence Flow Example

```
Subscriber Signs Up
        │
        ▼
┌─────────────────┐
│  Day 0: Welcome │ ──► Gateway ──► Email Sent
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Day 2: Value   │ ──► Gateway ──► Email Sent
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Day 5: Story   │ ──► Gateway ──► Email Sent
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  Day 7: Offer   │ ──► Gateway ──► Email Sent
└─────────────────┘
```

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
