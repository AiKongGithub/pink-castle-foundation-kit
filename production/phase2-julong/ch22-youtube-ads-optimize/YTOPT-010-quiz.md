# Google กับ Kartra ทำงานร่วมกัน — YTOPT-010 Quiz
> **Format:** Quiz (10 Questions)
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 10
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:06:52

---

## แบบทดสอบ (10 ข้อ)

### Multiple Choice (6 ข้อ)

**ข้อ 1.** ทำไมต้องเชื่อม Google Ads กับ Kartra?
- A) เพื่อให้ Kartra Landing Page โหลดเร็วขึ้น
- B) เพื่อวัด Conversion จริง ว่าคนคลิกโฆษณาแล้วกรอกฟอร์มหรือซื้อจริงหรือไม่
- C) เพื่อให้โฆษณาแสดงบน Kartra Dashboard
- D) เพื่อเพิ่มจำนวน Impressions ของโฆษณา

**ข้อ 2.** ใส่ Google Tag ใน Kartra ได้ที่ไหน?
- A) Kartra Dashboard → General Settings → SEO
- B) Kartra Page → Page Settings → Tracking Code → Header
- C) Kartra Email → Automation → Tracking
- D) Kartra Form → Submit Actions → Tag

**ข้อ 3.** Google Tag ที่ต้องใส่ใน Kartra มีกี่ส่วน อะไรบ้าง?
- A) 1 ส่วน คือ Global Site Tag
- B) 2 ส่วน คือ Global Site Tag (ทุกหน้า) และ Event Snippet (Thank You Page)
- C) 3 ส่วน คือ Global Tag, Event Tag, Remarketing Tag
- D) 4 ส่วน คือ Base Tag, Event Tag, Pixel, Snippet

**ข้อ 4.** ข้อใดเป็นข้อดีของ Google Tag Manager เมื่อเทียบกับ Global Site Tag?
- A) ไม่ต้องมี Google Ads Account
- B) ทำให้โฆษณาราคาถูกลง
- C) จัดการหลาย Tag จากที่เดียว มี Version Control และ Preview Mode
- D) ไม่ต้องวางโค้ดใดๆ ลงใน Kartra เลย

**ข้อ 5.** เครื่องมือที่ใช้ตรวจสอบว่า Google Tag ทำงานถูกต้องบน Kartra คืออะไร?
- A) Google Analytics Dashboard
- B) Google Tag Assistant Chrome Extension
- C) Google Search Console
- D) Google PageSpeed Insights

**ข้อ 6.** ในขั้นตอน Conversion Tracking Flow จุดที่ Google Ads บันทึก Conversion คือขั้นตอนใด?
- A) เมื่อคนเห็นโฆษณา (Impression)
- B) เมื่อคนคลิกโฆษณา (Click)
- C) เมื่อคนเข้า Kartra Landing Page (Page View)
- D) เมื่อคนเข้าถึง Thank You Page หลังกรอกฟอร์ม/ซื้อสินค้า

---

### True or False (3 ข้อ)

**ข้อ 7.** Global Site Tag เหมาะกับมือใหม่ที่มี Tag 1-2 ตัว เพราะวางโค้ดตรงง่ายกว่า GTM
- True
- False

**ข้อ 8.** ถ้าลืมใส่ Event Snippet บน Kartra Thank You Page จะทำให้ Google Ads ไม่สามารถบันทึก Conversion ได้
- True
- False

**ข้อ 9.** Smart Bidding ของ Google สามารถทำงานได้ดีโดยไม่ต้องมี Conversion Data จาก Kartra
- True
- False

---

### Fill in the Blank (1 ข้อ)

**ข้อ 10.** ข้อดี 3 ประการหลักของการเชื่อม Google Ads กับ Kartra คือ ข้อมูล Conversion ________, ________ Campaign ได้ดีขึ้น และใช้ ________ ได้

---

## เฉลย (Answer Key)

| ข้อ | คำตอบ | คำอธิบาย |
|-----|-------|----------|
| 1 | **B) เพื่อวัด Conversion จริง** | การเชื่อม Google กับ Kartra ทำให้รู้ว่าคนที่คลิกโฆษณามานั้นกรอกฟอร์มหรือซื้อสินค้าจริงหรือไม่ ไม่ใช่แค่ดู Clicks |
| 2 | **B) Page Settings → Tracking Code → Header** | ใน Kartra ให้เข้า Page ที่ต้องการ คลิก Page Settings หาส่วน Tracking Code แล้ววาง Google Tag ในช่อง Header |
| 3 | **B) 2 ส่วน** | Global Site Tag วางทุกหน้าที่เกี่ยวข้อง เป็น Tag หลัก ส่วน Event Snippet วางเฉพาะ Thank You Page เพื่อบอก Google ว่าเกิด Conversion |
| 4 | **C) จัดการหลาย Tag จากที่เดียว** | GTM ช่วยจัดการ Tag หลายตัว (Google, Facebook, TikTok) จากที่เดียว มี Version Control ย้อนกลับได้ และ Preview Mode ตรวจก่อน Publish |
| 5 | **B) Google Tag Assistant** | เป็น Chrome Extension ฟรีที่ตรวจว่า Tag ติดตั้งถูกต้องและยิงข้อมูลกลับไปที่ Google Ads ได้จริง สีเขียว = ปกติ |
| 6 | **D) เมื่อคนเข้าถึง Thank You Page** | Conversion ถูกบันทึกเมื่อ Event Snippet บน Thank You Page ยิงข้อมูลกลับไปที่ Google Ads หลังจากผู้ใช้กรอกฟอร์มหรือซื้อสินค้าสำเร็จ |
| 7 | **True** | Global Site Tag เหมาะกับมือใหม่เพราะวางโค้ดตรงง่าย ไม่ต้องเรียนรู้เครื่องมือเพิ่ม แต่ถ้าใช้หลายแพลตฟอร์มควรใช้ GTM |
| 8 | **True** | Event Snippet บน Thank You Page คือตัวที่บอก Google Ads ว่าเกิด Conversion ถ้าไม่มี Tag นี้ Google จะไม่รู้ว่ามีคนกรอกฟอร์มหรือซื้อสินค้า |
| 9 | **False** | Smart Bidding ต้องมี Conversion Data เพียงพอจึงจะทำงานได้แม่นยำ ยิ่งมี Conversion Data จาก Kartra มาก Smart Bidding ยิ่ง Optimize ได้ดีขึ้น |
| 10 | **แม่นยำ** / **Optimize** / **Smart Bidding** | ข้อดี 3 ประการ คือ ข้อมูล Conversion แม่นยำ, Optimize Campaign ได้ดีขึ้น และใช้ Smart Bidding ได้ |

---

## เกณฑ์การให้คะแนน (Grading Rubric)

| ช่วงคะแนน | ระดับ | คำแนะนำ |
|-----------|-------|---------|
| 9-10 / 10 | ดีเยี่ยม | พร้อมไปเรียนเรื่องลงโฆษณา Google Ads ตอนที่ 2 |
| 7-8 / 10 | ดี | ทบทวนเรื่อง GTM vs Global Site Tag และ Conversion Flow เพิ่มเติม |
| 5-6 / 10 | ผ่าน | ควรอ่านเนื้อหาซ้ำและลองใส่ Google Tag ใน Kartra จริง |
| ต่ำกว่า 5 / 10 | ไม่ผ่าน | ควรเรียนบทนี้ใหม่ตั้งแต่ต้น |

---

> ทบทวนต่อ: **YTOPT-012** — ลงโฆษณา Google Ads ตอนที่ 2
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*Questions: 10 (6 MC + 3 T/F + 1 Fill-in) | Difficulty: Intermediate*
