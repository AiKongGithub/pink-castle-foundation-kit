# Report: Facebook Ads

> **Format:** Detailed Report
> **Source:** SWP3 Chapter 13
> **Pages:** 14
> **Production ID:** SWP3-Ch13-001-RPT

---

## Executive Summary

Facebook Ads เป็น Paid Advertising Platform ที่ใหญ่ที่สุดในโลก มีผู้ใช้ 3 พันล้านคนต่อเดือน รายงานนี้ครอบคลุม Campaign Structure, Targeting, Creative, Pixel, Budgeting และ Optimization

---

## 1. Facebook Ads Overview

### 1.1 Why Facebook Ads?

| Advantage | Description |
|-----------|-------------|
| Reach | 3 พันล้านผู้ใช้ต่อเดือน |
| Targeting | ละเอียดที่สุดในโลก |
| Formats | Image, Video, Carousel, Collection |
| Entry Cost | เริ่มต้นได้ทุก Budget |
| Data | Pixel tracking ครบถ้วน |

### 1.2 Platform Statistics

| Metric | Value |
|--------|-------|
| Monthly Active Users | 3 billion |
| Daily Active Users | 2 billion |
| Average CTR | 0.9% |
| Average CPC | $0.97 |
| Mobile Users | 98%+ |
| Video Views Daily | 8 billion |

---

## 2. Campaign Structure

### 2.1 Three Levels

```
Campaign (วัตถุประสงค์)
    │
    └── Ad Set (กลุ่มเป้าหมาย + งบ)
            │
            └── Ad (ชิ้นงานโฆษณา)
```

### 2.2 Campaign Level

**What to Set:**
- Campaign Objective
- Campaign Budget Optimization (optional)
- A/B Testing (optional)

### 2.3 Ad Set Level

**What to Set:**
- Audience (targeting)
- Budget & Schedule
- Placements
- Optimization & Delivery

### 2.4 Ad Level

**What to Set:**
- Format (Image/Video/Carousel)
- Creative (Media)
- Copy (Primary text, Headline)
- CTA Button
- Destination URL

---

## 3. Campaign Objectives

### 3.1 Awareness

| Objective | Best For | Billing |
|-----------|----------|---------|
| Brand Awareness | ให้คนจำ Brand ได้ | CPM |
| Reach | เข้าถึงคนมากที่สุด | CPM |

### 3.2 Consideration

| Objective | Best For | Billing |
|-----------|----------|---------|
| Traffic | คนเข้าเว็บ | CPC/CPM |
| Engagement | Like, Comment, Share | CPE |
| Video Views | ดูวิดีโอ | CPV |
| Lead Generation | เก็บ Lead ใน Facebook | CPL |
| Messages | ส่งข้อความ | CPM |

### 3.3 Conversion

| Objective | Best For | Billing |
|-----------|----------|---------|
| Conversions | ซื้อ/สมัคร | CPA |
| Catalog Sales | E-commerce | CPA |
| Store Traffic | ร้านค้าจริง | CPM |

### 3.4 Choosing the Right Objective

**For Beginners (No Pixel Data):**
1. Start with Traffic → Collect data
2. Switch to Conversions → After 50+ conversions

**For E-commerce:**
1. Catalog Sales → Product ads
2. Conversions → Single product focus

**For Lead Generation:**
1. Lead Gen → Facebook form
2. Conversions → Landing page form

---

## 4. Targeting

### 4.1 Core Audiences

**Demographics:**
- Age (13-65+)
- Gender
- Location (Country, City, Radius)
- Language
- Education
- Job Title
- Relationship Status

**Interests:**
- Pages liked
- Activities
- Hobbies
- Shopping behavior
- Competitor brands

**Behaviors:**
- Purchase behavior
- Device usage
- Travel patterns
- Digital activities

### 4.2 Custom Audiences

| Source | Description | Retention |
|--------|-------------|-----------|
| Website | คนที่เข้าเว็บ (Pixel) | 1-180 days |
| Customer List | อัพโหลด Email/Phone | Until removed |
| App Activity | คนที่ใช้ App | 1-180 days |
| Engagement | คนที่ interact | 1-365 days |
| Video | คนที่ดูวิดีโอ | 1-365 days |
| Lead Form | คนที่กรอกฟอร์ม | 1-90 days |

### 4.3 Lookalike Audiences

**How It Works:**
1. อัพโหลด Source Audience (เช่น ลูกค้าที่ซื้อ)
2. เลือก % Similarity (1-10%)
3. Facebook หาคนที่คล้ายกัน

**Best Practices:**
- Source อย่างน้อย 100 คน (1,000+ ดีกว่า)
- เริ่มจาก 1% (Quality > Quantity)
- ใช้ Purchasers เป็น Source ดีที่สุด

### 4.4 Targeting Strategy by Funnel

| Stage | Audience | Budget % |
|-------|----------|----------|
| Cold | Interests, Lookalike 1-3% | 60-70% |
| Warm | Website visitors, Engagers | 20-30% |
| Hot | Add to cart, Past purchasers | 10-20% |

---

## 5. Facebook Pixel

### 5.1 What is Pixel?

JavaScript code ที่ติดบนเว็บไซต์ เพื่อ track พฤติกรรมผู้ใช้

### 5.2 Standard Events

| Event | Trigger | Use Case |
|-------|---------|----------|
| PageView | ทุกหน้า | Basic tracking |
| ViewContent | หน้าสินค้า | Product interest |
| AddToCart | ใส่ตะกร้า | Purchase intent |
| InitiateCheckout | เริ่ม checkout | High intent |
| Purchase | ซื้อสำเร็จ | Conversion |
| Lead | กรอกฟอร์ม | Lead gen |
| CompleteRegistration | สมัครสมาชิก | Sign up |

### 5.3 Benefits of Pixel

1. **Track Conversions** - วัด ROI ได้
2. **Build Custom Audiences** - Retarget คนที่สนใจ
3. **Create Lookalikes** - หาคนคล้ายลูกค้า
4. **Optimize Delivery** - Facebook หาคนที่จะ convert

### 5.4 Pixel Installation

**Option 1:** Manual Code
```html
<!-- Facebook Pixel Code -->
<script>
!function(f,b,e,v,n,t,s)...
</script>
```

**Option 2:** Google Tag Manager

**Option 3:** Platform Integration (Shopify, WordPress)

---

## 6. Ad Creative

### 6.1 Ad Formats

| Format | Specs | Best For |
|--------|-------|----------|
| Image | 1080x1080 (1:1) or 1200x628 (1.91:1) | Simple message |
| Video | < 15 sec, 4:5 or 1:1 | Engagement |
| Carousel | 2-10 cards, 1080x1080 | Multiple products |
| Collection | Cover + 4 products | E-commerce |
| Stories | 1080x1920 (9:16) | Mobile |
| Reels | 1080x1920 (9:16) | Young audience |

### 6.2 Creative Best Practices

**Visual:**
- First 3 seconds ต้องหยุดนิ้ว
- ใช้สีสดใส, contrast สูง
- ใบหน้าคน = engagement สูงกว่า
- Add captions (85% ดูแบบไม่มีเสียง)

**Copy:**
- Primary Text: 125 characters (visible without "See more")
- Headline: 40 characters
- Description: 30 characters

**CTA Buttons:**
- Shop Now (E-commerce)
- Learn More (Content)
- Sign Up (Lead gen)
- Download (Apps)
- Contact Us (Services)

### 6.3 Ad Copy Formulas

**PAS Formula:**
```
Problem: เหนื่อยกับการทำงานหนักแต่ไม่มีเวลาดูแลตัวเอง?
Agitate: ยิ่งไม่ดูแลสุขภาพ ยิ่งเหนื่อยง่าย ประสิทธิภาพลด
Solution: [Product] ช่วยให้คุณ [Benefit] ใน [Timeframe]
```

**AIDA Formula:**
```
Attention: 🔥 ลดน้ำหนัก 5 กก. ใน 30 วัน!
Interest: โดยไม่ต้องอดอาหาร ไม่ต้องออกกำลังกายหนัก
Desire: คนกว่า 10,000+ คนพิสูจน์แล้วว่าได้ผลจริง
Action: คลิกเรียนรู้เพิ่มเติมเลย!
```

---

## 7. Budget & Bidding

### 7.1 Budget Types

| Type | Description | Best For |
|------|-------------|----------|
| Daily Budget | ใช้ทุกวัน | Testing |
| Lifetime Budget | ใช้ตลอด campaign | Limited time offers |
| CBO | Budget ที่ Campaign level | Scaling |

### 7.2 Starting Budget

- **Testing:** 200-500 บาท/วัน
- **Scaling:** 10-20% increase ทุก 3-5 วัน
- **Rule:** อย่าเกิน 2x งบต่อวัน

### 7.3 Bidding Strategies

| Strategy | Description | Best For |
|----------|-------------|----------|
| Lowest Cost | FB หาราคาถูกที่สุด | เริ่มต้น |
| Cost Cap | กำหนด CPA สูงสุด | ควบคุม cost |
| Bid Cap | กำหนด bid สูงสุด | แข่งราคา |
| Minimum ROAS | กำหนด ROAS ขั้นต่ำ | E-commerce |

---

## 8. Testing Framework

### 8.1 What to Test (Priority Order)

1. **Audiences** - Test ก่อนเสมอ
2. **Creatives** - Image vs Video, Different hooks
3. **Copy** - Headlines, Body text
4. **Placements** - Feed vs Stories vs Reels
5. **Bid strategies** - After scaling

### 8.2 How to Test

1. Test 1 variable ต่อครั้ง
2. Budget เท่าๆ กัน (อย่างน้อย 200 บาท/วัน/ad set)
3. รันอย่างน้อย 3-7 วัน
4. ดูผลแบบ statistical significance
5. Pick winner และ iterate

### 8.3 Learning Phase

- Facebook ใช้เวลา 3-7 วัน optimize
- ต้องได้ ~50 conversions ต่อสัปดาห์
- **อย่าแก้ไข** ระหว่าง learning phase
- ถ้าแก้ = reset learning

---

## 9. Key Metrics

### 9.1 Performance Metrics

| Metric | Formula | Good | Excellent |
|--------|---------|------|-----------|
| CPM | Cost/1000 impressions | < $15 | < $10 |
| CPC | Cost/Clicks | < $1 | < $0.50 |
| CTR | Clicks/Impressions | > 1% | > 2% |
| CPA | Cost/Conversions | < Product margin | < 50% margin |
| ROAS | Revenue/Ad Spend | > 2x | > 4x |
| Frequency | Impressions/Reach | < 3 | < 2 |

### 9.2 Diagnostic Metrics

| Problem | Indicator | Solution |
|---------|-----------|----------|
| Low CTR | < 1% | Creative ไม่ดึงดูด |
| High CPC | Expensive clicks | Audience แคบ/แข่งเยอะ |
| High Frequency | > 3 | Audience เล็กเกินไป |
| Low Conversion Rate | Good CTR, Low conversions | Landing page problem |

---

## 10. Common Mistakes

| Mistake | Why It's Bad | Solution |
|---------|-------------|----------|
| ไม่ติด Pixel | เสีย data | ติดก่อนยิงโฆษณา |
| Audience กว้างเกินไป | เสียเงินฟรี | เริ่มจากแคบก่อน |
| ไม่ทดสอบ | ไม่รู้อะไรได้ผล | A/B Test ตลอด |
| ปิดเร็วเกินไป | ไม่ให้เวลา optimize | รอ 3-7 วัน |
| Frequency สูง | Ad fatigue | เปลี่ยน creative |
| Landing page ไม่ดี | โฆษณาดีแต่ไม่ convert | Fix landing page ก่อน |

---

## 11. Scaling Strategies

### 11.1 Vertical Scaling

เพิ่มงบ Ad Set ที่ได้ผลดี
- เพิ่ม 10-20% ทุก 3-5 วัน
- อย่าเพิ่มเกิน 2x ต่อวัน

### 11.2 Horizontal Scaling

ขยาย Audience หรือเพิ่ม Ad Sets
- Test Lookalike 2%, 3%
- Test ประเทศใหม่
- Test Interests ใหม่

### 11.3 Creative Scaling

สร้าง Creative ใหม่จาก Winners
- เปลี่ยน hook
- เปลี่ยนรูป/วิดีโอ
- เปลี่ยน angle

---

## Key Takeaways

1. **ติด Pixel ก่อน** - สำคัญที่สุด
2. **Structure matters** - Campaign > Ad Set > Ad
3. **Targeting is king** - Custom + Lookalike audiences
4. **Test everything** - Audience first, then Creative
5. **Respect Learning Phase** - อย่าแก้ไขเร็วเกินไป
6. **Monitor metrics** - CTR, CPC, CPA, Frequency
7. **Scale winners** - Cut losers fast

---

## Production Notes

| Field | Value |
|-------|-------|
| Created | 2026-01-28 |
| Producer | จูล่ง |
| Sections | 11 |
| Tables | 25+ |
| QC Status | Pending |

---

> *Pink Castle Foundation Kit v1.0*
