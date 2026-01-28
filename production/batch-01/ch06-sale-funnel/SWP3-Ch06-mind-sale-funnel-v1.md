# Mind Map: Sale Funnel Mastery

> **Format:** Mermaid Mind Map
> **Source:** SWP3 Chapter 6
> **Nodes:** 60+
> **Production ID:** SWP3-Ch06-001-MIND

---

## Mind Map Diagram

```mermaid
mindmap
  root((Sales Funnel<br/>Mastery))
    Definition[Funnel คืออะไร]
      ระบบอัตโนมัติ
      พาลูกค้าจากรู้จัก→ซื้อ
      ทำงาน 24/7
      Scalable
      Measurable
    Stages[5 Stages]
      Awareness
        รู้จัก
        Traffic Sources
      Interest
        สนใจ
        Landing Page
        Lead Magnet
      Decision
        ตัดสินใจ
        Email Sequence
        Webinar
      Action
        ซื้อ
        Sales Page
        Order Form
      Retention
        ซื้อซ้ำ
        Upsell
        Cross-sell
    Types[Funnel Types]
      Lead Magnet Funnel
        สร้าง List
        Free Offer
      Trip Wire Funnel
        เปลี่ยน Subscriber→Buyer
        $7-47
      Webinar Funnel
        High-Ticket
        $297+
    LandingPage[Landing Page]
      Above Fold
        Headline
        Hero Image
        CTA
      Below Fold
        Problem
        Solution
        Benefits
        Social Proof
        FAQ
    Email[Email Sequence]
      Welcome 5-7 emails
      Launch 7-10 emails
      Nurture ongoing
    Metrics[Metrics]
      Opt-in Rate 20-40%
      Open Rate 20-30%
      Conversion 1-5%
      AOV
      LTV
```

---

## Funnel Flow Diagram

```mermaid
flowchart TB
    subgraph Traffic
        A1[YouTube]
        A2[FB Ads]
        A3[Blog]
    end

    subgraph Capture
        B[Landing Page]
        C[Lead Magnet]
    end

    subgraph Nurture
        D[Email Sequence]
        E[Value Content]
    end

    subgraph Convert
        F[Sales Page]
        G[Order Form]
    end

    subgraph Maximize
        H[Upsell]
        I[Cross-sell]
    end

    A1 --> B
    A2 --> B
    A3 --> B
    B --> C
    C --> D
    D --> E
    E --> F
    F --> G
    G --> H
    H --> I
```

---

## 5 Stages Funnel

```mermaid
flowchart LR
    subgraph S1[Stage 1]
        A[Awareness<br/>รู้จัก]
    end

    subgraph S2[Stage 2]
        B[Interest<br/>สนใจ]
    end

    subgraph S3[Stage 3]
        C[Decision<br/>ตัดสินใจ]
    end

    subgraph S4[Stage 4]
        D[Action<br/>ซื้อ]
    end

    subgraph S5[Stage 5]
        E[Retention<br/>ซื้อซ้ำ]
    end

    A --> B --> C --> D --> E
    E -.-> |Referral| A
```

---

## Email Sequence Timeline

```mermaid
gantt
    title Welcome Email Sequence
    dateFormat  YYYY-MM-DD
    section Week 1
    Welcome + Deliver     :d1, 2026-01-01, 1d
    About Me             :d2, after d1, 1d
    Value Email 1        :d3, after d2, 1d
    Story Email          :d4, after d3, 1d
    Value Email 2        :d5, after d4, 1d
    Soft Pitch           :d6, after d5, 1d
    section Week 2
    Direct Pitch         :d7, after d6, 2d
```

---

## Funnel Types Comparison

```mermaid
flowchart TB
    subgraph LMF[Lead Magnet Funnel]
        LM1[Landing] --> LM2[Thank You]
        LM2 --> LM3[Email Nurture]
    end

    subgraph TWF[Trip Wire Funnel]
        TW1[Landing] --> TW2[OTO $27]
        TW2 --> TW3[Upsell]
    end

    subgraph WF[Webinar Funnel]
        W1[Register] --> W2[Webinar]
        W2 --> W3[Sales Page]
        W3 --> W4[Order]
    end

    style LMF fill:#90EE90
    style TWF fill:#FFD700
    style WF fill:#FF69B4
```

---

## Landing Page Structure

```mermaid
flowchart TB
    subgraph Above[Above the Fold]
        H[Headline]
        SH[Subheadline]
        Hero[Hero Image/Video]
        CTA1[CTA Button]
    end

    subgraph Below[Below the Fold]
        P[Problem]
        S[Solution]
        B[Benefits]
        SP[Social Proof]
        F[FAQ]
        CTA2[CTA Button]
    end

    H --> SH --> Hero --> CTA1
    CTA1 --> P --> S --> B --> SP --> F --> CTA2

    style CTA1 fill:#FF69B4
    style CTA2 fill:#FF69B4
```

---

## Metrics Dashboard

```mermaid
pie title Funnel Conversion
    "Visitors" : 100
    "Leads (30%)" : 30
    "Trip Wire Buyers (10%)" : 3
    "Core Buyers (5%)" : 1.5
```

---

## Usage Instructions

1. **View Online:** Copy mermaid code to [mermaid.live](https://mermaid.live)
2. **Export:** PNG สำหรับ presentation, PDF สำหรับ print
3. **Customize:** แก้ไขสี, ขนาด ตามต้องการ

---

## Production Notes

| Field | Value |
|-------|-------|
| Created | 2026-01-28 |
| Producer | จูล่ง |
| Main Concepts | 6 |
| Total Nodes | 65+ |
| QC Status | Pending |

---

> *Pink Castle Foundation Kit v1.0*
