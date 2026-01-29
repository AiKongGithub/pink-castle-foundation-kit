# Data Table: ใส่อีเมลที่ Gateway ใน Sequences

> **Format:** Data Tables & Reference
> **Source:** SWP3 - Email Marketing: ใส่อีเมลที่ Gateway ใน Sequences
> **Production ID:** EMAIL-021-DATA

---

## Table 1: SMTP Gateway Settings

| Setting | Value | Description |
|---------|-------|-------------|
| Host | mail.yourdomain.com | SMTP server address |
| Port (SSL) | 465 | Implicit TLS |
| Port (TLS) | 587 | STARTTLS |
| Username | email@yourdomain.com | Full email address |
| Password | Your email password | Keep secure |
| Encryption | SSL/TLS | Required |
| From Name | Your Name/Business | Display name |
| Reply-To | same or different | Where replies go |

---

## Table 2: Sequence Types & Metrics

| Type | Trigger | Length | Avg Open Rate | Goal |
|------|---------|--------|---------------|------|
| Welcome | New signup | 5-7 emails | 50-80% | Build relationship |
| Nurture | After welcome | Ongoing | 20-30% | Provide value |
| Sales | Page visit/action | 3-5 emails | 15-25% | Convert to sale |
| Re-engagement | 30-90 days inactive | 3-5 emails | 10-20% | Win back |
| Post-purchase | After purchase | 3-7 emails | 30-50% | Onboard & upsell |
| Abandoned Cart | Cart left | 3 emails | 40-50% | Recover sale |

---

## Table 3: Welcome Sequence Template

| Email # | Day | Subject Focus | Content | Goal |
|---------|-----|---------------|---------|------|
| 1 | 0 | Welcome! | Deliver lead magnet, set expectations | First impression |
| 2 | 2 | My Story | Why you do what you do | Build connection |
| 3 | 4 | Quick Win | Actionable tip/value | Establish expertise |
| 4 | 7 | Social Proof | Testimonials/case study | Build trust |
| 5 | 10 | Soft Offer | Mention product/service | Test interest |
| 6 | 14 | Main Offer | Clear CTA to buy | Convert |
| 7 | 21 | Follow-up | Reminder/objection handling | Close |

---

## Table 4: Email Timing Best Practices

| Factor | Recommendation | Reason |
|--------|---------------|--------|
| Days Between | 2-3 days | Balance frequency |
| Best Time | 9-11 AM | Highest open rates |
| Best Days | Tue, Wed, Thu | Highest engagement |
| Avoid | Mon AM, Fri PM | Low engagement |
| Timezone | Subscriber's local | Personalization |
| Weekend | Generally avoid | Lower open rates |

---

## Table 5: Domain Warm-up Schedule

| Week | Daily Volume | Total Sent | Notes |
|------|-------------|-----------|-------|
| 1 | 50 | 350 | Start slow |
| 2 | 100 | 1,050 | Double |
| 3 | 200 | 2,450 | Double again |
| 4 | 400 | 5,250 | Monitor carefully |
| 5 | 800 | 10,850 | Check deliverability |
| 6 | 1,500 | 21,350 | Near normal |
| 7+ | Full volume | Depends | Maintain |

---

## Table 6: Sequence Performance Benchmarks

| Metric | Poor | Average | Good | Excellent |
|--------|------|---------|------|-----------|
| Open Rate | <15% | 15-25% | 25-35% | >35% |
| Click Rate | <1% | 1-3% | 3-5% | >5% |
| Conversion | <0.5% | 0.5-2% | 2-5% | >5% |
| Unsubscribe | >1% | 0.5-1% | 0.2-0.5% | <0.2% |
| Bounce Rate | >5% | 2-5% | 1-2% | <1% |

---

## Table 7: Common Gateway Errors

| Error | Cause | Solution |
|-------|-------|----------|
| Authentication failed | Wrong credentials | Check email/password |
| Connection timeout | Port blocked | Try 587 instead of 465 |
| Relay denied | Server restriction | Use correct SMTP server |
| SSL error | Certificate issue | Enable SSL/TLS |
| Rate limit exceeded | Too many emails | Wait or increase limit |
| Blacklisted | Spam reports | Check blacklist, warm up |

---

## Table 8: Sequence Platform Comparison

| Platform | Free Tier | Sequences | Gateway Support | Best For |
|----------|-----------|-----------|-----------------|----------|
| Mailchimp | 500 contacts | Limited | Built-in | Beginners |
| Getresponse | 500 contacts | Advanced | Built-in | Marketers |
| ConvertKit | 300 contacts | Unlimited | Built-in | Creators |
| Kartra | None | Unlimited | Built-in + SMTP | All-in-one |
| ActiveCampaign | None | Advanced | Built-in + SMTP | Advanced |
| Custom (n8n) | Free | Unlimited | Any SMTP | Developers |

---

## Quick Reference Card

### Gateway Setup
```
Host: mail.yourdomain.com
Port: 465 (SSL) or 587 (TLS)
User: email@yourdomain.com
Pass: your-email-password
```

### Sequence Checklist
```
[ ] Configure Gateway
[ ] Test Connection
[ ] Create Sequence
[ ] Add 5-7 emails
[ ] Set timing (2-3 days)
[ ] Link Gateway
[ ] Test first email
[ ] Activate
```

### Key Metrics to Track
```
Open Rate: Target 25%+
Click Rate: Target 3%+
Unsubscribe: Keep <0.5%
Bounce: Keep <2%
```

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
