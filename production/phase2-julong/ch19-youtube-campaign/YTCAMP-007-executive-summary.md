# วิธีสร้าง Youtube Ads Campaign 2 — YTCAMP-007 Executive Summary
> **Format:** Executive Summary
> **Source:** SWP3 Ch19 Youtube Ads Campaign ตอนที่ 7
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:13:28

---

## สรุปภาพรวม

บทเรียนนี้เป็นภาคปฏิบัติส่วนที่ 2 ของการสร้าง Youtube Ads Campaign ต่อจาก YTCAMP-006 ที่ครอบคลุม 6 ขั้นตอนแรก ในตอนนี้จะลงลึกการตั้งค่า Ad Group ขั้นสูง การเลือก Bidding Strategy ให้เหมาะสม การซ้อน Targeting Layers เพื่อเข้าถึงกลุ่มเป้าหมายแม่นยำ การสร้าง Ad Creative และ CTA Overlay การทำ A/B Testing ด้วย Multiple Ad Groups และสุดท้ายคือการ Review และ Launch Campaign จริง

---

## ประเด็นสำคัญ (Key Takeaways)

| # | ประเด็น | รายละเอียด |
|---|---------|-----------|
| 1 | Ad Group Demographics | กำหนด Gender, Age, Parental Status, Household Income ได้ — ถ้าไม่แน่ใจให้ปล่อยกว้างแล้วค่อย Narrow จากข้อมูลจริง |
| 2 | Placements Targeting | เลือก Channel, วิดีโอ หรือเว็บไซต์เฉพาะที่ต้องการให้โฆษณาแสดง |
| 3 | Targeting Layers ซ้อนได้ | ซ้อน Audience + Topic + Keyword ได้ 2-3 ชั้น เพื่อความแม่นยำ แต่อย่าซ้อนมากเกินจน Reach แคบ |
| 4 | Ad Creative ต้องอยู่บน Youtube | วิดีโอโฆษณาต้อง Upload ลง Youtube ก่อน แล้ววาง URL ใน Google Ads |
| 5 | CTA Overlay สำคัญมาก | ข้อความ CTA ต้องชัดเจน ตรงเป้าหมาย — "สมัครฟรี" สำหรับ Conversion, "เรียนรู้เพิ่มเติม" สำหรับ Awareness |
| 6 | A/B Testing ด้วย Multiple Ad Groups | ทดสอบทีละตัวแปร (อายุ, Creative, ฯลฯ) ภายใน Campaign เดียวกัน |

---

## Bidding Strategy เปรียบเทียบ (เลือกให้ถูก)

| Strategy | วิธีคิดเงิน | เหมาะกับ | เมื่อไรควรใช้ |
|----------|------------|---------|--------------|
| CPV (Cost Per View) | จ่ายเมื่อดูเกิน 30 วินาที | มือใหม่, เน้น Engagement | เริ่มต้น Campaign แรก ต้องการควบคุมต้นทุน |
| CPM (Cost Per Mille) | จ่ายต่อ 1,000 Impressions | เน้น Reach สูงสุด | Campaign Awareness ต้องการให้คนเห็นมากที่สุด |
| CPA (Cost Per Acquisition) | จ่ายเมื่อเกิด Conversion | มีข้อมูลเพียงพอ, มี Tracking | Campaign ที่วิ่งมาแล้ว 2+ สัปดาห์ มี Conversion Data |

---

## Targeting Layers ซ้อน (ตัวอย่าง)

| Layer | ประเภท | ตัวอย่าง | ผลลัพธ์ |
|-------|--------|---------|---------|
| Layer 1 | Audience | คนสนใจเทคโนโลยี | กว้าง — Reach สูง |
| Layer 2 | Topic | Business Software | แคบลง — เจาะกลุ่มธุรกิจ |
| Layer 3 | Keyword | "AI tools for business" | แคบสุด — ตรงเป้ามาก |
| รวม 3 Layers | ซ้อนกัน | ทั้ง 3 เงื่อนไขพร้อมกัน | แม่นยำสูง แต่ Reach น้อย |

> **กฎ:** ซ้อน 2-3 ชั้นพอ ถ้ามากกว่านี้ Reach จะแคบจนไม่ได้ข้อมูลเพียงพอ

---

## ขั้นตอนการสร้าง Ad Creative

| ขั้นตอน | การดำเนินการ | หมายเหตุ |
|---------|-------------|----------|
| 1. วาง Video URL | ใส่ลิงก์วิดีโอจาก Youtube | ต้อง Upload ลง Youtube ก่อน |
| 2. ใส่ Headline | ข้อความสั้น ดึงดูด | จำกัดตัวอักษร ต้องกระชับ |
| 3. ใส่ Description | คำอธิบายเพิ่มเติม | บอกประโยชน์ที่คนดูจะได้ |
| 4. Companion Banner | รูป 300x60 px (Desktop) | ถ้าไม่มี Google Auto-generate |
| 5. CTA Overlay | ข้อความปุ่ม + Final URL | ชี้นำให้คนทำ Action ที่ต้องการ |

---

## A/B Testing ด้วย Multiple Ad Groups

| Ad Group | ตัวแปรทดสอบ | ตัวอย่าง |
|----------|------------|---------|
| Ad Group A vs B | อายุ | 18-24 vs 25-34 |
| Ad Group A vs B | ความยาววิดีโอ | 15 วินาที vs 30 วินาที |
| Ad Group A vs B | CTA Text | "สมัครฟรี" vs "เรียนรู้เพิ่มเติม" |

> **กฎทอง:** ทดสอบทีละ 1 ตัวแปร เพื่อให้รู้ว่าอะไรทำให้ผลต่างกัน

---

## Checklist ก่อน Launch

- [ ] ชื่อ Campaign ถูกต้องและสื่อความหมาย
- [ ] Budget ตรงตามที่ต้องการ
- [ ] Bidding Strategy ถูกแบบ (CPV/CPM/CPA)
- [ ] Targeting ครอบคลุมกลุ่มเป้าหมาย
- [ ] วิดีโอโฆษณาถูกตัว
- [ ] Headline + Description ดึงดูดและกระชับ
- [ ] CTA ข้อความชัดเจน + Final URL ถูกต้อง
- [ ] Preview ทั้ง Desktop และ Mobile แล้วโอเค

---

## ตัวเลขสำคัญ

| Metric | ค่า |
|--------|-----|
| Companion Banner Size | 300 x 60 px |
| Campaign Review Time (Google) | 24-48 ชั่วโมง |
| จำนวน Targeting Layers ที่แนะนำ | 2-3 ชั้น |
| A/B Test ตัวแปรต่อครั้ง | 1 ตัวแปร |

---

*Word count: ~550 | Tables: 7 | Estimated read time: 4 minutes*

---

> ทบทวนต่อ: **YTCAMP-008** — ข้อสรุปการทำ Youtube Ads Campaign
> Series: SWP3 Ch19 Youtube Ads Campaign
> PinkCastle Academy © 2026
