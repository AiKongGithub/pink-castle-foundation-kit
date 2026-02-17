# Insights Table: วิธีการติดตั้ง Plugin ตอนที่ 2 — WEB1-009
> **Format:** Insights Table (10 Rows)
> **Source:** SWP3 Ch10 สร้างเว็บไซต์ Part 1 ตอนที่ 9
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

| # | Insight (ข้อค้นพบ) | Detail (รายละเอียด) | Application (การนำไปใช้) | Impact Level (ระดับผลกระทบ) |
|---|---|---|---|---|
| 1 | เว็บช้ากว่า 3 วินาที = เสียลูกค้า 50% | Google ระบุว่าผู้เข้าชมกว่าครึ่งจะปิดเว็บที่โหลดนานเกิน 3 วินาที และยังใช้ Page Speed เป็น Ranking Factor อีกด้วย | ติดตั้ง Caching Plugin (WP Super Cache) + Image Optimization (ShortPixel) ทดสอบความเร็วด้วย Google PageSpeed Insights | สูง |
| 2 | Caching ลดภาระ Server อย่างมาก | Caching Plugin เก็บสำเนาหน้าเว็บ ไม่ต้องสร้างใหม่จาก Database ทุกครั้ง ลดเวลาโหลดจากหลายวินาทีเหลือไม่กี่มิลลิวินาที | ตั้งค่า WP Super Cache หรือ W3 Total Cache ให้เหมาะสม เปิด Page Cache และ Browser Cache | สูง |
| 3 | WebP เล็กกว่า JPG 25-35% | Image Optimization Plugin แปลงรูปเป็น WebP ซึ่งมีขนาดเล็กกว่ามากโดยไม่เสียคุณภาพ รูปภาพเป็นตัวการหลักที่ทำให้เว็บช้า | ใช้ ShortPixel หรือ Smush บีบอัดรูปทั้งเก่าและใหม่ เปิดการแปลง WebP อัตโนมัติ | กลาง |
| 4 | Social Sharing เพิ่มการเข้าถึงแบบ Organic | ปุ่มแชร์โซเชียลทำให้ผู้เข้าชมกระจายเนื้อหาไปยัง Facebook LINE Twitter Pinterest ได้ง่าย ช่วยสร้าง Traffic ฟรีจาก Social Media | เลือก Social Plugin ที่เบา (AddToAny) ใส่เฉพาะแพลตฟอร์มที่กลุ่มเป้าหมายใช้จริง หลีกเลี่ยงตัวที่โหลด JS หนัก | กลาง |
| 5 | Email List มีค่ามากกว่า Social Media Followers | Email List เป็นช่องทางสื่อสารตรงที่ไม่ต้องพึ่งอัลกอริทึม ไม่เสี่ยงถูกปิดบัญชี ส่งข้อเสนอถึงลูกค้าได้โดยตรง | ติดตั้ง MailChimp for WordPress เริ่มสะสม Email List ตั้งแต่วันแรก ใช้ OptinMonster สร้าง Popup เพื่อเพิ่มยอดสมัคร | สูง |
| 6 | Exit Intent เพิ่ม Conversion อย่างมาก | OptinMonster มีฟีเจอร์แสดง Popup เมื่อผู้ใช้กำลังจะปิดหน้าเว็บ (Exit Intent) เป็นโอกาสสุดท้ายในการเปลี่ยนผู้เข้าชมให้เป็นผู้สมัคร | ตั้งค่า Exit Intent Popup ที่นำเสนอข้อเสนอพิเศษ (Lead Magnet) เช่น eBook ฟรี หรือส่วนลดพิเศษ | กลาง |
| 7 | Page Builder เป็นการตัดสินใจระยะยาว | Elementor และ Thrive Architect เพิ่ม Code จำนวนมาก เนื้อหาผูกติดกับ Page Builder ตัวเดิม การย้ายในภายหลังยุ่งยากและเสียเวลามาก | เปรียบเทียบ Elementor (ใช้งานง่าย ทุกประเภทเว็บ) กับ Thrive (เน้น Conversion) เลือกให้เหมาะตั้งแต่แรก อย่าเปลี่ยนบ่อย | สูง |
| 8 | WooCommerce ฟรีแต่ทำให้เว็บหนักมาก | WooCommerce เพิ่มตาราง Database และฟังก์ชันจำนวนมาก เหมาะเฉพาะเว็บที่ต้องการขายของจริงจัง ไม่ควรลงเล่นๆ | ติดตั้ง WooCommerce เฉพาะเมื่อมีแผนจะขายสินค้าจริง คู่กับ Caching Plugin และ CDN เพื่อรองรับ Traffic | กลาง |
| 9 | Plugin Conflict แก้ได้ด้วย Deactivate ทีละตัว | เมื่อเว็บแสดงผลผิด หน้าจอขาว หรือฟีเจอร์ไม่ทำงาน ให้ Deactivate Plugin ทีละตัวตามลำดับ เมื่อเว็บกลับมาปกติก็จะรู้ว่าตัวไหนเป็นปัญหา | เมื่อพบปัญหา Conflict ให้สงบใจ Deactivate ทีละตัว ถ้าหาไม่เจอให้ Deactivate ทั้งหมดแล้วเปิดทีละตัว | สูง |
| 10 | สำรองข้อมูลก่อนอัปเดต Plugin เสมอ | การอัปเดต Plugin อาจทำให้เกิด Compatibility issue กับ WP เวอร์ชันปัจจุบันหรือ Plugin ตัวอื่น Backup ช่วยให้กู้คืนได้ทันที | ตั้งกฎ: สำรองข้อมูลก่อนอัปเดตทุกครั้ง อัปเดตทีละตัว ตรวจสอบเว็บหลังอัปเดตทุกครั้ง | สูง |

---

## สรุปตาม Impact Level

| ระดับ | จำนวน Insights | หัวข้อหลัก |
|-------|:---:|---|
| สูง | 6 | ความเร็ว, Caching, Email List, Page Builder, Conflict, Backup ก่อนอัปเดต |
| กลาง | 4 | WebP, Social Sharing, Exit Intent, WooCommerce |
| ต่ำ | 0 | — |

---

*จำนวน Insights ทั้งหมด: 10 รายการ*
