# วิธีปรับแต่ง Pop up form — CLONE-008
> **Format:** Slide Outline (12 Slides)
> **Source:** SWP3 Ch20 Cloning Sale Funnel Kartra ตอนที่ 8
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:14:26

---

## SLIDE 1: หน้าปก (Title Slide)
─────────────────

```
┌─────────────────────────────────┐
│                                 │
│   วิธีปรับแต่ง Pop up form     │
│   (Pop-up Form Customization)  │
│                                 │
│   SWP3 บทที่ 20:               │
│   Cloning Sale Funnel Kartra   │
│   ตอนที่ 8                      │
│                                 │
│   PinkCastle Academy           │
│   วันที่: 18 กุมภาพันธ์ 2569    │
│                                 │
└─────────────────────────────────┘
```

---

## SLIDE 2: สิ่งที่จะได้เรียนรู้วันนี้ (Learning Objectives)
─────────────────

- เข้าใจว่า Pop-up Form คืออะไร ทำไมถึงมี Conversion Rate สูง
- รู้จัก 4 ประเภทของ Pop-up และวิธีเลือกให้เหมาะสม
- ออกแบบองค์ประกอบ Pop-up ที่ดี (Headline, CTA, ฟิลด์)
- ปรับแต่ง Pop-up ใน Kartra Page Editor
- ตั้ง Timing, Trigger และ Design ที่เหมาะสม
- เชื่อมกับ Automation และทดสอบก่อน Publish

---

## SLIDE 3: Pop-up Form คืออะไร? (What is Pop-up Form?)
─────────────────

```
┌──────────────────────────────────┐
│  ┌────────────────────────────┐  │
│  │   หน้าเว็บปกติ (Page)      │  │
│  │                            │  │
│  │   ┌──────────────────┐     │  │
│  │   │  POP-UP FORM     │     │  │
│  │   │  ┌──────────┐    │     │  │
│  │   │  │ Name     │    │     │  │
│  │   │  │ Email    │    │     │  │
│  │   │  │ [CTA]    │    │     │  │
│  │   │  └──────────┘    │     │  │
│  │   └──────────────────┘     │  │
│  │                            │  │
│  └────────────────────────────┘  │
└──────────────────────────────────┘
```

- ฟอร์มที่ปรากฏซ้อนบนหน้าเว็บ เก็บข้อมูลลูกค้า
- Conversion Rate สูงกว่าฟอร์มปกติ **2-3 เท่า**
- ดึงความสนใจ สร้าง **Micro-commitment**
- ผู้เข้าชมต้องตัดสินใจ: กรอก หรือ ปิด

---

## SLIDE 4: 4 ประเภทของ Pop-up (Types of Pop-up)
─────────────────

```
┌──────────────┐  ┌──────────────┐
│ Exit Intent  │  │ Time Delay   │
│              │  │              │
│ เมาส์ → ปิด  │  │ 5-15 วินาที  │
│ Last-chance  │  │ สนใจเนื้อหา  │
│ Desktop only │  │ ทุกอุปกรณ์    │
└──────────────┘  └──────────────┘

┌──────────────┐  ┌──────────────┐
│ Scroll       │  │ Click        │
│ Trigger      │  │ Trigger      │
│              │  │              │
│ เลื่อน 50-70%│  │ คลิกปุ่ม     │
│ อ่านลึก      │  │ สนใจจริง     │
│ ทุกอุปกรณ์    │  │ CR สูงสุด    │
└──────────────┘  └──────────────┘
```

---

## SLIDE 5: องค์ประกอบ Pop-up ที่ดี (Good Pop-up Anatomy)
─────────────────

```
┌─────────────────────────────┐
│  [X] ปุ่มปิดชัดเจน          │
│                             │
│  รับ E-book ฟรี!            │  ← Headline ชัด
│  50 เทคนิคเพิ่มยอดขาย       │  ← Offer คุ้มค่า
│                             │
│  ┌────────────────────┐     │
│  │ ชื่อ                │     │  ← ฟิลด์น้อย
│  └────────────────────┘     │
│  ┌────────────────────┐     │
│  │ อีเมล              │     │  ← แค่ 2 ฟิลด์
│  └────────────────────┘     │
│                             │
│  ┌────────────────────┐     │
│  │  รับเลยฟรี!        │     │  ← CTA โดดเด่น
│  └────────────────────┘     │
│                             │
│  ไม่ต้องการ ขอบคุณ          │  ← ทางเลือกปิด
└─────────────────────────────┘
```

---

## SLIDE 6: ฟิลด์น้อย = Conversion สูง (Less Fields = More Conversions)
─────────────────

| จำนวนฟิลด์ | ตัวอย่าง | Conversion Rate (โดยประมาณ) |
|:---:|---|:---:|
| 1 ฟิลด์ | Email เท่านั้น | สูงมาก |
| 2 ฟิลด์ | Name + Email | สูง |
| 3 ฟิลด์ | Name + Email + Phone | กลาง |
| 4+ ฟิลด์ | Name + Email + Phone + Company | ต่ำ |

- ทุกฟิลด์ที่เพิ่ม → Conversion ลด **10-15%**
- **แนะนำ:** เก็บแค่ Name + Email
- ถ้าต้องการข้อมูลเพิ่ม → ขอทีหลังผ่าน Email Sequence

---

## SLIDE 7: วิธีแก้ไขใน Kartra (Kartra Page Editor)
─────────────────

- **ขั้นตอน:**
  1. เข้า Page Editor
  2. คลิกที่ Pop-up Element
  3. แก้ไข Headline → เปลี่ยนข้อความให้ตรง Offer ของเรา
  4. แก้ไขรูปภาพ → ใส่ Mockup ของ Lead Magnet
  5. แก้ไขฟิลด์ → ลดให้เหลือ Name + Email
  6. แก้ไข CTA → เปลี่ยนสีและข้อความ
  7. ตั้ง Form Settings → เชื่อม Email List + Automation

---

## SLIDE 8: Timing & Trigger (จังหวะเวลาที่เหมาะสม)
─────────────────

| ประเภท | ค่าแนะนำ | เหตุผล |
|--------|----------|--------|
| Time Delay | 5-15 วินาที | ไม่เร็วเกินจนรบกวน |
| Scroll Trigger | 50-70% ของหน้า | ผู้เข้าชมสนใจแล้ว |
| Exit Intent | อัตโนมัติ | จับจังหวะก่อนออก |
| Click Trigger | ทันทีเมื่อคลิก | ผู้เข้าชมเลือกเอง |

- **Frequency:** ตั้ง "Once per session" เป็นค่าเริ่มต้น
- Pop-up ที่เด้งซ้ำทุกหน้า = **ทำลาย User Experience**
- Exit Intent **ใช้ไม่ได้บนมือถือ** → ต้องมี Fallback

---

## SLIDE 9: Design Pop-up (การออกแบบ)
─────────────────

```
┌──────────────────────────────┐
│        Design Elements       │
├──────────────────────────────┤
│  ขนาด      │ 60-70% หน้าจอ  │
│  ตำแหน่ง    │ กลาง/มุมล่าง   │
│  Animation  │ Fade-in/Slide  │
│  Overlay    │ สีดำ 50% โปร่ง  │
│  สีพื้นหลัง  │ ตรงกับแบรนด์   │
│  ปุ่มปิด    │ มองเห็นชัด [X] │
└──────────────────────────────┘
```

- ไม่ควรใหญ่เกินจนบังทั้งหน้า (ลูกค้ารู้สึกถูกบังคับ)
- Fade-in/Slide-up ดูนุ่มนวลกว่าเด้งทันที
- Overlay ช่วยให้ **โฟกัส** ที่ Pop-up

---

## SLIDE 10: เชื่อมกับ Automation (Post-Submit Flow)
─────────────────

```
  ลูกค้ากรอกฟอร์ม
        │
        ▼
  ┌─────────────┐
  │ Email List  │ ← เพิ่มชื่อเข้าลิสต์
  └──────┬──────┘
         │
         ▼
  ┌─────────────┐
  │ Email       │ ← ส่ง Welcome Sequence
  │ Sequence    │
  └──────┬──────┘
         │
         ▼
  ┌─────────────┐
  │ Tag         │ ← ติด Tag แบ่งกลุ่ม
  └──────┬──────┘
         │
         ▼
  ┌─────────────┐
  │ Thank You   │ ← Redirect ไปหน้าขอบคุณ
  │ Page        │
  └─────────────┘
```

---

## SLIDE 11: Testing Checklist (ทดสอบก่อน Publish)
─────────────────

- **Checklist 4 จุด:**
  1. Pop-up แสดง **ถูกเวลา** ตามที่ตั้งไว้
  2. ฟอร์ม **Submit ได้จริง** ข้อมูลเข้า Email List
  3. **Redirect** ไปถูกหน้าหลัง Submit
  4. **ไม่รบกวน** ลูกค้ามากเกินไป

- **A/B Test:**
  - ลองเปลี่ยน Headline → วัด Conversion Rate
  - ลองเปลี่ยนเวลาแสดง → วัด Engagement
  - ลองเปลี่ยนสี CTA → วัด Click-through Rate

---

## SLIDE 12: สรุปและ Key Takeaway (Summary)
─────────────────

- **4 ประเภท Pop-up:** Exit Intent / Time Delay / Scroll / Click
- **5 องค์ประกอบ:** Headline ชัด + Offer คุ้ม + ฟิลด์น้อย + CTA เด่น + ปุ่มปิดชัด
- **Timing:** 5-15 วินาที / 50-70% Scroll / Once per session
- **Design:** 60-70% หน้าจอ / Fade-in / Overlay โปร่งแสง
- **Automation:** Email List → Sequence → Tag → Thank You Page
- **Testing:** ทดสอบ 4 จุด + A/B Test
- **Key Takeaway:** Pop-up ที่ดีให้คุณค่า ไม่ใช่รบกวน
- ตอนหน้า: วิธีปรับแต่งหน้า Thank You Page

---

> ทบทวนต่อ: **CLONE-009** — ปรับแต่งหน้า Thank You Page
> Series: SWP3 Ch20 Cloning Sale Funnel Kartra
> PinkCastle Academy © 2026

*จำนวน Slides ทั้งหมด: 12 สไลด์*
