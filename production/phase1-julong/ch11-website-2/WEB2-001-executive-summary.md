# Executive Summary: วิธีการตั้งค่าต่างๆ ของ WordPress — WEB2-001
> **Format:** Executive Summary
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 1
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## บทสรุปผู้บริหาร

### ภาพรวม

การตั้งค่า WordPress อย่างถูกต้องตั้งแต่เริ่มต้นเป็นรากฐานสำคัญของเว็บไซต์ที่ประสบความสำเร็จ ครอบคลุม 6 หมวดหลัก ได้แก่ General, Writing, Reading, Discussion, Media และ Permalinks แต่ละหมวดส่งผลโดยตรงต่อประสิทธิภาพเว็บไซต์ ประสบการณ์ผู้ใช้ และอันดับ SEO การละเลยขั้นตอนนี้อาจนำไปสู่ปัญหาที่แก้ไขยากในภายหลัง โดยเฉพาะเรื่องโครงสร้าง URL ที่ส่งผลกระทบต่อลิงก์ทั้งหมดของเว็บไซต์

### ประเด็นสำคัญ (Key Findings)

**1. General Settings — ฐานรากของเว็บไซต์**

Site Title และ Tagline คือสิ่งแรกที่ Google และผู้เข้าชมเห็นในผลการค้นหา Timezone ต้องตั้งให้ถูกต้อง (Bangkok, UTC+7 สำหรับประเทศไทย) เพื่อให้เวลาที่แสดงในบทความตรงกับความเป็นจริง Date Format และ Site Language ช่วยให้เว็บไซต์เป็นมิตรกับกลุ่มเป้าหมาย

**2. Writing & Reading Settings — ควบคุมเนื้อหาและการแสดงผล**

Writing Settings กำหนดค่าเริ่มต้นในการเขียนบทความ เช่น Default Post Category Reading Settings ควบคุมว่าหน้าแรกจะแสดงบทความล่าสุดหรือเป็น Static Page (เหมาะกับเว็บธุรกิจ) จุดสำคัญอยู่ที่ Search Engine Visibility ซึ่งต้องปิดการซ่อนจาก Google เมื่อเว็บไซต์พร้อมเปิดตัว

**3. Discussion & Media Settings — จัดการปฏิสัมพันธ์และภาพ**

ระบบคอมเมนต์ควรเปิด Comment Moderation เพื่อกรองสแปม Media Settings ควบคุมขนาดรูปภาพ 3 ระดับ (Thumbnail 150px, Medium 300px, Large 1024px) ที่ WordPress สร้างอัตโนมัติ

**4. Permalink Settings — กระทบ SEO โดยตรง**

การเลือกโครงสร้าง URL เป็น Post name (เช่น yoursite.com/post-title) เป็นการตั้งค่าที่สำคัญที่สุดและต้องทำตั้งแต่วันแรก การเปลี่ยน Permalink หลังจากมีเนื้อหาจำนวนมากจะทำให้ลิงก์เก่าใช้งานไม่ได้และกระทบอันดับ SEO อย่างรุนแรง

### ตารางสรุป 6 หมวดการตั้งค่า

| หมวด | การตั้งค่าหลัก | ระดับความสำคัญ |
|------|---------------|---------------|
| General | Site Title, Tagline, Timezone, Language | สูง |
| Writing | Default Post Category, Post Format | กลาง |
| Reading | Homepage Display, Posts per Page, Search Visibility | สูง |
| Discussion | Comment Moderation, Avatars, Notifications | กลาง |
| Media | Thumbnail, Medium, Large image sizes | ต่ำ |
| Permalinks | URL Structure (Post name แนะนำ) | สูงมาก |

### ข้อเสนอแนะ (Recommendations)

**ทำทันทีหลังติดตั้ง WordPress:**
1. ตั้ง Permalink เป็น Post name ก่อนเป็นอันดับแรก
2. ตั้ง Timezone เป็น Bangkok (UTC+7)
3. ใส่ Site Title และ Tagline ที่สื่อความหมาย
4. เปิด Comment Moderation เพื่อป้องกันสแปม

**เมื่อเว็บพร้อมเปิดตัว:** ตรวจสอบว่า Search Engine Visibility ไม่ได้ถูกซ่อนจาก Google เพื่อให้เว็บไซต์ถูกจัดอันดับในผลการค้นหา

**หลักการสำคัญ:** ตั้งค่าพื้นฐานให้ถูกต้องตั้งแต่ครั้งแรก ดีกว่ากลับมาแก้ไขทีหลัง โดยเฉพาะ Permalink ที่เปลี่ยนแปลงภายหลังได้ยากมาก

---

*สิ้นสุดบทสรุปผู้บริหาร — ประมาณ 450 คำ*
