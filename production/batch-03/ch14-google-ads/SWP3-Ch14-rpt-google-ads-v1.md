# Report: Google Ads

> **Format:** Detailed Report
> **Source:** SWP3 Chapter 14
> **Pages:** 16
> **Production ID:** SWP3-Ch14-001-RPT

---

## Executive Summary

Google Ads เป็น Paid Advertising Platform อันดับ 1 ของโลก มี 8.5 พันล้านค้นหาต่อวัน รายงานนี้ครอบคลุม Campaign Types, Keyword Research, Match Types, Quality Score, Bidding Strategies, Ad Copy, Extensions และ Conversion Tracking

---

## 1. Google Ads Overview

### 1.1 Why Google Ads?

| Advantage | Description |
|-----------|-------------|
| Intent-Based | คนค้นหาสิ่งที่ต้องการอยู่แล้ว |
| Reach | 8.5 พันล้านค้นหาต่อวัน |
| Network | Search, Display, YouTube, Shopping |
| Precision | Keyword + Audience Targeting |
| Measurable | Conversion Tracking ครบถ้วน |

### 1.2 Platform Statistics

| Metric | Value |
|--------|-------|
| Daily Searches | 8.5 billion |
| Market Share | 92% |
| Average Search CTR (Position 1) | 27.6% |
| Average Display CTR | 0.46% |
| Businesses Using Google Ads | 80% globally |

---

## 2. Campaign Types

### 2.1 Search Ads

**Best For:** High-intent keywords, Lead gen, Services, B2B

**How It Works:**
1. ผู้ใช้ค้นหา keyword
2. โฆษณาแสดงในผลค้นหา
3. จ่ายเมื่อมีคนคลิก (CPC)

**Pros:**
- Intent สูงมาก
- Conversion rate ดี
- วัดผลง่าย

**Cons:**
- CPC อาจสูงใน competitive keywords
- ต้องมี keyword research ที่ดี

### 2.2 Display Ads

**Best For:** Brand awareness, Retargeting, Lookalike

**Targeting Options:**
| Type | Description |
|------|-------------|
| Audiences | In-market, Affinity |
| Topics | หมวดหมู่เว็บไซต์ |
| Placements | เว็บไซต์เฉพาะ |
| Keywords | Contextual targeting |
| Remarketing | คนที่เคยเข้าเว็บ |

**Ad Sizes:**
| Size | Name | Best For |
|------|------|----------|
| 300x250 | Medium Rectangle | Universal |
| 336x280 | Large Rectangle | In-content |
| 728x90 | Leaderboard | Header |
| 160x600 | Wide Skyscraper | Sidebar |
| 300x600 | Half Page | High impact |

### 2.3 Shopping Ads

**Best For:** E-commerce, Retail

**Requirements:**
1. Google Merchant Center account
2. Product feed (XML/CSV)
3. E-commerce website
4. Pricing & availability data

**Feed Optimization:**
| Field | Best Practice |
|-------|--------------|
| Title | Include keywords + brand + attributes |
| Description | Detailed product info |
| Images | High quality, white background |
| Price | Accurate, competitive |
| GTIN | Include when available |

### 2.4 YouTube Ads

**Best For:** Branding, Awareness, Tutorial content

| Format | Length | Skippable | Billing |
|--------|--------|-----------|---------|
| Skippable In-Stream | Any (skip after 5s) | Yes | CPV (30s or full) |
| Non-Skip In-Stream | 15s max | No | CPM |
| Bumper | 6s | No | CPM |
| Discovery | Thumbnail | N/A | CPC |
| Shorts | 60s max | Varies | CPV/CPM |

### 2.5 Performance Max

**Best For:** Automated cross-channel advertising

**Features:**
- AI-powered optimization
- Runs across all Google networks
- Requires conversion tracking
- Less manual control

---

## 3. Campaign Structure

### 3.1 Hierarchy

```
Account (บัญชี)
    │
    └── Campaign (Budget + Settings)
            │
            └── Ad Group (Keywords + Targeting)
                    │
                    └── Ads (Headlines + Descriptions)
                            │
                            └── Keywords (Match Types)
```

### 3.2 Campaign Level Settings

| Setting | Options |
|---------|---------|
| Campaign Type | Search, Display, Shopping, YouTube |
| Goal | Sales, Leads, Traffic, Awareness |
| Budget | Daily budget amount |
| Bidding | Manual, Automated |
| Location | Countries, Cities, Radius |
| Language | Target languages |
| Schedule | Days, Hours |

### 3.3 Ad Group Best Practices

- จัดกลุ่ม Keywords ที่เกี่ยวข้องกัน
- 10-20 keywords ต่อ Ad Group
- Ads ตรงกับ Keywords ในกลุ่ม
- ใช้ single keyword ad groups (SKAGs) สำหรับ high-value terms

---

## 4. Keyword Research

### 4.1 Research Tools

| Tool | Cost | Features |
|------|------|----------|
| Google Keyword Planner | Free | Search volume, CPC estimates |
| SEMrush | $129/mo | Competitor keywords, Gap analysis |
| Ahrefs | $99/mo | Keyword difficulty, SERP analysis |
| Ubersuggest | Free/$29/mo | Basic research |
| SpyFu | $39/mo | Competitor PPC history |

### 4.2 Key Metrics

| Metric | What It Means |
|--------|---------------|
| Search Volume | จำนวนค้นหาต่อเดือน |
| CPC | ราคาโดยประมาณต่อคลิก |
| Competition | ระดับการแข่งขัน (Low/Medium/High) |
| Keyword Difficulty | ความยากในการ rank |

### 4.3 Keyword Intent

| Type | Intent Level | Example | CPC |
|------|-------------|---------|-----|
| Informational | ต่ำ | "วิธีลดน้ำหนัก" | ต่ำ |
| Navigational | กลาง | "Nike official" | กลาง |
| Commercial | สูง | "รีวิว iPhone 16" | สูง |
| Transactional | สูงมาก | "ซื้อ iPhone 16" | สูงมาก |

**Focus on:** Commercial และ Transactional keywords สำหรับ conversions

---

## 5. Keyword Match Types

### 5.1 Match Type Comparison

| Match Type | Symbol | Control | Reach | Best For |
|------------|--------|---------|-------|----------|
| Exact | [keyword] | สูงสุด | ต่ำสุด | Starting, High-value |
| Phrase | "keyword" | กลาง | กลาง | Core keywords |
| Broad | keyword | ต่ำสุด | สูงสุด | Discovery |
| Negative | -keyword | - | - | Filtering |

### 5.2 Examples

**Keyword: รองเท้าวิ่ง**

| Match Type | Triggers When Search Is |
|------------|------------------------|
| Broad: รองเท้าวิ่ง | รองเท้ากีฬา, รองเท้าออกกำลังกาย, sneakers |
| Phrase: "รองเท้าวิ่ง" | รองเท้าวิ่งผู้หญิง, ซื้อรองเท้าวิ่ง, รองเท้าวิ่ง Nike |
| Exact: [รองเท้าวิ่ง] | รองเท้าวิ่ง, รองเท้าวิ่ง (close variants) |

### 5.3 Negative Keywords Strategy

**Common Negative Keywords:**
- ฟรี, free
- DIY, ทำเอง
- วิธี (สำหรับ commercial intent)
- รีวิว (ถ้าต้องการ transactional)
- เงินเดือน, salary
- ตัวอย่าง, template

**Process:**
1. Review Search Terms Report weekly
2. Add irrelevant searches as negatives
3. Create negative keyword lists
4. Apply to campaigns/ad groups

---

## 6. Quality Score

### 6.1 Components

| Component | Weight | What Google Measures |
|-----------|--------|---------------------|
| Expected CTR | 40% | Historical CTR, relevance signals |
| Ad Relevance | 30% | Keyword in ad, message match |
| Landing Page Experience | 30% | Load speed, mobile-friendly, content match |

### 6.2 Scoring Scale

| Score | Rating | Action |
|-------|--------|--------|
| 1-3 | Below Average | Immediate improvement needed |
| 4-6 | Average | Room for improvement |
| 7-10 | Above Average | Maintain and optimize |

### 6.3 Impact on Performance

**Ad Rank Formula:**
```
Ad Rank = Max Bid × Quality Score
```

**Example:**
| Advertiser | Max Bid | QS | Ad Rank | Position |
|------------|---------|-----|---------|----------|
| A | $3.00 | 10 | 30 | 1 |
| B | $4.00 | 6 | 24 | 2 |
| C | $5.00 | 4 | 20 | 3 |

Advertiser A wins despite lowest bid!

### 6.4 Improvement Strategies

**For Expected CTR:**
- Write compelling headlines
- Use numbers and statistics
- Add urgency
- Test multiple variations

**For Ad Relevance:**
- Include keyword in headline
- Match ad to search intent
- Use dynamic keyword insertion

**For Landing Page:**
- Improve load speed
- Make mobile-friendly
- Match content to ad promise
- Add clear CTA

---

## 7. Bidding Strategies

### 7.1 Manual Bidding

| Strategy | Description | Best For |
|----------|-------------|----------|
| Manual CPC | กำหนด bid เองทุก keyword | เริ่มต้น, Full control |
| Enhanced CPC | Google ปรับ bid ตาม conversion likelihood | Transition to automated |

### 7.2 Automated Bidding

| Strategy | Description | Requirements | Best For |
|----------|-------------|--------------|----------|
| Target CPA | กำหนด target cost per acquisition | 30+ conversions | Lead gen |
| Target ROAS | กำหนด target return on ad spend | Value tracking | E-commerce |
| Maximize Clicks | หา clicks มากที่สุด | None | Traffic focus |
| Maximize Conversions | หา conversions มากที่สุด | Conversion tracking | Budget limited |
| Maximize Conversion Value | หา value มากที่สุด | Value tracking | E-commerce |

### 7.3 Recommended Path

```
Phase 1: Manual CPC
    ↓ (15-30 days, collect data)
Phase 2: Enhanced CPC
    ↓ (30+ conversions)
Phase 3: Target CPA or Maximize Conversions
    ↓ (Scale)
Phase 4: Target ROAS (if e-commerce)
```

---

## 8. Ad Copy Best Practices

### 8.1 Responsive Search Ads (RSA)

| Element | Quantity | Display |
|---------|----------|---------|
| Headlines | Up to 15 | Shows 3 |
| Descriptions | Up to 4 | Shows 2 |
| URL Path | 2 fields | 15 chars each |

### 8.2 Headline Strategies

| Strategy | Example |
|----------|---------|
| Include Keyword | "รองเท้าวิ่ง Nike" |
| Add Benefit | "รองเท้าวิ่ง - น้ำหนักเบา สบายเท้า" |
| Add CTA | "สั่งซื้อรองเท้าวิ่งวันนี้" |
| Use Numbers | "รองเท้าวิ่ง ลด 50%" |
| Create Urgency | "รองเท้าวิ่ง - เหลือ 3 วันสุดท้าย" |

### 8.3 Description Strategies

- Expand on headline benefits
- Include features
- Add social proof
- Clear CTA
- Mention guarantee/warranty

---

## 9. Ad Extensions (Assets)

### 9.1 Extension Types

| Extension | Purpose | CTR Impact |
|-----------|---------|------------|
| Sitelink | ลิงก์เพิ่มเติม | +10-20% |
| Callout | USPs (non-clickable) | +10% |
| Structured Snippet | Features list | +5-10% |
| Call | Phone number | +5% (mobile) |
| Location | Store address | +10% (local) |
| Price | Product pricing | +10% |
| Image | Product images | +15% |
| Promotion | Special offers | +10% |

### 9.2 Best Practices

- Add ALL relevant extensions
- Keep sitelinks updated
- Use callouts for USPs: "ส่งฟรี", "รับประกัน 1 ปี"
- Schedule call extensions during business hours
- Test different combinations

---

## 10. Conversion Tracking

### 10.1 Setup Process

1. **Create Conversion Action** in Google Ads
2. **Install Google Tag** on website
3. **Configure Conversion Goals** (primary/secondary)
4. **Test with Tag Assistant** or Preview mode

### 10.2 Conversion Types

| Type | Track When |
|------|------------|
| Website purchases | Order completed |
| Lead form submissions | Form submitted |
| Phone calls | Call made/received |
| App downloads | App installed |
| Store visits | Physical store visit |

### 10.3 Attribution Models

| Model | Credit Distribution |
|-------|-------------------|
| Last Click | 100% to last click |
| First Click | 100% to first click |
| Linear | Equal across all |
| Time Decay | More to recent |
| Position-Based | 40-20-40 |
| Data-Driven | ML-based |

---

## 11. Google Ads Editor

### 11.1 Benefits

- Work offline
- Bulk edits
- Copy/Paste campaigns
- Find & Replace
- Export/Import
- Review changes before upload

### 11.2 Best Practices

- Use for large campaigns
- Draft mode → Review → Upload
- Backup before major changes
- Use for A/B test setup
- Export regularly for backup

---

## 12. Key Metrics

### 12.1 Performance Metrics

| Metric | Formula | Good | Excellent |
|--------|---------|------|-----------|
| CTR | Clicks/Impressions | > 3% | > 5% |
| CPC | Cost/Clicks | Industry varies | - |
| CPA | Cost/Conversions | < Margin | < 50% margin |
| ROAS | Revenue/Ad Spend | > 3x | > 5x |
| Quality Score | Google rating | > 5 | > 7 |
| Conversion Rate | Conv/Clicks | > 2% | > 5% |

### 12.2 Diagnostic Metrics

| Problem | Indicator | Solution |
|---------|-----------|----------|
| Low CTR | < 2% | Improve ad copy, relevance |
| High CPC | Above industry avg | Improve QS, use negatives |
| Low QS | < 5 | Improve 3 components |
| Low Impression Share | < 50% | Increase budget or bids |
| Low Conversion Rate | < 1% | Fix landing page |

---

## 13. Common Mistakes

| Mistake | Impact | Solution |
|---------|--------|----------|
| ไม่ติด Conversion Tracking | ไม่รู้ว่าได้ผล | ติดก่อนยิงโฆษณา |
| ใช้ Broad Match ตั้งแต่แรก | เสียเงินฟรี | เริ่มจาก Exact |
| ไม่ใส่ Negative Keywords | Clicks ไม่ relevant | Review Search Terms |
| QS ต่ำแต่ไม่แก้ | CPC สูง | ปรับ 3 components |
| ไม่ใส่ Extensions | CTR ต่ำ | ใส่ครบทุกอัน |
| Landing page ไม่ตรง | QS ต่ำ, Bounce สูง | Match ad promise |

---

## Key Takeaways

1. **Intent-based** - คนค้นหาสิ่งที่ต้องการอยู่แล้ว
2. **Quality Score matters** - ยิ่งสูง CPC ยิ่งถูก
3. **Start with Exact Match** - ควบคุมได้มากที่สุด
4. **Negative Keywords** - เพิ่มตลอดเวลา
5. **Extensions are essential** - ช่วย CTR 10-20%
6. **Track conversions first** - ก่อนยิงโฆษณา
7. **Manual → Automated** - เมื่อมี data พอ

---

## Production Notes

| Field | Value |
|-------|-------|
| Created | 2026-01-28 |
| Producer | จูล่ง |
| Sections | 13 |
| Tables | 30+ |
| QC Status | Pending |

---

> *Pink Castle Foundation Kit v1.0*
