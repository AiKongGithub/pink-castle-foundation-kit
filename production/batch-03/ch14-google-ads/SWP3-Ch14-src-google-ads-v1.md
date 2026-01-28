# Source Summary: Google Ads

> **Chapter:** 14 - Google Ads
> **Source:** Speed Wealth Project 3
> **Duration:** 18:32:45
> **Files:** 28
> **Production ID:** SWP3-Ch14-001-SRC

---

## Chapter Overview

Google Ads เป็น Paid Advertising Platform อันดับ 1 ของโลก ครอบคลุม Search Ads, Display Ads, Shopping Ads, YouTube Ads พร้อมระบบ Keyword Targeting, Quality Score และ Conversion Tracking ที่ทรงพลัง

---

## Key Concepts

### 1. Why Google Ads?

- **Intent-Based**: คนค้นหาสิ่งที่ต้องการแล้ว
- **Reach**: 8.5 พันล้านค้นหา/วัน
- **Network**: Search, Display, YouTube, Shopping
- **Precision**: Keyword + Audience Targeting
- **Measurable**: Conversion Tracking ครบถ้วน

### 2. Types of Google Ads

| Type | Best For | Billing |
|------|----------|---------|
| Search Ads | High intent keywords | CPC |
| Display Ads | Brand awareness, Retargeting | CPM/CPC |
| Shopping Ads | E-commerce products | CPC |
| YouTube Ads | Video content, Branding | CPV/CPM |
| Performance Max | Automated cross-channel | CPA |

### 3. Campaign Structure

```
Account
    └── Campaign (Budget + Settings)
            └── Ad Group (Keywords + Targeting)
                    └── Ads (Headlines + Descriptions)
                            └── Keywords (Match Types)
```

### 4. Keyword Research

**Tools:**
- Google Keyword Planner (Free)
- SEMrush
- Ahrefs
- Ubersuggest

**Metrics to Consider:**
- Search Volume (ปริมาณการค้นหา)
- CPC (ราคาต่อคลิก)
- Competition (ระดับการแข่งขัน)
- Keyword Difficulty

**Keyword Types:**
| Type | Intent | Example | CPC |
|------|--------|---------|-----|
| Informational | ต่ำ | "วิธีลดน้ำหนัก" | ต่ำ |
| Navigational | กลาง | "Nike official" | กลาง |
| Commercial | สูง | "รีวิว iPhone 16" | สูง |
| Transactional | สูงมาก | "ซื้อ iPhone 16" | สูงมาก |

### 5. Match Types

| Match Type | Symbol | Example Keyword | Triggers |
|------------|--------|-----------------|----------|
| Broad Match | keyword | รองเท้าวิ่ง | รองเท้ากีฬา, รองเท้าออกกำลังกาย |
| Phrase Match | "keyword" | "รองเท้าวิ่ง" | รองเท้าวิ่งผู้หญิง, ซื้อรองเท้าวิ่ง |
| Exact Match | [keyword] | [รองเท้าวิ่ง] | รองเท้าวิ่ง (exact หรือ close variants) |
| Negative | -keyword | -ฟรี | ไม่แสดงเมื่อค้นหา "รองเท้าวิ่งฟรี" |

**Best Practice:**
- เริ่มจาก Exact Match → ขยายเป็น Phrase → Broad
- ใช้ Negative Keywords เสมอ
- Review Search Terms Report ทุกสัปดาห์

### 6. Quality Score

**Components (1-10 scale):**
- **Expected CTR** (40%): โอกาสที่คนจะคลิก
- **Ad Relevance** (30%): โฆษณาตรงกับ keyword
- **Landing Page Experience** (30%): ประสบการณ์หน้า landing

**Why It Matters:**
- Quality Score สูง = CPC ต่ำลง
- Quality Score สูง = Ad Rank สูงขึ้น
- Quality Score 7+ = เป้าหมายที่ดี

**Ad Rank Formula:**
```
Ad Rank = Max Bid × Quality Score
```

### 7. Bidding Strategies

| Strategy | Type | Best For |
|----------|------|----------|
| Manual CPC | Manual | เริ่มต้น, ควบคุมเต็มที่ |
| Enhanced CPC | Semi-Auto | เริ่มต้น + optimization |
| Target CPA | Auto | มี conversion data แล้ว |
| Target ROAS | Auto | E-commerce |
| Maximize Clicks | Auto | Traffic |
| Maximize Conversions | Auto | มี budget จำกัด |

**Recommendation:**
1. เริ่มจาก Manual CPC
2. เก็บ conversion data 15-30 วัน
3. เปลี่ยนเป็น Target CPA หลังได้ 30+ conversions

### 8. Ad Copy Best Practices

**Responsive Search Ads (RSA):**
- Headlines: 15 (แสดง 3)
- Descriptions: 4 (แสดง 2)

**Headline Tips:**
- ใส่ Keyword ใน Headline
- ใส่ Benefit/USP
- ใส่ CTA
- ใส่ตัวเลข (prices, discounts)

**Description Tips:**
- ขยายความจาก Headline
- ใส่ Features + Benefits
- Social proof ถ้ามี
- CTA ชัดเจน

### 9. Ad Extensions (Assets)

| Extension | Purpose | Impact |
|-----------|---------|--------|
| Sitelink | ลิงก์เพิ่มเติม | +10-20% CTR |
| Callout | USPs (ไม่คลิกได้) | +10% CTR |
| Structured Snippet | รายการ features | +5-10% CTR |
| Call | เบอร์โทร | +5% CTR (mobile) |
| Location | ที่อยู่ร้าน | +10% CTR (local) |
| Price | ราคาสินค้า | +10% CTR |
| Image | รูปสินค้า | +15% CTR |

### 10. Conversion Tracking

**Setup Steps:**
1. สร้าง Conversion Action ใน Google Ads
2. ติด Google Tag บนเว็บ
3. ตั้งค่า Conversion Goals
4. ทดสอบว่า fire ถูกต้อง

**Conversion Types:**
- Website purchases
- Lead form submissions
- Phone calls
- App downloads
- Store visits

### 11. Google Ads Editor

**Benefits:**
- ทำงาน Offline ได้
- Bulk edits (แก้ไขหลายอันพร้อมกัน)
- Copy/Paste campaigns
- Find & Replace
- Export/Import
- Review changes ก่อน upload

**Best Practices:**
- ใช้สำหรับ campaigns ใหญ่
- Draft mode → Review → Upload
- Backup ก่อนแก้ไขใหญ่

### 12. Key Metrics

| Metric | Formula | Good | Excellent |
|--------|---------|------|-----------|
| CTR | Clicks/Impressions | > 3% | > 5% |
| CPC | Cost/Clicks | ขึ้นอยู่กับ industry | - |
| CPA | Cost/Conversions | < Profit margin | < 50% margin |
| ROAS | Revenue/Ad Spend | > 3x | > 5x |
| Quality Score | 1-10 | > 5 | > 7 |
| Conversion Rate | Conversions/Clicks | > 2% | > 5% |
| Impression Share | Impressions/Eligible | > 50% | > 80% |

---

## Campaign Types Deep Dive

### Search Ads

**Best For:** High-intent keywords, Lead gen, Services

**Structure:**
```
Campaign: รองเท้าวิ่ง
    Ad Group 1: รองเท้าวิ่งผู้ชาย
        Keywords: [รองเท้าวิ่งผู้ชาย], "รองเท้าวิ่งผู้ชาย"
    Ad Group 2: รองเท้าวิ่งผู้หญิง
        Keywords: [รองเท้าวิ่งผู้หญิง], "รองเท้าวิ่งผู้หญิง"
```

### Display Ads

**Best For:** Brand awareness, Retargeting, Lookalike

**Targeting Options:**
- Audiences (In-market, Affinity)
- Topics
- Placements (specific websites)
- Keywords (contextual)
- Remarketing lists

**Ad Sizes:**
| Size | Name | Best For |
|------|------|----------|
| 300x250 | Medium Rectangle | Universal |
| 336x280 | Large Rectangle | In-content |
| 728x90 | Leaderboard | Header |
| 160x600 | Wide Skyscraper | Sidebar |
| 300x600 | Half Page | High impact |

### Shopping Ads

**Requirements:**
- Google Merchant Center account
- Product feed (XML/CSV)
- E-commerce website
- Pricing & availability data

**Feed Optimization:**
- Title: Include keywords + brand + attributes
- Description: Detailed product info
- Images: High quality, white background
- Price: Accurate, competitive

### YouTube Ads

**Ad Formats:**
| Format | Length | Skippable | Billing |
|--------|--------|-----------|---------|
| Skippable In-Stream | Any (skip after 5s) | Yes | CPV (30s or full) |
| Non-Skip In-Stream | 15s max | No | CPM |
| Bumper | 6s | No | CPM |
| Discovery | Thumbnail | N/A | CPC |
| Shorts | 60s max | Varies | CPV/CPM |

---

## Key Statistics

| Metric | Value |
|--------|-------|
| Google Daily Searches | 8.5 billion |
| Google Market Share | 92% |
| Average Search CTR (Position 1) | 27.6% |
| Average Display CTR | 0.46% |
| Average YouTube View Rate | 31.9% |
| Businesses using Google Ads | 80% of global businesses |

---

## Tools Mentioned

| Tool | Purpose | Cost |
|------|---------|------|
| Google Keyword Planner | Keyword research | Free |
| Google Ads Editor | Bulk management | Free |
| Google Tag Manager | Tag management | Free |
| Google Analytics | Website analytics | Free |
| SEMrush | Competitor research | $129/mo |
| SpyFu | Competitor keywords | $39/mo |

---

## Action Items

1. สร้าง Google Ads Account
2. ติดตั้ง Google Tag + Conversion Tracking
3. Keyword Research ด้วย Keyword Planner
4. สร้าง Campaign แรก (Search - Exact Match)
5. เพิ่ม Ad Extensions ครบ
6. Monitor Quality Score
7. Review Search Terms Weekly
8. Scale keywords ที่ได้ผล

---

## Production Notes

| Field | Value |
|-------|-------|
| Extracted | 2026-01-28 |
| Producer | จูล่ง |
| Source Files | 28 |
| Total Duration | 18:32:45 |
| QC Status | Pending |

---

> *Pink Castle Foundation Kit v1.0*
