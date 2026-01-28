# Mind Map: Email Marketing

> **Format:** Mind Map (Mermaid)
> **Source:** SWP3 Chapter 12
> **Nodes:** 50+
> **Production ID:** SWP3-Ch12-001-MIND

---

## Main Mind Map: Email Marketing Overview

```mermaid
mindmap
  root((Email Marketing))
    Why Email?
      ROI สูงสุด
        $42 per $1
        4,200% ROI
      เป็นเจ้าของ List
        ไม่ขึ้นกับ Platform
        ไม่กลัวถูก Ban
      No Algorithm
        ส่งตรงถึง Inbox
        Open Rate 20-25%
      Automation
        ทำงาน 24/7
        Passive Income
    Building List
      Lead Magnets
        eBook/PDF
        Checklist
        Template
        Mini Course
        Free Trial
      Opt-in Placement
        Homepage
        Blog Posts
        Popup
        Exit Intent
    Email Types
      Welcome Email
      Newsletter
      Promotional
      Nurture Sequence
      Re-engagement
      Transactional
    Email Anatomy
      From Name
        ใช้ชื่อคน
        ไม่ใช่ noreply
      Subject Line
        < 50 ตัวอักษร
        ดึงดูดให้เปิด
      Preview Text
        ขยายความ Subject
      Body
        AIDA Formula
        80% Value
      CTA
        1 CTA หลัก
        ชัดเจน
      Footer
        Unsubscribe
        Physical Address
    Automation
      Welcome Sequence
        Day 0 Lead Magnet
        Day 1 Introduction
        Day 3-7 Value
        Day 10-14 Offer
      Cart Abandonment
        1 hour reminder
        24 hour urgency
        48 hour last chance
      Re-engagement
        Win back inactive
    Metrics
      Open Rate
        Target 20-30%
      Click Rate
        Target 2-5%
      Conversion Rate
      Unsubscribe Rate
        Target < 0.5%
    Platforms
      Mailchimp
        Free 500 contacts
        เริ่มต้นง่าย
      ConvertKit
        Free 1000 contacts
        สำหรับ Creators
      ActiveCampaign
        Advanced Automation
      Mailerlite
        Budget option
```

---

## Sub Mind Map 1: Subject Line Formulas

```mermaid
mindmap
  root((Subject Line))
    Curiosity
      สร้างความอยากรู้
      "คุณทำผิดพลาดนี้หรือเปล่า?"
      "ความลับที่ไม่มีใครบอก"
    Benefit
      บอกประโยชน์ชัด
      "วิธีเพิ่มยอดขาย 3 เท่า"
      "ประหยัดเวลา 10 ชั่วโมง/สัปดาห์"
    Urgency
      สร้างความเร่งด่วน
      "เหลืออีก 24 ชั่วโมง"
      "โอกาสสุดท้าย"
    Question
      ถามคำถาม
      "ทำไมยังไม่สำเร็จ?"
      "พร้อมหรือยัง?"
    Number
      ใช้ตัวเลข
      "5 เทคนิคที่ได้ผล"
      "3 ขั้นตอนง่ายๆ"
    Personal
      เรื่องส่วนตัว
      "สิ่งที่ผมเรียนรู้"
      "ความผิดพลาดของผม"
    Best Practices
      < 50 ตัวอักษร
      ใส่ชื่อคนรับ +26%
      Avoid Spam Words
      A/B Test
```

---

## Sub Mind Map 2: Welcome Sequence

```mermaid
mindmap
  root((Welcome Sequence))
    Day 0
      Welcome Email
      Deliver Lead Magnet
      Set Expectations
    Day 1-2
      Introduction
      Your Story
      Why You Help
    Day 3-4
      Value Email 1
      Quick Win
      Actionable Tip
    Day 5-6
      Value Email 2
      Common Mistakes
      How to Avoid
    Day 7-8
      Soft Pitch
      Introduce Product
      No Hard Sell
    Day 10
      Case Study
      Success Story
      Social Proof
    Day 14
      Main Offer
      Full Pitch
      CTA to Buy
```

---

## Sub Mind Map 3: Email Copywriting AIDA

```mermaid
mindmap
  root((AIDA Formula))
    A - Attention
      Strong Hook
      Question
      Surprising Fact
      Story Opening
      Avoid Boring Start
    I - Interest
      Tell Stories
      Share Data
      Relevant Examples
      Connect to Reader
    D - Desire
      Show Benefits
      Paint Picture
      Social Proof
      Handle Objections
    A - Action
      Clear CTA
      One Main Action
      Button or Link
      Create Urgency
```

---

## Sub Mind Map 4: Deliverability

```mermaid
mindmap
  root((Deliverability))
    Authentication
      SPF
      DKIM
      DMARC
    List Hygiene
      Double Opt-in
      Clean Inactive
        3-6 months no open
      Remove Bounces
    Content
      Avoid Spam Words
        FREE!
        URGENT!
        CLICK NOW!
      Good Text to Image Ratio
      Avoid ALL CAPS
    Sending
      Consistent Schedule
      Warm Up New Domain
      Monitor Reputation
    Engagement
      High Open Rate
      High Click Rate
      Low Complaints
```

---

## Process Flow: Email Marketing Funnel

```mermaid
flowchart TD
    A[Traffic] --> B[Landing Page]
    B --> C{Opt-in?}
    C -->|Yes| D[Welcome Sequence]
    C -->|No| E[Retarget]
    D --> F[Newsletter]
    F --> G[Promotional Email]
    G --> H{Purchase?}
    H -->|Yes| I[Customer Sequence]
    H -->|No| J[Nurture Sequence]
    J --> G
    I --> K[Upsell/Cross-sell]

    style A fill:#e1f5fe
    style D fill:#fff9c4
    style I fill:#c8e6c9
```

---

## Process Flow: A/B Testing

```mermaid
flowchart LR
    A[Choose Element] --> B[Create 2 Versions]
    B --> C[Split List 50/50]
    C --> D[Send Test]
    D --> E[Wait 2-4 hours]
    E --> F[Check Results]
    F --> G{Clear Winner?}
    G -->|Yes| H[Send Winner to Rest]
    G -->|No| I[Choose Based on Goal]
    H --> J[Document Learning]
    I --> J

    style H fill:#c8e6c9
```

---

## Comparison: ESP Platforms

```mermaid
flowchart TB
    subgraph Free["Free Tier"]
        A[Mailchimp 500]
        B[ConvertKit 1000]
        C[Mailerlite 1000]
        D[GetResponse 500]
    end

    subgraph Paid["Paid Features"]
        E[ActiveCampaign $29+]
        F[ConvertKit $15+]
        G[Mailchimp $13+]
    end

    subgraph BestFor["Best For"]
        H[Beginners → Mailchimp]
        I[Creators → ConvertKit]
        J[Automation → ActiveCampaign]
        K[Budget → Mailerlite]
    end
```

---

## Production Notes

| Field | Value |
|-------|-------|
| Created | 2026-01-28 |
| Producer | จูล่ง |
| Total Nodes | 50+ |
| Diagrams | 7 |
| QC Status | Pending |

---

> *Pink Castle Foundation Kit v1.0*
