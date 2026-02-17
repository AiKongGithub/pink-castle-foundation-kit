# วิธีเชื่อม Capture Page กับ Thank You Page — YTCAMP-002
> **Format:** Executive Summary
> **Source:** SWP3 Ch19 Youtube Ads Campaign ตอนที่ 2
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18
> **Duration:** 0:42:23

---

## สรุปภาพรวม

บทเรียนนี้เป็นตอนที่ยาวที่สุดของซีรีส์ Youtube Ads Campaign เน้นการลงมือปฏิบัติจริงในการเชื่อม Capture Page กับ Thank You Page ใน Kartra เนื้อหาครอบคลุม 4 ขั้นตอนหลัก ได้แก่ การเชื่อมเพจใน Kartra (Page Linking), การตั้งค่า Redirect ทั้ง Internal และ External, การติดตั้ง Tracking Pixel สำหรับ Google Ads และ Google Analytics และการทดสอบ Conversion Flow ทั้งหมดก่อนปล่อยแคมเปญจริง เปรียบเทียบ Capture Page กับ Thank You Page เป็นเหมือน "ประตูหน้าบ้าน" กับ "ห้องรับแขก" — ถ้าเชื่อมไม่ถูกต้อง ลูกค้าจะหายไปเลย

## ประเด็นสำคัญ (Key Takeaways)

| # | ประเด็น | รายละเอียด |
|---|---------|-----------|
| 1 | Capture Page = ประตูหน้าบ้าน | หน้ารับข้อมูลที่มีฟอร์มให้กรอก ต้องเชื่อมกับ Thank You Page อย่างถูกต้อง |
| 2 | After Submission Settings | ใน Kartra ตั้งค่า Redirect หลังกรอกฟอร์มที่ Form Element → After Submission |
| 3 | Internal vs External Redirect | Internal ง่ายและเร็วกว่า (แนะนำ) / External ต้องใส่ Full URL ให้ถูก |
| 4 | Tracking Pixel 2 จุด | Google Ads Conversion Tag (Thank You Page) + GA Tag (ทั้ง 2 หน้า) |
| 5 | ทดสอบก่อนปล่อยเสมอ | Test ทุกขั้นตอนบนทั้ง Desktop และ Mobile ก่อนเริ่มแคมเปญจริง |

## โครงสร้างเนื้อหา

| Segment | หัวข้อ | Timestamp | สาระสำคัญ |
|---------|--------|-----------|-----------|
| 1 | เปิดรายการ | 00:00 - 02:00 | ภาพรวมและเปรียบเทียบ Capture Page = ประตูหน้าบ้าน |
| 2 | Kartra Page Linking | 02:00 - 05:00 | เชื่อม Capture Page → Thank You Page ใน Page Builder |
| 3 | Redirect Setup | 05:00 - 08:00 | Internal vs External Redirect + Speed + Mobile Test |
| 4 | Tracking Pixels | 08:00 - 11:00 | Google Ads Conversion Tag + GA Tag + Google Tag Assistant |
| 5 | Conversion Flow Test | 11:00 - 13:30 | ทดสอบ Full Flow + PageSpeed Insights |

## Conversion Flow แบบสมบูรณ์

```
Youtube Ad (วิดีโอโฆษณา)
    ↓ คลิก
Capture Page (ฟอร์มกรอกข้อมูล)
    ↓ กรอก + Submit
Redirect (Internal/External)
    ↓ อัตโนมัติ
Thank You Page (ขอบคุณ)
    ↓ Pixel ทำงาน
Google Ads Conversion Tag (นับ Lead)
    + GA Tag (วัดพฤติกรรม)
```

## Tracking Pixel Checklist

| # | Pixel | ติดตั้งที่ | วัตถุประสงค์ | ตรวจสอบด้วย |
|---|-------|-----------|-------------|-------------|
| 1 | Google Ads Conversion Tag | Thank You Page | นับ Conversion (Lead) | Google Tag Assistant |
| 2 | Google Analytics Tag | Capture Page + Thank You Page | วัดพฤติกรรมผู้ใช้ | Google Tag Assistant |

## Testing Checklist

| # | รายการทดสอบ | สถานะ | หมายเหตุ |
|---|------------|--------|---------|
| 1 | กรอกฟอร์มจริงบน Capture Page | ▢ | ใช้อีเมลทดสอบ |
| 2 | Redirect ไป Thank You Page | ▢ | ต้องเร็ว ไม่เกิน 3 วินาที |
| 3 | Pixel ทำงาน (Tag Assistant) | ▢ | ทั้ง Conversion Tag และ GA Tag |
| 4 | ทดสอบบน Desktop | ▢ | Chrome, Safari, Firefox |
| 5 | ทดสอบบน Mobile | ▢ | สำคัญมาก — คนส่วนใหญ่มาจาก Youtube บนมือถือ |
| 6 | Page Speed < 3 วินาที | ▢ | ใช้ Google PageSpeed Insights |

## คำแนะนำสำหรับผู้บริหาร

การเชื่อม Capture Page กับ Thank You Page เป็นพื้นฐานที่สำคัญที่สุดก่อนเริ่ม Youtube Ads Campaign ถ้าขั้นตอนนี้ไม่ถูกต้อง ต่อให้โฆษณาดีแค่ไหน งบที่ใช้ก็จะสูญเปล่า การลงทุนเวลาทดสอบ Flow ทั้งหมดก่อนปล่อยแคมเปญจะช่วยป้องกันการเสียเงินโดยไม่จำเป็น สิ่งสำคัญคือ (1) ใช้ Single Opt-in เพื่อให้ Flow ลื่นไหล (2) ติดตั้ง Tracking Pixel ก่อนปล่อยแคมเปญ (3) ทดสอบบน Mobile เสมอ เพราะผู้ชม Youtube ส่วนใหญ่อยู่บนมือถือ

---

*Word count: ~500 | Tables: 5 | Reading time: 3 minutes*
