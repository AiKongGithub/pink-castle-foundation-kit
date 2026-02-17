# Insights Table: วิธีปรับแต่ง Performance — WEB2-006
> **Format:** Insights Table (10 Rows)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 6
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

| # | Insight (ข้อค้นพบ) | Detail (รายละเอียด) | Application (การนำไปใช้) | Impact Level (ระดับผลกระทบ) |
|---|---|---|---|---|
| 1 | เว็บช้า 1 วินาที = เสีย Conversion 7% | ผู้ใช้ 53% ออกจากเว็บถ้าโหลดเกิน 3 วินาที ทุก 1 วินาทีที่ช้าลง อัตรา Conversion ลดลงประมาณ 7% ส่งผลต่อรายได้โดยตรง | ตั้งเป้าหมายโหลดเว็บภายใน 3 วินาที (ดีมาก: ต่ำกว่า 2 วินาที) ทดสอบด้วย PageSpeed Insights เป็นประจำ | สูง |
| 2 | Google ใช้ Core Web Vitals จัดอันดับ | Core Web Vitals ประกอบด้วย LCP (Largest Contentful Paint), FID (First Input Delay), CLS (Cumulative Layout Shift) เป็นปัจจัยจัดอันดับของ Google | ตรวจสอบ Core Web Vitals ใน Google Search Console แก้ไขปัญหาที่พบ โดยเฉพาะ LCP ที่เกี่ยวข้องกับความเร็วโดยตรง | สูง |
| 3 | Browser Caching ทำให้โหลดครั้งที่ 2 เร็วขึ้น 40-60% | ไฟล์ CSS, JavaScript, รูปภาพ ถูกเก็บในเบราว์เซอร์ผู้เข้าชม ไม่ต้องโหลดใหม่เมื่อเข้าครั้งที่สอง ลดเวลาโหลดอย่างมาก | ตั้งค่าผ่านปลั๊กอิน cache เช่น WP Rocket, W3 Total Cache หรือ WP Super Cache (ฟรี) กำหนด expiry time ให้เหมาะสม | สูง |
| 4 | GZIP ลดขนาดไฟล์ได้ 60-80% | GZIP Compression บีบอัดไฟล์ก่อนส่งจาก server คล้ายการซิปไฟล์ เบราว์เซอร์ decompress อัตโนมัติ ไม่ส่งผลต่อคุณภาพ | เปิดใช้ GZIP ผ่าน .htaccess หรือปลั๊กอิน cache ตรวจสอบว่าทำงานได้ที่ checkgzipcompression.com | สูง |
| 5 | รูปภาพเป็นตัวการหลักที่ทำเว็บช้า | รูปภาพคิดเป็น 50-80% ของขนาดหน้าเว็บทั้งหมด รูปที่ไม่ผ่านการ optimize จะมีขนาดใหญ่มาก ทำให้โหลดช้า | ลดขนาดรูปก่อนอัปโหลดทุกครั้ง ใช้รูปแบบ WebP (เล็กกว่า JPEG 25-34%) ติดตั้งปลั๊กอิน optimize เช่น ShortPixel, Smush | สูง |
| 6 | Lazy Loading ลดเวลาโหลดหน้าแรกอย่างมาก | รูปภาพและวิดีโอโหลดเฉพาะตอนเลื่อนมาถึง ไม่โหลดทั้งหมดตั้งแต่แรก WordPress 5.5+ มี Lazy Loading ในตัวสำหรับรูปภาพ | ตรวจสอบว่า Lazy Loading เปิดใช้งานอยู่ สำหรับวิดีโอ embed อาจต้องใช้ปลั๊กอินเสริมเช่น WP YouTube Lyte | กลาง |
| 7 | Minification ลดขนาด CSS/JS 10-30% | เอาช่องว่าง comment และอักขระที่ไม่จำเป็นออกจากไฟล์ CSS/JavaScript โดยไม่ส่งผลต่อการทำงาน | ใช้ Autoptimize (ฟรี) หรือ WP Rocket (มีค่าใช้จ่าย) ทำ Minification อัตโนมัติ ทดสอบหลังเปิดใช้ว่าเว็บไม่พัง | กลาง |
| 8 | Database บวมทำให้ query ช้าลงเรื่อยๆ | WordPress สะสม post revisions, spam comments, transient data, auto-drafts เมื่อเวลาผ่านไป ฐานข้อมูลจะใหญ่ขึ้นเรื่อยๆ | ใช้ WP-Optimize ทำความสะอาดฐานข้อมูลเดือนละ 1-2 ครั้ง จำกัด post revisions ไว้ที่ 3-5 revision ต่อบทความ | กลาง |
| 9 | CDN ทำให้เว็บเร็วจากทุกที่ในโลก | CDN กระจายไฟล์ไปยัง server ทั่วโลก ส่งจากจุดที่ใกล้ผู้ใช้ที่สุด ลดระยะทางในการส่งข้อมูล | ใช้ Cloudflare (ฟรี) เป็น CDN ตั้งค่าง่าย แค่เปลี่ยน Nameserver นอกจาก CDN ยังได้ DDoS Protection ด้วย | สูง |
| 10 | ต้องทดสอบเป็นประจำ ไม่ใช่ครั้งเดียว | ทุกครั้งที่เพิ่มปลั๊กอิน อัปเดตธีม หรือเพิ่มเนื้อหา อาจส่งผลต่อความเร็ว ต้องติดตามตลอด | ทดสอบด้วย PageSpeed Insights + GTmetrix ทุกเดือน หรือทุกครั้งที่เปลี่ยนแปลงเว็บไซต์ บันทึกผลเปรียบเทียบ | กลาง |

---

## สรุปตาม Impact Level

| ระดับ | จำนวน Insights | หัวข้อหลัก |
|-------|:---:|---|
| สูง | 6 | ความเร็ว-Conversion, Core Web Vitals, Browser Cache, GZIP, Image Optimization, CDN |
| กลาง | 4 | Lazy Loading, Minification, Database Optimization, การทดสอบเป็นประจำ |
| ต่ำ | 0 | — |

---

*จำนวน Insights ทั้งหมด: 10 รายการ*
