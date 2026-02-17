# Insights Table: วิธีการตั้งค่า WP-Rocket — WEB2-012
> **Format:** Insights Table (10 Rows)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 12
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

| # | Insight (ข้อค้นพบ) | Detail (รายละเอียด) | Application (การนำไปใช้) | Impact Level (ระดับผลกระทบ) |
|---|---|---|---|---|
| 1 | Minify CSS/JS ลดขนาดไฟล์โดยไม่กระทบการทำงาน | ลบช่องว่าง บรรทัดว่าง และ comment ที่ไม่จำเป็นออกจากไฟล์ CSS/JS ทำให้ขนาดไฟล์เล็กลง โหลดเร็วขึ้น | เปิด Minify CSS และ Minify JS เป็นอันดับแรก ทดสอบเว็บให้แน่ใจว่าไม่มีปัญหาหน้าตาเพี้ยน | สูง |
| 2 | Combine CSS/JS ลด HTTP Requests แต่มีความเสี่ยง | รวมไฟล์หลายตัวเป็นไฟล์เดียว ลดจำนวนการเชื่อมต่อ server แต่อาจทำให้ CSS/JS ทำงานผิดปกติ | เปิดทดลอง ถ้าหน้าเว็บเพี้ยนหรือฟังก์ชันพังให้ปิดทันที ใช้แค่ Minify ก็เพียงพอ | กลาง |
| 3 | Defer JS Loading เร่งการแสดงผลหน้าเว็บ | ให้ HTML โหลดเสร็จก่อนแล้วค่อยรัน JavaScript ทำให้ผู้ใช้เห็นเนื้อหาเร็วขึ้นมาก ส่งผลดีต่อ First Contentful Paint | เปิด Defer JS Loading เป็นค่าเริ่มต้น ถ้าพบปัญหา JS บางตัวทำงานผิดปกติ ให้ exclude JS ตัวนั้นออก | สูง |
| 4 | LazyLoad ลดเวลาโหลดหน้าแรกอย่างมาก | รูปภาพ iframes และวิดีโอโหลดเฉพาะตอนเลื่อนลงมาถึง ลดจำนวนทรัพยากรที่ต้องโหลดตอนเปิดหน้า | เปิด LazyLoad ทั้ง images, iframes และ videos โดยเฉพาะเว็บที่มีรูปภาพมากกว่า 10 รูปต่อหน้า | สูง |
| 5 | Missing Image Dimensions ส่งผลต่อ Core Web Vitals | รูปภาพที่ไม่มี width/height ทำให้เกิด Layout Shift (CLS) หน้าเว็บกระตุกเมื่อรูปโหลดเสร็จ CLS เป็นหนึ่งใน Core Web Vitals ที่ Google ใช้จัดอันดับ | เปิด Add Missing Image Dimensions ทันที เป็นฟีเจอร์ที่ไม่มีผลข้างเคียง ช่วย CLS ได้อย่างชัดเจน | สูง |
| 6 | Sitemap-based Preloading ให้ทุกคนได้ cache ทันที | WP-Rocket Crawl ทุกหน้าตาม Sitemap แล้วสร้าง cache ล่วงหน้า ผู้เข้าชมคนแรกก็ได้หน้าที่ cache แล้วเลย | เปิด Preloading และตรวจสอบว่า Sitemap URL ถูกต้อง ถ้าใช้ Yoast SEO ระบบจะดึง Sitemap ให้อัตโนมัติ | กลาง |
| 7 | Never Cache URLs ป้องกันปัญหาข้อมูลล้าสมัย | หน้าที่มีข้อมูลเฉพาะบุคคลหรือเปลี่ยนแปลงบ่อย เช่น Checkout, Cart, My Account ไม่ควร cache เพราะผู้ใช้อาจเห็นข้อมูลเก่า | ตั้ง Never Cache สำหรับหน้า /checkout/, /cart/, /my-account/ และหน้าที่มีฟอร์มลงทะเบียน | สูง |
| 8 | Database Cleanup ลดขนาดฐานข้อมูลและเร่ง query | Post Revisions, Auto Drafts, Transients, Spam Comments สะสมจนฐานข้อมูลบวมเป็น MB ลบออกช่วยให้ query เร็วขึ้น | ตั้ง Database Cleanup เป็นประจำ (สัปดาห์ละครั้ง) แต่อย่าลบ Revisions ถ้ายังต้องการประวัติการแก้ไข | กลาง |
| 9 | Heartbeat API กินทรัพยากร server อย่างเงียบๆ | WordPress ส่ง heartbeat ทุก 15-60 วินาที กินทรัพยากร CPU และ bandwidth โดยเฉพาะบนโฮสติ้ง Shared ที่มีทรัพยากรจำกัด | ลดความถี่ Heartbeat เป็น 120 วินาที หรือปิดใน Frontend และ Post Editor (เก็บไว้แค่ Dashboard) | กลาง |
| 10 | ทดสอบก่อน-หลังด้วย GTmetrix เห็นผลลัพธ์ชัดเจน | ใช้ GTmetrix วัดคะแนนก่อนเปิด WP-Rocket จากนั้นตั้งค่าแล้ววัดอีกครั้ง คะแนน PageSpeed เพิ่มขึ้น 20-40 คะแนน เวลาโหลดลดลง 40-60% | ทดสอบทุกครั้งหลังปรับตั้งค่า เก็บ screenshot ก่อน-หลังเป็นหลักฐาน ใช้ GTmetrix เป็นตัวตัดสินว่าตั้งค่าถูกหรือไม่ | สูง |

---

## สรุปตาม Impact Level

| ระดับ | จำนวน Insights | หัวข้อหลัก |
|-------|:---:|---|
| สูง | 6 | Minify, Defer JS, LazyLoad, Image Dimensions, Never Cache URLs, GTmetrix |
| กลาง | 4 | Combine CSS/JS, Preloading, Database Cleanup, Heartbeat Control |
| ต่ำ | 0 | — |

---

*จำนวน Insights ทั้งหมด: 10 รายการ*
