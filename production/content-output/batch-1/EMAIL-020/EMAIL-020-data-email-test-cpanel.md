# Data Table: ทดลองส่งอีเมลจากระบบ Cpanel

> **Format:** Data Tables & Reference
> **Source:** SWP3 - Email Marketing: ทดลองส่งอีเมลจากระบบ Cpanel
> **Production ID:** EMAIL-020-DATA

---

## Table 1: Email Testing Matrix

| Test # | Type | From | To | Purpose | Pass Criteria |
|--------|------|------|----|---------| --------------|
| 1 | Outbound | Your Email | Gmail | Deliverability | Inbox, not Spam |
| 2 | Outbound | Your Email | Yahoo | Cross-provider | Inbox, not Spam |
| 3 | Outbound | Your Email | Hotmail | Microsoft check | Inbox, not Spam |
| 4 | Inbound | Gmail | Your Email | Receive test | Email received |
| 5 | Reply | Both | Both | Reply chain | Reply works |
| 6 | Attachment | Both | Both | File handling | Attachment OK |

---

## Table 2: Email Authentication Records

| Record | Purpose | Example Value | Check Method |
|--------|---------|---------------|--------------|
| SPF | Authorize senders | v=spf1 include:_spf.google.com ~all | dig TXT domain.com |
| DKIM | Digital signature | v=DKIM1; k=rsa; p=MIGf... | Email headers |
| DMARC | Policy & reporting | v=DMARC1; p=quarantine; rua=mailto:... | dig TXT _dmarc.domain.com |

---

## Table 3: Authentication Results Interpretation

| Status | SPF | DKIM | DMARC | Meaning | Action |
|--------|-----|------|-------|---------|--------|
| Excellent | Pass | Pass | Pass | Full authentication | Ready to use |
| Good | Pass | Pass | None | Partial auth | Add DMARC |
| Warning | Pass | Fail | - | DKIM issue | Fix DKIM |
| Critical | Fail | - | - | No SPF | Add SPF immediately |
| Spam Risk | Fail | Fail | Fail | No authentication | Fix all records |

---

## Table 4: Common SMTP Errors

| Error Code | Meaning | Cause | Solution |
|------------|---------|-------|----------|
| 535 | Auth failed | Wrong password | Check credentials |
| 550 | Relay denied | Wrong server | Use correct SMTP |
| 553 | Mailbox invalid | Typo in address | Check recipient |
| 421 | Timeout | Server busy | Retry later |
| 452 | Quota exceeded | Mailbox full | Clear space |

---

## Table 5: Common IMAP Errors

| Error Code | Meaning | Cause | Solution |
|------------|---------|-------|----------|
| Login failed | Auth error | Wrong credentials | Check email/password |
| Connection timeout | Port blocked | Firewall | Try port 993 SSL |
| Certificate error | SSL issue | Self-signed cert | Accept certificate |
| Mailbox not found | Wrong folder | IMAP path | Check folder names |

---

## Table 6: Email Ports Reference

| Protocol | Port | Security | Use Case |
|----------|------|----------|----------|
| IMAP | 993 | SSL/TLS | Receive (recommended) |
| IMAP | 143 | STARTTLS | Receive (legacy) |
| POP3 | 995 | SSL/TLS | Receive (download) |
| POP3 | 110 | None | Not recommended |
| SMTP | 465 | SSL/TLS | Send (recommended) |
| SMTP | 587 | STARTTLS | Send (alternative) |
| SMTP | 25 | None | Server-to-server only |

---

## Table 7: Mail-Tester Score Interpretation

| Score | Rating | Meaning | Action Needed |
|-------|--------|---------|---------------|
| 10/10 | Perfect | All checks passed | None |
| 8-9/10 | Good | Minor issues | Optional fixes |
| 6-7/10 | Fair | Some problems | Review recommendations |
| 4-5/10 | Poor | Major issues | Fix SPF/DKIM |
| <4/10 | Critical | High spam risk | Urgent fixes needed |

---

## Table 8: Bounce Rate Benchmarks

| Rate | Status | Meaning | Action |
|------|--------|---------|--------|
| <1% | Excellent | Very clean list | Maintain |
| 1-2% | Good | Normal | Monitor |
| 2-5% | Warning | List quality issue | Clean list |
| 5-10% | Critical | Major problems | Stop sending, clean |
| >10% | Dangerous | Sender reputation at risk | Immediate action |

---

## Quick Reference Card

### Testing Checklist
```
[ ] Outbound: Gmail, Yahoo, Hotmail
[ ] Inbound: Receive from external
[ ] Reply: Both directions
[ ] Attachment: Send and receive
[ ] Headers: SPF/DKIM/DMARC Pass
```

### Troubleshooting Quick Fixes
```
Spam Issue → Check SPF/DKIM/DMARC
Send Error → Port 465 SSL or 587 TLS
Receive Error → Port 993 SSL
Auth Error → Use full email as username
```

### Useful Tools
```
mail-tester.com → Spam score check
mxtoolbox.com → DNS/MX lookup
dmarcian.com → DMARC analyzer
```

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
