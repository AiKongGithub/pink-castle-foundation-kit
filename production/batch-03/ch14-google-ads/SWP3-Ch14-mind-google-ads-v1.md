# Mind Map: Google Ads

> **Format:** Mind Map (Mermaid)
> **Source:** SWP3 Chapter 14
> **Nodes:** 60+
> **Production ID:** SWP3-Ch14-001-MIND

---

## Main Mind Map: Google Ads Overview

```mermaid
mindmap
  root((Google Ads))
    Campaign Types
      Search Ads
        Text ads
        High intent
        CPC billing
      Display Ads
        Banner ads
        Brand awareness
        Retargeting
      Shopping Ads
        Product images
        E-commerce
        Feed required
      YouTube Ads
        Video ads
        Skippable/Non-skip
        CPV/CPM
      Performance Max
        Automated
        Cross-channel
    Campaign Structure
      Account
        Billing
        Access
      Campaign
        Budget
        Bidding
        Location
        Schedule
      Ad Group
        Keywords
        Targeting
        Themes
      Ads
        Headlines
        Descriptions
        Extensions
    Keywords
      Match Types
        Broad
        Phrase
        Exact
        Negative
      Research
        Keyword Planner
        Search Volume
        CPC
        Competition
      Intent
        Informational
        Commercial
        Transactional
    Quality Score
      Components
        Expected CTR 40%
        Ad Relevance 30%
        Landing Page 30%
      Impact
        Ad Rank
        Actual CPC
        Position
    Bidding
      Manual
        Manual CPC
        Enhanced CPC
      Automated
        Target CPA
        Target ROAS
        Maximize Clicks
        Maximize Conversions
    Metrics
      CTR
        Target 3%+
      CPC
        Industry varies
      CPA
        Below margin
      ROAS
        Target 3x+
      Quality Score
        Target 7+
```

---

## Sub Mind Map 1: Campaign Types

```mermaid
mindmap
  root((Campaign Types))
    Search Ads
      Text-based
      High intent keywords
      Best for
        Lead generation
        Services
        B2B
      Billing CPC
    Display Ads
      Banner images
      Video
      Best for
        Brand awareness
        Retargeting
        Lookalike
      Billing CPM/CPC
    Shopping Ads
      Product images
      Price shown
      Best for
        E-commerce
        Retail
      Requires
        Merchant Center
        Product feed
    YouTube Ads
      Video content
      Best for
        Branding
        Awareness
        Tutorials
      Formats
        Skippable
        Non-skip
        Bumper
        Discovery
    Performance Max
      AI-powered
      All channels
      Best for
        Automation
        Scale
```

---

## Sub Mind Map 2: Keyword Match Types

```mermaid
mindmap
  root((Match Types))
    Broad Match
      keyword
      Widest reach
      Less control
      Use with caution
      Best for
        Discovery
        After data
    Phrase Match
      "keyword"
      Medium reach
      Good balance
      Includes variants
      Best for
        Core keywords
        Scaling
    Exact Match
      [keyword]
      Most control
      Highest intent
      Best for
        Starting out
        High value terms
    Negative Keywords
      -keyword
      Block unwanted
      Essential
      Examples
        -free
        -cheap
        -DIY
    Strategy
      Start Exact
      Expand to Phrase
      Add Negatives
      Review Search Terms
```

---

## Sub Mind Map 3: Quality Score Deep Dive

```mermaid
mindmap
  root((Quality Score))
    Components
      Expected CTR
        40% weight
        Historical CTR
        Relevance signals
      Ad Relevance
        30% weight
        Keyword in ad
        Message match
      Landing Page
        30% weight
        Load speed
        Mobile friendly
        Content match
    Scoring
      1-3 Below average
      4-6 Average
      7-10 Above average
      Target 7+
    Impact
      Ad Rank
        QS x Max Bid
      Actual CPC
        Lower with high QS
      Position
        Better placement
      Eligibility
        Extensions show
    Improvement
      Add keywords to ads
      Improve landing page
      Test ad variations
      Negative keywords
```

---

## Sub Mind Map 4: Bidding Strategies

```mermaid
mindmap
  root((Bidding))
    Manual
      Manual CPC
        Full control
        Set each bid
        Best for starting
      Enhanced CPC
        Semi-automated
        Adjusts for conversions
        Good transition
    Automated
      Target CPA
        Set target cost
        Needs 30+ conversions
        Best for lead gen
      Target ROAS
        Set target return
        E-commerce focus
        Needs value tracking
      Maximize Clicks
        Get most clicks
        Traffic focus
        Budget limited
      Maximize Conversions
        Get most conversions
        Budget limited
        Needs conversion data
    Strategy Path
      1. Start Manual CPC
      2. Collect data 15-30 days
      3. Get 30+ conversions
      4. Switch to Target CPA
      5. Optimize and scale
```

---

## Process Flow: Google Ads Campaign Setup

```mermaid
flowchart TD
    A[Keyword Research] --> B[Create Campaign]
    B --> C[Set Budget & Bidding]
    C --> D[Create Ad Groups]
    D --> E[Add Keywords by Match Type]
    E --> F[Write Ads]
    F --> G[Add Extensions]
    G --> H[Set Conversion Tracking]
    H --> I[Launch]
    I --> J{Monitor}
    J --> K[Optimize]
    K --> J

    style A fill:#e1f5fe
    style H fill:#fff9c4
    style I fill:#c8e6c9
```

---

## Process Flow: Keyword Research to Quality Score

```mermaid
flowchart LR
    A[Keyword Research] --> B[Select Keywords]
    B --> C[Write Relevant Ads]
    C --> D[Create Landing Page]
    D --> E{Quality Score}
    E -->|7+| F[Good Position + Low CPC]
    E -->|<7| G[Improve Components]
    G --> C

    style F fill:#c8e6c9
    style G fill:#ffcdd2
```

---

## Comparison: Match Types Control vs Reach

```mermaid
flowchart TB
    subgraph Exact["[Exact Match]"]
        A[Highest Control]
        B[Lowest Reach]
        C[Highest Intent]
    end

    subgraph Phrase["\"Phrase Match\""]
        D[Medium Control]
        E[Medium Reach]
        F[Good Balance]
    end

    subgraph Broad["Broad Match"]
        G[Lowest Control]
        H[Highest Reach]
        I[Discovery]
    end

    Exact -->|Scale when data| Phrase
    Phrase -->|Scale when data| Broad
```

---

## Comparison: Bidding Strategy Selection

```mermaid
flowchart TB
    subgraph Starting["Starting Phase"]
        A[Manual CPC]
        B[Full Control]
        C[Learn Platform]
    end

    subgraph Growing["Growing Phase"]
        D[Enhanced CPC]
        E[Partial Automation]
        F[15+ Conversions]
    end

    subgraph Scaling["Scaling Phase"]
        G[Target CPA/ROAS]
        H[Full Automation]
        I[30+ Conversions]
    end

    Starting -->|Collect Data| Growing
    Growing -->|More Data| Scaling
```

---

## Production Notes

| Field | Value |
|-------|-------|
| Created | 2026-01-28 |
| Producer | จูล่ง |
| Total Nodes | 60+ |
| Diagrams | 8 |
| QC Status | Pending |

---

> *Pink Castle Foundation Kit v1.0*
