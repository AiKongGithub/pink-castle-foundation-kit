# วิธีอัพโหลดวิดีโอในระบบสมาชิก — SOMT-009
> **Format:** Insights Table
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 9
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

## ตาราง 10 Insights สำคัญ

| # | Insight | Detail | Application | Impact Level |
|---|---------|--------|-------------|--------------|
| 1 | เสียงสำคัญกว่าภาพสำหรับ Retention | คนยอมดูภาพ 720p ได้ แต่เสียงแย่ = ปิดทันที Audio มีผลต่อ Retention มากกว่า Visual Quality ลงทุนกับ Microphone คุ้มกว่ากล้องแพง | ซื้อ USB Microphone ดีๆ (2,000-5,000 บาท) ก่อนลงทุนกับกล้อง ใช้ AAC, 128-256 kbps, Stereo ทดสอบเสียงก่อนอัดทุกครั้ง | สูงมาก |
| 2 | 1080p เพียงพอ ไม่จำเป็นต้อง 4K | 4K ไฟล์ใหญ่เกินไป โหลดช้า Bandwidth สูง คนส่วนใหญ่ดูบนจอเล็ก (มือถือ/Laptop) 1080p ชัดเจนเพียงพอและไฟล์ขนาดเหมาะสม | อัดวิดีโอที่ 1080p ใช้ MP4 H.264 Compress ด้วย HandBrake ที่ 5-8 Mbps ลดขนาด 50-70% คุณภาพแทบไม่เปลี่ยน | สูงมาก |
| 3 | วิดีโอไม่ควรยาวเกิน 15-20 นาที | Attention Span อยู่ที่ 10-15 นาที วิดีโอสั้นมี Completion Rate สูงกว่าวิดีโอยาวมาก สมาชิกรู้สึกว่า "จบได้" จึงกดเข้าดู | ตัดวิดีโอให้ไม่เกิน 20 นาที ถ้ายาวกว่าให้แบ่งเป็น Part ทุก Part ต้องจบในตัวเอง มี Introduction และ Summary | สูงมาก |
| 4 | Thumbnail ที่มี Face + Font ใหญ่ เพิ่ม Click Rate | สมองมนุษย์สนใจใบหน้ามากที่สุด Font ใหญ่อ่านง่ายแม้จอเล็ก สีแบรนด์สร้าง Consistency หมายเลขบทเรียนช่วยหาง่าย | ออกแบบ Thumbnail Template 1 แบบ มี Face + Font ใหญ่ + เลขบทเรียน ขนาด 1280x720 px ใช้ซ้ำทุกบทเรียน ประหยัดเวลาออกแบบ | สูง |
| 5 | ชื่อบทเรียนต้องบอก Outcome ไม่ใช่แค่หมายเลข | "วิธีสร้าง Content ที่มีคนแชร์" ดีกว่า "บทที่ 3" เพราะสมาชิกรู้ล่วงหน้าว่าจะได้อะไร กดเข้าดูมากกว่า | ตั้งชื่อทุกบทเรียนด้วยรูปแบบ "วิธี..." หรือ "X อย่างที่ต้องรู้เรื่อง..." ทำให้ทุกชื่อสื่อถึง Value ที่จะได้ | สูง |
| 6 | เริ่ม Kartra Built-in แล้วย้าย Vimeo เมื่อโต | ไม่ต้องลงทุนเพิ่มตอนเริ่มต้น Kartra Embed Vimeo ได้ง่าย ย้ายได้ทุกเมื่อ Vimeo Pro มี Player สวย Analytics ดี ไม่มีโฆษณา | ใช้ Kartra Built-in ไปก่อน เมื่อมีสมาชิก 100+ คนค่อยพิจารณา Vimeo Pro (~$20/เดือน) เพื่อ Analytics และ Bandwidth ที่ดีขึ้น | ปานกลาง-สูง |
| 7 | Speed Control เป็น Feature เล็กที่ผลกระทบใหญ่ | สมาชิกหลายคนชอบดู 1.5x-2x ถ้าไม่มีจะรู้สึกเสียเวลา ส่งผลต่อ User Experience อย่างมาก | เปิด Speed Control ในทุก Player (1x, 1.25x, 1.5x, 2x) เป็น Default Setting ที่ต้องมีเสมอ | สูง |
| 8 | Adaptive Bitrate สำคัญสำหรับ Mobile Users | ปรับคุณภาพวิดีโออัตโนมัติตามความเร็วเน็ต เน็ตเร็ว 1080p เน็ตช้า 480p ทำให้วิดีโอไม่ Buffer ทุกสถานการณ์ | เลือก Video Hosting ที่รองรับ Adaptive Bitrate Streaming (Kartra และ Vimeo รองรับอยู่แล้ว) | ปานกลาง-สูง |
| 9 | Compression ลดขนาด 50-70% ประหยัด Storage | วิดีโอดิบจาก Camera ใหญ่มาก HandBrake (ฟรี) ลดขนาดได้มากโดยคุณภาพแทบไม่ต่าง ประหยัดพื้นที่ Hosting อัพโหลดเร็วขึ้น สมาชิก Buffer น้อยลง | Compress ทุกวิดีโอก่อนอัพโหลด ใช้ HandBrake ตั้ง H.264, 5-8 Mbps, AAC 128-256 kbps ทำเป็น Workflow มาตรฐาน | ปานกลาง-สูง |
| 10 | Offline Viewing เพิ่ม Engagement โดยเฉพาะต่างจังหวัด | ไม่ใช่ทุกที่จะมีเน็ตแรง สมาชิกต่างจังหวัดหรือระหว่างเดินทางต้องการ Offline Viewing การดาวน์โหลดวิดีโอทำให้เรียนต่อเนื่องได้ | ถ้า Platform รองรับ ให้เปิด Download Button สำหรับ Mobile ตั้ง DRM Protection ถ้ากังวลเรื่องการ Copy | ปานกลาง |

---

### สรุป Impact Level

| Level | จำนวน Insights |
|-------|---------------|
| สูงมาก | 3 |
| สูง | 3 |
| ปานกลาง-สูง | 3 |
| ปานกลาง | 1 |

---

*Insights count: 10 | Focus: Video Upload & Management in Membership*
