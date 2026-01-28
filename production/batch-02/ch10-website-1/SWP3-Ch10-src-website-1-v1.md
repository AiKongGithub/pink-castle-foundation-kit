# Source Summary: Website Part 1

> **Format:** Source Summary
> **Source:** SWP3 Chapter 10
> **Topic:** Website Part 1 - พื้นฐานเว็บไซต์
> **Production ID:** SWP3-Ch10-001-SRC

---

## บทสรุปหลัก

### ทำไมต้องมีเว็บไซต์?

เว็บไซต์คือ "บ้าน" ของธุรกิจออนไลน์ เป็นทรัพย์สินที่คุณเป็นเจ้าของ ต่างจาก Social Media ที่อยู่บน platform คนอื่น

**สูตร:** Domain + Hosting + Platform = Website

---

## 3 องค์ประกอบหลักของเว็บไซต์

### 1. Domain Name (ชื่อโดเมน)

**คืออะไร:** ที่อยู่เว็บไซต์ เช่น yourname.com

**วิธีเลือก:**
- สั้น จำง่าย
- เกี่ยวข้องกับธุรกิจ
- ใช้ .com เป็นหลัก
- หลีกเลี่ยงตัวเลขและขีด

**ผู้ให้บริการ:**
| Provider | ราคา/ปี | ดีตรงไหน |
|----------|---------|----------|
| Namecheap | $9-15 | ถูก, Free WhoisGuard |
| GoDaddy | $12-20 | Brand ใหญ่ |
| Google Domains | $12 | เชื่อมต่อ Google |
| Cloudflare | $9 | ถูกที่สุด |

---

### 2. Web Hosting (โฮสติ้ง)

**คืออะไร:** พื้นที่เก็บไฟล์เว็บไซต์บน server

**ประเภท Hosting:**
| Type | ราคา/เดือน | เหมาะสำหรับ |
|------|------------|-------------|
| Shared | $3-10 | มือใหม่ |
| VPS | $20-80 | Traffic ปานกลาง |
| Dedicated | $100+ | Traffic สูงมาก |
| Managed WordPress | $15-50 | WordPress users |

**ผู้ให้บริการแนะนำ:**
| Provider | ราคา | จุดเด่น |
|----------|------|--------|
| Cloudways | $11/mo | Performance ดี |
| Hostinger | $3/mo | ถูก |
| SiteGround | $15/mo | Support ดี |
| Kinsta | $35/mo | Premium WordPress |

---

### 3. Platform (แพลตฟอร์ม)

**ตัวเลือก:**

| Platform | ราคา | Difficulty | Best For |
|----------|------|------------|----------|
| WordPress | Free (hosting cost) | กลาง | ทุกอย่าง |
| Wix | $16-45/mo | ง่าย | มือใหม่สุด |
| Squarespace | $16-49/mo | ง่าย | Portfolio |
| Shopify | $29-299/mo | ง่าย | E-commerce |
| Webflow | $12-36/mo | ยาก | Design-focused |

**แนะนำ:** WordPress เพราะ
- Free และ Open Source
- Plugin มากมาย
- Customize ได้เต็มที่
- Community ใหญ่

---

## WordPress Basics

### WordPress.org vs WordPress.com

| Aspect | WordPress.org | WordPress.com |
|--------|--------------|---------------|
| Hosting | ต้องหาเอง | รวมมาแล้ว |
| Cost | Hosting cost | Free-$45/mo |
| Freedom | 100% | จำกัด |
| Plugins | Unlimited | จำกัด |
| Monetize | ได้เลย | ต้องจ่าย |

**แนะนำ:** WordPress.org + Self-hosting

---

### Essential Plugins (10 ตัวที่ต้องมี)

| Plugin | Function | Free? |
|--------|----------|-------|
| Elementor | Page Builder | Yes* |
| Yoast SEO | SEO Optimization | Yes* |
| WPForms | Contact Forms | Yes* |
| UpdraftPlus | Backup | Yes* |
| Wordfence | Security | Yes* |
| WP Super Cache | Speed | Yes |
| Smush | Image Optimization | Yes* |
| Rank Math | SEO (Alternative) | Yes* |
| WooCommerce | E-commerce | Yes |
| MonsterInsights | Google Analytics | Yes* |

*มี Pro version

---

### Theme Selection

**Free Themes แนะนำ:**
- Astra (เร็ว, ยืดหยุ่น)
- GeneratePress (เบา)
- Kadence (Modern)
- OceanWP (Feature เยอะ)

**เลือก Theme ดูอะไร:**
1. **Speed** - ต้องเร็ว
2. **Responsive** - ใช้ได้ทุกหน้าจอ
3. **Customizable** - ปรับแต่งได้
4. **Support** - มีคนช่วยเหลือ
5. **Updates** - อัพเดทสม่ำเสมอ

---

## การตั้งค่าพื้นฐาน

### Step-by-Step Setup

```
1. ซื้อ Domain
   ↓
2. ซื้อ Hosting
   ↓
3. ติดตั้ง WordPress (1-Click Install)
   ↓
4. เลือก Theme
   ↓
5. ติดตั้ง Essential Plugins
   ↓
6. ตั้งค่า Settings พื้นฐาน
   ↓
7. สร้างหน้าสำคัญ
   ↓
8. ตั้งค่า SEO
```

### WordPress Settings ที่ต้องตั้ง

| Setting | Location | Action |
|---------|----------|--------|
| Site Title | Settings > General | ใส่ชื่อเว็บ |
| Tagline | Settings > General | คำอธิบายสั้น |
| Timezone | Settings > General | Asia/Bangkok |
| Permalinks | Settings > Permalinks | เลือก Post name |
| Comments | Settings > Discussion | ปิดถ้าไม่ต้องการ |
| Homepage | Settings > Reading | เลือก Static page |

---

## 5 หน้าที่ต้องมี

| หน้า | วัตถุประสงค์ | Priority |
|------|-------------|----------|
| Home | หน้าแรก, First impression | Critical |
| About | แนะนำตัว, สร้าง trust | High |
| Services/Products | สินค้า/บริการ | Critical |
| Contact | ติดต่อ | High |
| Blog | Content, SEO | Medium |

---

## Speed Optimization Basics

### ทำไม Speed สำคัญ?

- **Google Ranking:** Site เร็ว = rank สูงกว่า
- **Conversion:** 1 วินาทีช้า = ลด conversion 7%
- **Bounce Rate:** คนไม่รอเว็บช้า

### Quick Wins

| Action | Impact | Difficulty |
|--------|--------|------------|
| Use Caching Plugin | สูง | ง่าย |
| Optimize Images | สูง | ง่าย |
| Use CDN | สูง | กลาง |
| Minify CSS/JS | กลาง | ง่าย |
| Choose Fast Hosting | สูง | กลาง |
| Limit Plugins | กลาง | ง่าย |

---

## Security Basics

### Must-Do Security

| Action | Tool/Method |
|--------|-------------|
| Strong Password | Password Manager |
| Limit Login Attempts | Wordfence |
| Keep Updated | Auto-updates |
| Regular Backups | UpdraftPlus |
| SSL Certificate | Let's Encrypt (Free) |
| Hide Login URL | WPS Hide Login |

---

## Key Takeaways

1. **3 องค์ประกอบ:** Domain + Hosting + Platform
2. **WordPress.org** = Best choice for most
3. **10 Essential Plugins** ช่วยทำงานง่ายขึ้น
4. **Speed & Security** ต้องให้ความสำคัญ
5. **5 หน้าสำคัญ** ต้องมีครบ

---

## Action Items

- [ ] เลือกและซื้อ Domain
- [ ] เลือกและซื้อ Hosting
- [ ] ติดตั้ง WordPress
- [ ] เลือก Theme
- [ ] ติดตั้ง Essential Plugins
- [ ] ตั้งค่า Settings พื้นฐาน
- [ ] สร้าง 5 หน้าสำคัญ
- [ ] ตั้งค่า Security & Backup

---

## Production Notes

| Field | Value |
|-------|-------|
| Created | 2026-01-28 |
| Producer | จูล่ง |
| Chapter | 10 |
| Topic | Website Part 1 |
| QC Status | Pending |

---

> *Pink Castle Foundation Kit v1.0*
