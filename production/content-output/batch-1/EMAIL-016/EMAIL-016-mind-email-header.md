# Mind Map: Email Header Design

> **Format:** Visual Mind Map (Text-based)
> **Source:** SWP3 - Email Header Customization
> **Production ID:** EMAIL-016-MIND

---

## Central Theme: Email Header Mastery

```
                         ┌─────────────────────────────────┐
                         │       EMAIL HEADER              │
                         │         MASTERY                 │
                         └──────────────┬──────────────────┘
                                        │
          ┌─────────────────────────────┼─────────────────────────────┐
          │                             │                             │
          ▼                             ▼                             ▼
┌─────────────────┐          ┌─────────────────┐          ┌─────────────────┐
│   Components    │          │    Branding     │          │  Deliverability │
└────────┬────────┘          └────────┬────────┘          └────────┬────────┘
         │                            │                            │
    ┌────┴────┬────┐           ┌──────┴──────┐              ┌──────┴──────┐
    │         │    │           │             │              │             │
    ▼         ▼    ▼           ▼             ▼              ▼             ▼
┌───────┐ ┌─────┐┌────┐  ┌─────────┐  ┌─────────┐   ┌──────────┐  ┌──────────┐
│ From  │ │Subj ││Pre │  │ Logo    │  │ Colors  │   │ SPF/DKIM │  │ Domain   │
│ Name  │ │ect  ││view│  │ Style   │  │ Consist │   │ DMARC    │  │ Custom   │
│ Email │ │Line ││Text│  └─────────┘  └─────────┘   └──────────┘  └──────────┘
└───────┘ └─────┘└────┘
```

---

## Branch Details

### 1. Header Components
- **From Name:** ชื่อที่แสดง (สำคัญที่สุด!)
- **From Email:** อีเมลผู้ส่ง
- **Reply-to:** อีเมลตอบกลับ
- **Subject Line:** หัวข้อ
- **Preview Text:** ข้อความ preview (35-90 ตัวอักษร)

### 2. Branding Elements
- **Logo:** ใน email body (ไม่ใช่ header)
- **Colors:** สีที่ consistent กับ brand
- **Typography:** Font ที่อ่านง่าย
- **Voice:** Tone เดียวกันทุกครั้ง

### 3. Deliverability Factors
- **Custom Domain:** ใช้ domain ของตัวเอง
- **SPF:** Sender Policy Framework
- **DKIM:** DomainKeys Identified Mail
- **DMARC:** Domain-based Authentication
- **Reputation:** ประวัติการส่ง

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
