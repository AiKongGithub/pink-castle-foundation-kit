# วิธี Deploy Membership System — SOMT-005
> **Format:** Slides (Presentation)
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 5
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

### SLIDE 1: Title Slide

# Deploy Membership System
## Step-by-Step Guide บน Kartra

**SWP3 Chapter 30 — ตอนที่ 5 (ตอนจบ)**
PinkCastle Academy

*"จาก Mindset สู่ Implementation — ถึงเวลาลงมือทำ!"*

---

### SLIDE 2: Overview — 6 ขั้นตอน

## Deployment Roadmap

```
1. สร้าง Portal ──► 2. ตั้งค่า Levels ──► 3. Domain
       │                    │                   │
       ▼                    ▼                   ▼
4. SSL Setup ──► 5. Payment Setup ──► 6. Test & Go Live!
```

**เวลาโดยประมาณ: 2-4 ชั่วโมง** (ไม่รวมสร้าง Content)

---

### SLIDE 3: ขั้นตอนที่ 1 — สร้าง Portal

## สร้าง Membership Portal

**วิธีทำ:**
1. เข้า Kartra Dashboard
2. ไปที่ **Memberships** → **New Membership**
3. ตั้งชื่อ Membership
4. เลือก Template
5. ใส่ Description + Welcome Message

**Template ที่มีให้เลือก:**
- Modern (แนะนำ)
- Classic
- Sidebar Navigation

> **Tip:** เลือก Template ประหยัดเวลากว่าสร้างจากศูนย์

---

### SLIDE 4: ขั้นตอนที่ 2 — ตั้งค่า Levels

## Membership Levels Setup

**กด "Add Level" สร้าง 2 ระดับ:**

| Setting | Silver | Gold |
|---------|--------|------|
| ชื่อ Level | Silver Member | Gold Member |
| Access | Category 1-5 | ทุก Category |
| Drip Schedule | สัปดาห์ละ 1 Module | สัปดาห์ละ 1 Module |
| Locked Content | Gold Content = Locked | ไม่มี Lock |

**Access Rules:**
- Silver: เห็น Gold Content แต่ Lock → "Upgrade"
- Gold: เข้าถึงทุกอย่าง

---

### SLIDE 5: ขั้นตอนที่ 3 — Domain Configuration

## ตั้งค่า Domain

**ตัวเลือกที่ 1: Custom Domain (แนะนำ)**
```
Domain: members.yourbrand.com
DNS: CNAME → ชี้ไป Kartra
รอ: 1-48 ชั่วโมง (DNS Propagation)
```

**ตัวเลือกที่ 2: Kartra Subdomain**
```
Domain: yourbrand.kartra.com
DNS: ไม่ต้องตั้ง
ใช้งาน: ทันที
```

> **แนะนำ Custom Domain** เพื่อความ Professional

---

### SLIDE 6: ขั้นตอนที่ 4 — SSL Setup

## เปิดใช้ SSL (HTTPS)

**วิธีทำ:**
1. เข้า **Domain Settings**
2. กด **Enable SSL**
3. รอ Provision (ไม่เกิน 24 ชม.)

**ทำไมต้องมี SSL:**
- ความปลอดภัย (เข้ารหัสข้อมูล)
- ความน่าเชื่อถือ (กุญแจล็อค)
- Payment (Stripe/PayPal บังคับ HTTPS)

**Kartra ให้ SSL ฟรี!**

---

### SLIDE 7: ขั้นตอนที่ 5 — Payment Setup

## ตั้งค่าระบบรับเงิน

**Step 1: เชื่อมต่อ Payment Gateway**
- My Integrations → Stripe หรือ PayPal
- ใส่ API Keys

**Step 2: สร้าง Products**
| Product | ราคา | Billing |
|---------|------|---------|
| Silver Membership | 990 บาท | รายเดือน |
| Gold Membership | 2,990 บาท | รายเดือน |

**Step 3: เชื่อม Product ↔ Level**
- Silver Product → Silver Level
- Gold Product → Gold Level

**Step 4: ทดสอบด้วย Test Mode!**

---

### SLIDE 8: ขั้นตอนที่ 6 — Testing Checklist

## ทดสอบทุกอย่างก่อน Go Live

| # | รายการ | ผล |
|---|--------|-----|
| 1 | Signup Flow — สมัครได้? | [ ] |
| 2 | Payment — ชำระได้? (Test Card) | [ ] |
| 3 | Access — Silver ไม่เห็น Gold? | [ ] |
| 4 | Dripping — เนื้อหาเปิดตามตาราง? | [ ] |
| 5 | Welcome Email — ได้รับ? | [ ] |
| 6 | Cancel — เข้าไม่ได้หลัง Cancel? | [ ] |

**ทุกข้อต้องผ่าน!**

---

### SLIDE 9: Launch Strategy

## Soft Launch → Public Launch

**Soft Launch:**
- เปิดให้ 5-10 Beta Members
- ทดสอบกับผู้ใช้จริง
- เก็บ Feedback
- แก้ไขปัญหา
- สร้าง Testimonials แรก

**Public Launch:**
- ประกาศอย่างเป็นทางการ
- ใช้ Testimonials จาก Beta Members
- เปิด Affiliate Program
- Launch Campaign (Email + Social Media)

---

### SLIDE 10: Pre-Launch Content Checklist

## เตรียมให้พร้อมก่อน Go Live

| รายการ | สถานะ |
|--------|------|
| Welcome Message + Video | [ ] |
| Content อย่างน้อย 2 สัปดาห์ | [ ] |
| Welcome Email Sequence (7 วัน) | [ ] |
| Community Guidelines | [ ] |
| FAQ Page | [ ] |
| Upgrade Page (Silver → Gold) | [ ] |
| Cancellation Policy | [ ] |

---

### SLIDE 11: Series Recap

## Secret Of Millionaire Trainer — สรุป 5 ตอน

| ตอน | หัวข้อ | สิ่งที่ได้ |
|-----|--------|----------|
| 1 | Identity & Mindset | Niche, Authority, Expert Enough |
| 2 | Revenue Strategies | 6 ช่องทาง, Pricing, Premium Offer |
| 3 | Empire Model | Value Ladder, Ecosystem, Positioning |
| 4 | Membership System | Recurring Revenue, Community, Dripping |
| 5 | **Deploy** | **Technical Setup, Go Live!** |

**เส้นทาง: Mindset → Strategy → Framework → Design → Implementation**

---

### SLIDE 12: Key Takeaway

## สรุป SOMT-005

> **ความสำเร็จอยู่ที่การ "ลงมือทำ" ไม่ใช่แค่ "รู้"**

**จำให้ขึ้นใจ:**
1. 6 ขั้นตอน Deploy ทำตามทีละขั้น
2. อย่าข้ามขั้นตอน Testing
3. ใช้ Custom Domain เพื่อความ Professional
4. Soft Launch ก่อน Public Launch
5. เตรียม Content อย่างน้อย 2 สัปดาห์
6. **เริ่มเลย!**

**คุณมีทุกอย่างที่ต้องการแล้ว — เหลือแค่ลงมือทำ!**

---

*สิ้นสุด Slides — SOMT-005 | จำนวน 12 Slides*
