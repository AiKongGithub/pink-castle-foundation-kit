# Mind Map: วิธีทำการตลาดออนไลน์ที่ได้ผล

> **Format:** Mermaid Mind Map
> **Source:** SWP3 Chapter 3
> **Nodes:** 50+
> **Production ID:** SWP3-Ch03-001-MIND

---

## Mind Map Diagram

```mermaid
mindmap
  root((การตลาดออนไลน์<br/>ที่ได้ผล))
    3M[3M Marketing]
      Message
        สิ่งที่จะสื่อสาร
        ตรงกลุ่มเป้าหมาย
        ชัดเจน
      Market
        กลุ่มเป้าหมาย
        Avatar
        Pain Points
      Media
        ช่องทาง
        Platform
        Format
    AIDA[AIDA Model]
      A-Attention
        Headline
        Visual
        Hook
      I-Interest
        เล่าเรื่อง
        ให้ข้อมูล
        พูดถึงเขา
      D-Desire
        Benefits
        Social Proof
        Testimonials
      A-Action
        CTA
        Urgency
        ลด Friction
    Content[Content Marketing]
      Pillars
        Educational
        Inspirational
        Entertaining
        Promotional
      Types
        Short Video
        Long Video
        Blog
        Carousel
        Stories
        Live
      Repurpose
        1 Content
        Multi Platform
        Save Time
    Traffic[Traffic Channels]
      Organic
        YouTube
        Blog/SEO
        Social Media
        Podcast
      Paid
        Facebook Ads
        Google Ads
        YouTube Ads
    Conversion[Conversion]
      Landing Page
        Headline
        Benefits
        CTA
        Social Proof
      AB Testing
        Test ทีละอย่าง
        วัดผล
        ปรับปรุง
```

---

## AIDA Flow Diagram

```mermaid
flowchart LR
    subgraph AIDA["AIDA Model"]
        A[Attention<br/>ดึงดูด] --> I[Interest<br/>สนใจ]
        I --> D[Desire<br/>อยากได้]
        D --> Act[Action<br/>ลงมือทำ]
    end

    A -.-> |Headline, Visual| A
    I -.-> |Story, Value| I
    D -.-> |Benefits, Proof| D
    Act -.-> |CTA, Urgency| Act
```

---

## Content Marketing Flow

```mermaid
flowchart TB
    subgraph Creation
        C[Create Content]
    end

    subgraph Distribution
        C --> YT[YouTube]
        C --> Blog[Blog]
        C --> SM[Social Media]
        C --> Email[Email]
    end

    subgraph Repurpose
        YT --> Shorts[Shorts]
        YT --> Pod[Podcast]
        Blog --> Carousel[Carousel]
        SM --> Stories[Stories]
    end

    subgraph Result
        Shorts --> Traffic
        Pod --> Traffic
        Carousel --> Traffic
        Stories --> Traffic
        Traffic --> Leads
        Leads --> Sales
    end
```

---

## Traffic Channels Comparison

```mermaid
quadrantChart
    title Traffic Channels
    x-axis ช้า --> เร็ว
    y-axis ราคาถูก --> ราคาแพง
    quadrant-1 เร็ว + แพง
    quadrant-2 ช้า + แพง
    quadrant-3 ช้า + ถูก
    quadrant-4 เร็ว + ถูก
    YouTube: [0.3, 0.2]
    Blog/SEO: [0.2, 0.15]
    Facebook Ads: [0.75, 0.7]
    Google Ads: [0.8, 0.85]
    YouTube Ads: [0.7, 0.5]
    TikTok: [0.5, 0.3]
```

---

## Landing Page Structure

```mermaid
flowchart TB
    subgraph LP[Landing Page]
        H[Headline] --> SH[Subheadline]
        SH --> Hero[Hero Image/Video]
        Hero --> Benefits[Benefits 3-5 ข้อ]
        Benefits --> Proof[Social Proof]
        Proof --> CTA1[CTA Button]
        CTA1 --> FAQ[FAQ]
        FAQ --> CTA2[CTA Button 2]
    end

    style H fill:#FF69B4
    style CTA1 fill:#FFD700
    style CTA2 fill:#FFD700
```

---

## Conversion Funnel Metrics

```mermaid
flowchart TB
    V[Visitors<br/>100%] --> O[Opt-in<br/>30%]
    O --> C[Click Email<br/>10%]
    C --> S[Sale<br/>3%]

    V -.-> |"Traffic Metrics"| V
    O -.-> |"Opt-in Rate 20-40%"| O
    C -.-> |"CTR 3-5%"| C
    S -.-> |"Conversion 1-5%"| S
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
| Main Concepts | 5 |
| Total Nodes | 55+ |
| QC Status | Pending |

---

> *Pink Castle Foundation Kit v1.0*
