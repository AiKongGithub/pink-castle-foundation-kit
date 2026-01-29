# Data Table: Email Header Design

> **Format:** Data Tables & Reference
> **Source:** SWP3 - Email Header Customization
> **Production ID:** EMAIL-016-DATA

---

## Table 1: Header Components

| Component | Max Length | Purpose | Example |
|-----------|------------|---------|---------|
| From Name | 20 chars | Brand recognition | "สมชาย จาก ABC" |
| From Email | - | Identification | hello@abc.com |
| Reply-to | - | Response routing | support@abc.com |
| Subject Line | 50 chars | Open rate driver | "3 เทคนิค..." |
| Preview Text | 35-90 chars | 2nd subject line | "ที่คุณต้องรู้..." |

---

## Table 2: From Name Strategies

| Strategy | Format | Example | Best For | Recognition |
|----------|--------|---------|----------|-------------|
| Personal | ชื่อจริง | "สมชาย" | Solo creators | Medium |
| Brand | ชื่อ brand | "ABC Company" | Large brands | High |
| Combined | ชื่อ + brand | "สมชาย จาก ABC" | Most cases | Highest |
| Role | ตำแหน่ง + brand | "ทีมบริการ ABC" | Support | Medium |
| Product | ชื่อ product | "ABC Course" | Product-specific | Medium |

---

## Table 3: Character Limits by Device

| Element | Desktop | Mobile (iOS) | Mobile (Android) | Gmail |
|---------|---------|--------------|------------------|-------|
| From Name | 20 | 15-20 | 18-20 | 20 |
| Subject | 60 | 35-40 | 40-45 | 70 |
| Preview | 100 | 35-50 | 40-60 | 90 |

---

## Table 4: Email Authentication Protocols

| Protocol | Full Name | Purpose | Required |
|----------|-----------|---------|----------|
| SPF | Sender Policy Framework | ระบุ server ที่มีสิทธิ์ส่ง | Yes |
| DKIM | DomainKeys Identified Mail | ลายเซ็นดิจิทัล | Yes |
| DMARC | Domain-based Message Auth | Policy enforcement | Recommended |
| BIMI | Brand Indicators for Message ID | แสดง logo | Optional |

---

## Table 5: Header Impact on Open Rate

| Factor | Impact | Notes |
|--------|--------|-------|
| Recognizable From Name | +35% | จำได้ = เปิด |
| Custom domain | +20% | Trust สูงขึ้น |
| Optimized preview text | +15% | เพิ่ม context |
| Mobile optimization | +25% | 60%+ เปิดบน mobile |
| Authentication (SPF/DKIM) | +15-30% | ไม่เข้า spam |

---

## Table 6: Domain Warm-up Schedule

| Week | Daily Volume | Notes |
|------|--------------|-------|
| Week 1 | 50-100 | เริ่มจากน้อย |
| Week 2 | 100-300 | เพิ่มทีละน้อย |
| Week 3 | 300-500 | Monitor bounce rate |
| Week 4 | 500-1,000 | ดู spam complaints |
| Week 5-8 | เพิ่ม 25%/week | จนถึง full volume |

---

## Table 7: Spam Trigger Words to Avoid

| Category | Words to Avoid |
|----------|----------------|
| Money | "ฟรี", "รวยเร็ว", "ไม่มีค่าใช้จ่าย" |
| Urgency | "ด่วน!!", "ทำเลย", "รีบ!!!" |
| Claims | "รับประกันผล", "100% สำเร็จ" |
| Symbols | "$$$", "!!!", "ALL CAPS" |

---

## Table 8: Header Checklist

| Task | Priority | Done |
|------|----------|------|
| **Setup** | | |
| ซื้อ custom domain | High | ☐ |
| Setup SPF record | High | ☐ |
| Setup DKIM | High | ☐ |
| Setup DMARC | Medium | ☐ |
| **Configuration** | | |
| ตั้ง From Name | High | ☐ |
| ตั้ง Reply-to | Medium | ☐ |
| สร้าง Preview Text template | High | ☐ |
| **Testing** | | |
| ทดสอบบน mobile | High | ☐ |
| ตรวจสอบ spam score | High | ☐ |
| A/B test From Name | Medium | ☐ |

---

## Quick Reference Card

### Header Formula
```
From Name: "ชื่อจริง จาก Brand" (20 chars)
From Email: hello@yourdomain.com
Subject: Front-load keywords (50 chars)
Preview: Complete the story (35-90 chars)
```

### Authentication Checklist
```
SPF:   v=spf1 include:_spf.google.com ~all
DKIM:  Setup in email provider dashboard
DMARC: v=DMARC1; p=none; rua=mailto:...
```

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
