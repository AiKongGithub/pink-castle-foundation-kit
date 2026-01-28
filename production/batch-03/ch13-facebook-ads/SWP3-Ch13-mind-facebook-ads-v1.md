# Mind Map: Facebook Ads

> **Format:** Mind Map (Mermaid)
> **Source:** SWP3 Chapter 13
> **Nodes:** 55+
> **Production ID:** SWP3-Ch13-001-MIND

---

## Main Mind Map: Facebook Ads Overview

```mermaid
mindmap
  root((Facebook Ads))
    Campaign Structure
      Campaign
        Objective
        Budget Type
      Ad Set
        Audience
        Budget
        Schedule
        Placements
      Ad
        Creative
        Copy
        CTA
    Objectives
      Awareness
        Brand Awareness
        Reach
      Consideration
        Traffic
        Engagement
        Video Views
        Lead Generation
        Messages
      Conversion
        Conversions
        Catalog Sales
        Store Traffic
    Targeting
      Demographics
        Age
        Gender
        Location
        Language
      Interests
        Pages Liked
        Activities
        Hobbies
      Behaviors
        Purchase
        Device
        Travel
      Custom Audiences
        Website Visitors
        Email List
        Video Viewers
        Engagers
      Lookalike
        1% Most Similar
        Scale to 10%
    Ad Formats
      Image
        1080x1080
        1200x628
      Video
        15 sec or less
        4:5 Feed
        9:16 Stories
      Carousel
        2-10 cards
      Collection
        E-commerce
      Stories/Reels
        1080x1920
    Pixel
      Standard Events
        PageView
        ViewContent
        AddToCart
        Purchase
        Lead
      Benefits
        Track Conversions
        Custom Audiences
        Optimize
    Metrics
      CPM
        Cost per 1000
      CPC
        Cost per Click
      CTR
        Click Through Rate
        Target 1%+
      CPA
        Cost per Acquisition
      ROAS
        Return on Ad Spend
      Frequency
        Target < 3
```

---

## Sub Mind Map 1: Campaign Objectives

```mermaid
mindmap
  root((Objectives))
    Awareness
      Brand Awareness
        ให้คนจำได้
      Reach
        เข้าถึงมากที่สุด
    Consideration
      Traffic
        คนเข้าเว็บ
        เริ่มต้นแนะนำ
      Engagement
        Like Comment Share
      Video Views
        ดูวิดีโอ
      Lead Generation
        เก็บ Lead
      Messages
        ส่งข้อความ
    Conversion
      Conversions
        ซื้อ สมัคร
        ต้องมี Pixel data
      Catalog Sales
        E-commerce
      Store Traffic
        ร้านค้าจริง
```

---

## Sub Mind Map 2: Targeting Strategy

```mermaid
mindmap
  root((Targeting))
    Cold Audiences
      Interests
        สิ่งที่สนใจ
        คู่แข่ง
      Lookalike 1-3%
        จากลูกค้า
        จากคนซื้อ
      Broad Targeting
        ให้ FB หา
        ต้องมี data เยอะ
    Warm Audiences
      Website Visitors
        เข้าเว็บ 30-180 วัน
      Video Viewers
        ดู 25-95%
      Engagers
        Like Comment
    Hot Audiences
      Add to Cart
        ใส่ตะกร้า
      Initiated Checkout
        เริ่ม checkout
      Past Purchasers
        ซื้อแล้ว
        Upsell
```

---

## Sub Mind Map 3: Ad Creative Best Practices

```mermaid
mindmap
  root((Creative))
    Visual
      First 3 Seconds
        หยุดนิ้ว
        สีสดใส
        ใบหน้าคน
      Video
        15 sec หรือน้อยกว่า
        4:5 Feed
        9:16 Stories
        Add Captions
      Image
        High Quality
        Clear Message
        Human Faces
    Copy
      PAS Formula
        Problem
        Agitate
        Solution
      AIDA
        Attention
        Interest
        Desire
        Action
      Headlines
        Benefit Focused
        Numbers Work
    CTA
      สมัครเลย
      ซื้อตอนนี้
      ดูเพิ่มเติม
      ส่งข้อความ
```

---

## Sub Mind Map 4: Facebook Pixel

```mermaid
mindmap
  root((Facebook Pixel))
    What It Does
      Track Events
      Build Audiences
      Optimize Ads
    Standard Events
      PageView
        ทุกหน้า
      ViewContent
        หน้าสินค้า
      AddToCart
        ใส่ตะกร้า
      InitiateCheckout
        เริ่ม checkout
      Purchase
        ซื้อสำเร็จ
      Lead
        กรอกฟอร์ม
    Use Cases
      Retargeting
        คนเข้าเว็บ
        คนใส่ตะกร้า
      Lookalike
        จากคนซื้อ
        จาก Lead
      Conversion Optimization
        หาคนที่จะซื้อ
```

---

## Process Flow: Facebook Ads Funnel

```mermaid
flowchart TD
    A[Cold Traffic] --> B[Awareness Ad]
    B --> C[Website Visit]
    C --> D[Pixel Tracks]
    D --> E[Retargeting Ad]
    E --> F{Convert?}
    F -->|Yes| G[Purchase]
    F -->|No| H[More Retargeting]
    H --> E
    G --> I[Lookalike Audience]
    I --> A

    style A fill:#e1f5fe
    style G fill:#c8e6c9
```

---

## Process Flow: Testing Framework

```mermaid
flowchart LR
    A[Start] --> B[Test Audiences]
    B --> C{Winner?}
    C -->|Yes| D[Test Creatives]
    C -->|No| B
    D --> E{Winner?}
    E -->|Yes| F[Test Copy]
    E -->|No| D
    F --> G{Winner?}
    G -->|Yes| H[Scale Budget]
    G -->|No| F
    H --> I[Monitor & Optimize]

    style H fill:#c8e6c9
```

---

## Comparison: Budget Strategies

```mermaid
flowchart TB
    subgraph Daily["Daily Budget"]
        A[ใช้ทุกวันเท่าๆ กัน]
        B[เหมาะกับ Testing]
        C[ควบคุมง่าย]
    end

    subgraph Lifetime["Lifetime Budget"]
        D[ตั้งงบรวมทั้งหมด]
        E[FB จัดการให้]
        F[เหมาะกับ Limited Offers]
    end

    subgraph CBO["Campaign Budget Optimization"]
        G[ตั้งงบที่ Campaign]
        H[FB แจกให้ Ad Sets ที่ดี]
        I[เหมาะกับ Scale]
    end
```

---

## Production Notes

| Field | Value |
|-------|-------|
| Created | 2026-01-28 |
| Producer | จูล่ง |
| Total Nodes | 55+ |
| Diagrams | 7 |
| QC Status | Pending |

---

> *Pink Castle Foundation Kit v1.0*
