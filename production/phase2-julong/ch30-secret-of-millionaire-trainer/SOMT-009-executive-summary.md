# วิธีอัพโหลดวิดีโอในระบบสมาชิก — SOMT-009
> **Format:** Executive Summary
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 9
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

## Executive Summary

### สรุปภาพรวม

ตอนที่ 9 ใช้เวลา 22:21 นาที เจาะลึกเรื่องการอัพโหลดและจัดการวิดีโอในระบบสมาชิก ซึ่งเป็นเนื้อหาหลักของ Membership System ครอบคลุมตั้งแต่การเลือก Video Hosting (Kartra Built-in, Vimeo Pro, YouTube Unlisted) ไปจนถึง Technical Specifications (File Format, Resolution, Compression, Audio) การออกแบบ Thumbnail ที่ดึงดูด การจัดระเบียบบทเรียนแบบ Hierarchy (Course → Module → Lesson) การตั้งค่า Video Player และ Mobile Optimization

สิ่งที่โดดเด่นของตอนนี้คือการเน้นย้ำว่า "เสียงสำคัญกว่าภาพ" ในบริบทคอร์สออนไลน์ คนยอมดูภาพที่ไม่คมได้ แต่ถ้าเสียงแย่จะปิดทันที การลงทุนกับ Microphone ดีๆ จึงคุ้มค่ากว่ากล้องราคาแพง นอกจากนี้ยังเน้นว่าวิดีโอแต่ละตอนไม่ควรยาวเกิน 15-20 นาทีเพราะ Attention Span ของมนุษย์มีจำกัด

---

### Key Findings

1. **Video Hosting มี 3 ทางเลือกหลัก** — Kartra Built-in (ง่าย แต่พื้นที่จำกัด), Vimeo Pro (มืออาชีพ มี Analytics แต่มีค่าใช้จ่าย), YouTube Unlisted (ฟรี แต่ไม่ปลอดภัยและดูไม่มืออาชีพ) แนะนำเริ่มที่ Kartra แล้วย้ายไป Vimeo เมื่อโต

2. **เสียงสำคัญกว่าภาพ** — คนยอมรับภาพที่ไม่คมได้ แต่เสียงแย่ = ปิดทันที การลงทุนกับ Microphone ดีๆ คุ้มค่ากว่ากล้องราคาแพง Audio ต้อง AAC, 128-256 kbps

3. **1080p + H.264 + Compression เป็นมาตรฐาน** — ไม่จำเป็นต้อง 4K สำหรับคอร์สออนไลน์ Compress ด้วย HandBrake ที่ 5-8 Mbps ได้ไฟล์คุณภาพดีขนาดเหมาะสม

4. **วิดีโอไม่ควรยาวเกิน 15-20 นาที** — Attention Span อยู่ที่ 10-15 นาที วิดีโอสั้นมี Completion Rate สูงกว่า ถ้ายาวกว่านั้นให้แบ่งเป็นหลาย Part

5. **Thumbnail + ชื่อบทเรียนตัดสิน Click Rate** — Thumbnail ต้องมี Face + Font ใหญ่ + เลขบทเรียน ชื่อบทเรียนต้องบอก Outcome ที่ได้ ไม่ใช่แค่ "บทที่ 3" แต่เป็น "วิธีสร้าง Content ที่มีคนแชร์"

---

### ตาราง Video Hosting Comparison

| Hosting | ราคา | Bandwidth | Analytics | ความปลอดภัย | แนะนำ |
|---------|------|-----------|-----------|------------|-------|
| Kartra Built-in | รวมใน Plan | จำกัดตาม Plan | พื้นฐาน | ดี | เริ่มต้น |
| Vimeo Pro | ~$20/เดือน | ไม่จำกัด | ละเอียด | ดีมาก | เติบโต |
| YouTube Unlisted | ฟรี | ไม่จำกัด | ดี | ต่ำ (Share Link ได้) | ไม่แนะนำ |

---

### ตาราง Video Specifications

| Parameter | ค่าที่แนะนำ | หมายเหตุ |
|-----------|------------|----------|
| Format | MP4 (H.264) | รองรับทุก Browser/Device |
| Resolution | 1080p (1920x1080) | เพียงพอ ไม่ต้อง 4K |
| Video Bitrate | 5-8 Mbps | Compress ด้วย HandBrake |
| Audio Codec | AAC | มาตรฐาน |
| Audio Bitrate | 128-256 kbps | Stereo |
| Framerate | 30fps (Talking Head), 24fps (Screen Record) | ไม่ต้อง 60fps |
| Thumbnail | 1280x720 px | มี Face + Font ใหญ่ |
| Duration | 15-20 นาที/ตอน | แบ่ง Part ถ้ายาวกว่านี้ |

---

### Recommendations

1. **เริ่มด้วย Kartra Built-in แล้วย้ายไป Vimeo เมื่อโต** — ไม่ต้องลงทุนเพิ่มตอนเริ่มต้น Kartra Embed Vimeo ได้ง่าย ย้ายได้ตอนไหนก็ได้

2. **ลงทุนกับ Microphone ก่อนกล้อง** — USB Microphone ราคา 2,000-5,000 บาทเพิ่มคุณภาพเสียงได้มหาศาล ส่งผลต่อ Retention มากกว่าภาพที่คมขึ้น

3. **Compress ทุกวิดีโอก่อนอัพโหลด** — ใช้ HandBrake (ฟรี) ตั้ง 5-8 Mbps ลดขนาดไฟล์ได้ 50-70% โดยคุณภาพแทบไม่เปลี่ยน ประหยัดพื้นที่และ Bandwidth

4. **สร้าง Thumbnail Template ที่สม่ำเสมอ** — ออกแบบ Template 1 แบบ แล้วเปลี่ยนแค่ชื่อและเลขบทเรียน ทำให้ทุกบทเรียนดูเป็นชุดเดียวกัน ประหยัดเวลาออกแบบ

5. **เปิด Speed Control ในทุก Player** — สมาชิกหลายคนชอบดู 1.5x-2x Feature นี้เพิ่ม User Experience อย่างมาก ถ้าไม่มีจะรู้สึกเสียเวลา

---

### บทสรุปสำหรับผู้บริหาร

วิดีโอเป็นเนื้อหาหลักของ Membership System คุณภาพวิดีโอส่งผลโดยตรงกับ Retention Rate และ Member Satisfaction การเลือก Hosting ที่เหมาะสม การ Compress ไฟล์อย่างถูกวิธี การจัดระเบียบที่ชัดเจน และ Mobile Optimization เป็น 4 เสาหลักที่ต้องทำให้ดี ที่สำคัญ ลงทุนกับเสียง (Microphone) มากกว่าภาพ (Camera) เพราะเสียงมีผลต่อ Retention มากกว่า และจำกัดความยาววิดีโอไว้ที่ 15-20 นาทีต่อตอนเพื่อ Completion Rate ที่ดี

---

*Word count: ~700 | Reading time: 5 minutes*
