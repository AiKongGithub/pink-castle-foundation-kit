# ทำความรู้จักระบบ Affiliate — TRIP-003
> **Format:** Slide Deck (14 สไลด์)
> **Source:** SWP3 Ch8 Trip Wire ตอนที่ 3
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

SLIDE 1: [Title Slide]
# ทำความรู้จักระบบ Affiliate
### เจาะลึกกลไก Tracking, คอมมิชชัน และแพลตฟอร์ม
**SWP3 บทที่ 8 — Trip Wire ตอนที่ 3**
PinkCastle Academy

---

SLIDE 2: [Agenda]
# สิ่งที่จะเรียนรู้ในวันนี้
1. ระบบ Tracking ทำงานอย่างไร
2. ประเภทของคอมมิชชัน (CPA, CPS, Recurring)
3. Affiliate Ecosystem — 4 ผู้เล่น
4. เปรียบเทียบแพลตฟอร์ม Affiliate
5. จริยธรรมและ Disclosure

---

SLIDE 3: [Tracking - Cookie]
# ระบบ Tracking: Cookie
> **เมื่อลูกค้าคลิกลิงก์ → ฝัง Cookie → จำว่ามาจากใคร**

- Cookie ฝังในเบราว์เซอร์ลูกค้า
- อายุ: 24 ชั่วโมง - 90 วัน (ตามแพลตฟอร์ม)
- จำข้อมูลแม้ปิดเบราว์เซอร์แล้วกลับมา
- ข้อจำกัด: ถูกบล็อกโดย Ad Blocker

---

SLIDE 4: [Tracking - Pixel & UTM]
# ระบบ Tracking: Pixel & UTM
### Pixel Tracking
- โค้ดเล็กๆ (1x1 pixel) ฝังในเว็บ
- ติดตามพฤติกรรมละเอียด
- Track ข้ามอุปกรณ์ได้

### UTM Parameters
- ส่วนต่อท้าย URL: `?utm_source=facebook&utm_medium=affiliate`
- ระบุแหล่งที่มาชัดเจน
- วิเคราะห์ใน Google Analytics

---

SLIDE 5: [Commission Types]
# ประเภทคอมมิชชัน 3 แบบ
| ประเภท | เงื่อนไข | อัตรา |
|--------|---------|------|
| **CPA** | จ่ายเมื่อทำ action | $1-$50/ครั้ง |
| **CPS** | จ่ายเมื่อขายได้ | 5-75% |
| **Recurring** | จ่ายทุกเดือน | 20-40%/เดือน |

> **Recurring = Passive Income ตัวจริง!**

---

SLIDE 6: [Recurring Deep Dive]
# Recurring Commission — ทำไมถึงน่าสนใจ?
### ตัวอย่าง:
- แนะนำ SaaS ราคา $50/เดือน
- คอมมิชชัน 30% = **$15/เดือน/ลูกค้า**
- 10 ลูกค้า = **$150/เดือน**
- 100 ลูกค้า = **$1,500/เดือน**

> ไม่ต้องขายเพิ่ม ได้ทุกเดือนตราบใดที่ลูกค้ายังสมัครอยู่!

---

SLIDE 7: [Ecosystem]
# Affiliate Ecosystem — 4 ผู้เล่น
```
Merchant (ผู้ขาย) ←→ Network (ตัวกลาง) ←→ Affiliate (เรา) ←→ Customer (ลูกค้า)
```

| ผู้เล่น | ได้ประโยชน์ |
|---------|-----------|
| Merchant | ลูกค้าใหม่ จ่ายเมื่อขายได้ |
| Network | ค่าบริการจากทั้งสองฝ่าย |
| Affiliate | คอมมิชชัน |
| Customer | สินค้าดี + รีวิวน่าเชื่อถือ |

> **Win-Win ทุกฝ่าย!**

---

SLIDE 8: [Platforms - Global]
# แพลตฟอร์ม Affiliate ระดับโลก
### ClickBank
- สินค้าดิจิทัล | คอมมิชชัน **50-75%**
- Cookie: 60 วัน
- เหมาะ: คอร์ส, Ebook, Software

### Amazon Associates
- สินค้าทุกประเภท | คอมมิชชัน **1-10%**
- Cookie: 24 ชั่วโมง
- เหมาะ: รีวิวสินค้ากายภาพ

---

SLIDE 9: [Platforms - Thai]
# แพลตฟอร์ม Affiliate ตลาดไทย
### Shopee Affiliate
- คอมมิชชัน **3-10%** | Cookie: 7 วัน
- จุดเด่น: คนไทยคุ้นเคย ซื้อง่าย

### Lazada Affiliate
- คอมมิชชัน **3-10%** | Cookie: 7 วัน
- จุดเด่น: ตลาดใหญ่ โปรโมชันบ่อย

> **คนไทยคุ้นเคยอยู่แล้ว → Conversion Rate สูง**

---

SLIDE 10: [Platform Comparison]
# เปรียบเทียบแพลตฟอร์ม
| แพลตฟอร์ม | คอมมิชชัน | Cookie | เหมาะกับ |
|-----------|----------|--------|---------|
| ClickBank | 50-75% | 60 วัน | สินค้าดิจิทัล |
| Amazon | 1-10% | 24 ชม. | สินค้าหลากหลาย |
| Shopee | 3-10% | 7 วัน | ตลาดไทย |
| Lazada | 3-10% | 7 วัน | ตลาดไทย |

---

SLIDE 11: [Ethics]
# จริยธรรม Affiliate
### 4 ข้อที่ต้องปฏิบัติ

1. **Disclosure** — เปิดเผยว่าเป็น Affiliate ทุกครั้ง
2. **ความซื่อสัตย์** — ไม่พูดเกินจริง รีวิวทั้งข้อดี-ข้อจำกัด
3. **คุณภาพสินค้า** — เลือกเฉพาะสินค้าที่เชื่อมั่นจริง
4. **ความโปร่งใส** — ไม่ใช้วิธีหลอกลวงหรือ cloaking

> ความน่าเชื่อถือ = ทรัพย์สินที่มีค่าที่สุดของ Affiliate

---

SLIDE 12: [Strategy]
# กลยุทธ์เลือกแพลตฟอร์ม
| กลุ่มเป้าหมาย | แพลตฟอร์มแนะนำ |
|-------------|--------------|
| คนไทยทั่วไป | Shopee + Lazada |
| ผู้สนใจดิจิทัล | ClickBank |
| สินค้าทั่วโลก | Amazon |
| SaaS/Tech | แพลตฟอร์ม SaaS โดยตรง |
| ผู้เริ่มต้น | Shopee + ClickBank |

---

SLIDE 13: [Action Steps]
# เริ่มต้นอย่างมืออาชีพ
1. **เลือกแพลตฟอร์ม** ให้ตรงกับกลุ่มเป้าหมาย
2. **ศึกษาโครงสร้างคอมมิชชัน** ของแต่ละแพลตฟอร์ม
3. **เน้น Recurring Commission** สำหรับ Passive Income
4. **สร้าง Content Evergreen** ที่ดึง Traffic ต่อเนื่อง
5. **ปฏิบัติตามจริยธรรม** Disclosure ทุกครั้ง

---

SLIDE 14: [Closing]
# สรุป
> **ระบบ Affiliate = Win-Win Ecosystem ที่ทุกฝ่ายได้ประโยชน์**

### จำไว้:
- Tracking: Cookie + Pixel + UTM
- คอมมิชชัน: CPA | CPS | **Recurring** (ดีที่สุด)
- 4 ผู้เล่น: Merchant, Network, Affiliate, Customer
- เลือกแพลตฟอร์มให้ตรงกับกลุ่มเป้าหมาย
- จริยธรรม = ทรัพย์สินมีค่าที่สุด

**ตอนหน้า: Software สร้าง Headline**

---

> **จำนวนสไลด์:** 14 | **เวลานำเสนอโดยประมาณ:** 20-25 นาที
