# Flashcards: Google Ads

> **Format:** Flashcards (Q&A)
> **Source:** SWP3 Chapter 14
> **Total Cards:** 15
> **Production ID:** SWP3-Ch14-001-FLASH

---

## Flashcard Set

### Card 1 (Concept)
**Q:** Google Ads ต่างจาก Facebook Ads อย่างไร?

**A:** Google Ads เป็น **Intent-based Marketing**
- คนค้นหาสิ่งที่ต้องการอยู่แล้ว (Pull)
- Facebook Ads เป็น Interruption (Push)
- Search Ads มี conversion rate สูงกว่า

**Key:** "คนมาหาเรา ไม่ใช่เราไปหาคน"

---

### Card 2 (Structure)
**Q:** Google Ads มีโครงสร้างกี่ระดับ อะไรบ้าง?

**A:** 4 ระดับ:
1. **Account** - บัญชี, Billing
2. **Campaign** - Budget, Bidding, Location, Schedule
3. **Ad Group** - Keywords + Targeting + Ads
4. **Ads + Keywords** - ชิ้นงาน + คำค้นหา

---

### Card 3 (Match Types)
**Q:** Keyword Match Types มีกี่แบบ อะไรบ้าง?

**A:** 4 แบบ:
| Type | Symbol | Example |
|------|--------|---------|
| **Broad** | keyword | รองเท้าวิ่ง |
| **Phrase** | "keyword" | "รองเท้าวิ่ง" |
| **Exact** | [keyword] | [รองเท้าวิ่ง] |
| **Negative** | -keyword | -ฟรี |

**แนะนำ:** เริ่มจาก Exact Match

---

### Card 4 (Match Types Detail)
**Q:** Exact Match [รองเท้าวิ่ง] จะ trigger เมื่อค้นหาอะไรบ้าง?

**A:**
- "รองเท้าวิ่ง" (exact)
- "รองเท้า วิ่ง" (close variant - spacing)
- "รองเท้าวิ่ง ราคา" (close variant - minor addition)

**ไม่ trigger:** "รองเท้ากีฬา", "รองเท้าออกกำลังกาย"

---

### Card 5 (Quality Score)
**Q:** Quality Score ประกอบด้วยอะไรบ้าง?

**A:** 3 องค์ประกอบ (คะแนน 1-10):
1. **Expected CTR** (40%) - โอกาสที่คนจะคลิก
2. **Ad Relevance** (30%) - โฆษณาตรงกับ keyword
3. **Landing Page Experience** (30%) - หน้าเว็บดี, เร็ว, ตรงกับโฆษณา

**เป้าหมาย:** Quality Score 7+

---

### Card 6 (Formula)
**Q:** Ad Rank คำนวณอย่างไร?

**A:**
```
Ad Rank = Max Bid × Quality Score
```

**ตัวอย่าง:**
- คู่แข่ง: Bid $4 × QS 6 = 24
- เรา: Bid $3 × QS 10 = 30

**เราชนะ** แม้ bid ต่ำกว่า!

---

### Card 7 (Bidding)
**Q:** Bidding Strategies หลักๆ มีอะไรบ้าง?

**A:**
**Manual:**
- **Manual CPC** - กำหนดเอง (เริ่มต้น)
- **Enhanced CPC** - Semi-automated

**Automated:**
- **Target CPA** - กำหนด cost per acquisition
- **Target ROAS** - กำหนด return on ad spend
- **Maximize Conversions** - หา conversions มากสุด

**Path:** Manual CPC → Enhanced → Target CPA

---

### Card 8 (CTR Target)
**Q:** CTR (Click-Through Rate) ที่ดีสำหรับ Search Ads ควรเป็นเท่าไหร่?

**A:**
- **Good:** > 3%
- **Excellent:** > 5%
- **Average industry:** ~3.17%

ถ้า CTR ต่ำ:
- Ad copy ไม่ดึงดูด
- Keywords ไม่ relevant
- Extensions ไม่ครบ

---

### Card 9 (Extensions)
**Q:** Ad Extensions (Assets) ที่สำคัญมีอะไรบ้าง?

**A:**
| Extension | Purpose | CTR Impact |
|-----------|---------|------------|
| **Sitelink** | ลิงก์เพิ่มเติม | +10-20% |
| **Callout** | USPs | +10% |
| **Structured Snippet** | Features | +5-10% |
| **Call** | เบอร์โทร | +5% |
| **Location** | ที่อยู่ | +10% |

**สำคัญ:** ใส่ Extensions ครบทุกอัน!

---

### Card 10 (RSA)
**Q:** Responsive Search Ads (RSA) ใส่ได้กี่ Headlines และ Descriptions?

**A:**
- **Headlines:** สูงสุด 15 (แสดง 3)
- **Descriptions:** สูงสุด 4 (แสดง 2)

**Tips:**
- ใส่ Keyword ใน Headline
- ใส่ Benefit/USP
- ใส่ CTA
- ใส่ตัวเลข (ราคา, ส่วนลด)

---

### Card 11 (Campaign Types)
**Q:** Google Ads Campaign Types หลักๆ มีอะไรบ้าง?

**A:**
| Type | Best For |
|------|----------|
| **Search Ads** | High-intent, Lead gen |
| **Display Ads** | Awareness, Retargeting |
| **Shopping Ads** | E-commerce |
| **YouTube Ads** | Branding, Video |
| **Performance Max** | Automated, All channels |

**มือใหม่:** เริ่มจาก Search Ads

---

### Card 12 (Conversion Tracking)
**Q:** ทำไมต้องติด Conversion Tracking ก่อนยิงโฆษณา?

**A:**
1. **วัดผล** - รู้ว่าอะไรได้ผล
2. **Optimize** - Google ปรับให้หา converters
3. **Automated Bidding** - ต้องมี data
4. **ROAS** - คำนวณ return on investment

**ขั้นตอน:**
1. สร้าง Conversion Action
2. ติด Google Tag
3. ตั้ง Conversion Goals
4. ทดสอบด้วย Tag Assistant

---

### Card 13 (Negative Keywords)
**Q:** Negative Keywords คืออะไร และทำไมสำคัญ?

**A:** Keywords ที่ **ไม่ต้องการ** ให้โฆษณาแสดง

**ตัวอย่าง:** -ฟรี, -DIY, -วิธี

**ทำไมสำคัญ:**
- ประหยัดงบ
- เพิ่ม CTR (clicks ที่ relevant)
- เพิ่ม Quality Score

**Process:** Review Search Terms Report ทุกสัปดาห์

---

### Card 14 (Keyword Intent)
**Q:** Keyword Intent มีกี่ระดับ ควรเน้นระดับไหน?

**A:**
| Intent | Example | Conversion |
|--------|---------|------------|
| **Informational** | วิธีลดน้ำหนัก | ต่ำ |
| **Navigational** | Nike official | กลาง |
| **Commercial** | รีวิว iPhone | สูง |
| **Transactional** | ซื้อ iPhone | สูงมาก |

**เน้น:** Commercial + Transactional

---

### Card 15 (Process)
**Q:** ขั้นตอนเริ่มต้น Google Ads ควรทำอะไรบ้าง?

**A:**
1. **Keyword Research** - Keyword Planner
2. **ติด Conversion Tracking** - ก่อนยิง!
3. **สร้าง Campaign** - Search, Manual CPC
4. **ใช้ Exact Match** - ควบคุมได้
5. **เพิ่ม Negative Keywords** - กรอง
6. **ใส่ Extensions ครบ** - เพิ่ม CTR
7. **Monitor Quality Score** - เป้า 7+
8. **Review Search Terms** - ทุกสัปดาห์

---

## Export Format (Anki)

```
Google Ads vs Facebook Ads?	Intent-based (คนมาหาเรา) vs Interruption
Campaign Structure?	Account > Campaign > Ad Group > Ads + Keywords
Match Types?	Broad, "Phrase", [Exact], -Negative
Quality Score Components?	CTR (40%), Ad Relevance (30%), Landing Page (30%)
Ad Rank Formula?	Max Bid × Quality Score
CTR Target (Search)?	> 3% (Good), > 5% (Excellent)
Quality Score Target?	7+
เริ่มต้น Bidding?	Manual CPC → Enhanced → Target CPA
```

---

## Production Notes

| Field | Value |
|-------|-------|
| Created | 2026-01-28 |
| Producer | จูล่ง |
| Total Cards | 15 |
| Card Types | Concept (1), Structure (1), Match Types (2), Quality Score (1), Formula (1), Bidding (1), Metrics (1), Extensions (1), RSA (1), Campaign Types (1), Tracking (1), Negative KW (1), Intent (1), Process (1) |
| QC Status | Pending |

---

> *Pink Castle Foundation Kit v1.0*
