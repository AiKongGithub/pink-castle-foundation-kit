# วิธีเชื่อม Capture Page กับ Thank You Page — YTCAMP-002 Insights Table
> Format: Insights Table (10 rows)
> Source: SWP3 Ch19 Youtube Ads Campaign ตอนที่ 2
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 0:42:23

---

| # | Insight | รายละเอียด | ระดับสำคัญ | การนำไปใช้ |
|---|---------|-----------|-----------|-----------|
| 1 | **Capture Page = ประตูหน้าบ้าน** | Capture Page และ Thank You Page เปรียบเหมือนประตูหน้าบ้านกับห้องรับแขก ถ้าเชื่อมไม่ถูกต้อง (ประตูเปิดไม่ได้ / ไปผิดห้อง) ลูกค้าจะหายไปเลย ดังนั้นขั้นตอนนี้เป็นพื้นฐานที่สำคัญที่สุดก่อนทำ Youtube Ads | ⭐⭐⭐⭐⭐ Critical | เชื่อมและทดสอบ Capture Page → Thank You Page ให้สมบูรณ์ก่อนคิดเรื่อง Ads เด็ดขาด อย่าข้ามขั้นตอนนี้ |
| 2 | **After Submission Settings คือจุดเชื่อม** | ใน Kartra การเชื่อมเพจทำผ่าน Page Builder → Form Element → After Submission Settings → Redirect to Page → เลือก Thank You Page ต้องมั่นใจว่า URL และ Custom Domain ตั้งค่าตรงกัน | ⭐⭐⭐⭐⭐ Critical | เข้า Page Builder ตั้งค่า After Submission Settings ทันที ตรวจสอบ Domain ให้ตรงกันทั้ง 2 หน้า |
| 3 | **Single Opt-in สำหรับ Youtube Ads** | มี 2 แบบ: Single Opt-in (กรอกแล้วเข้าเลย) และ Double Opt-in (ต้องยืนยันอีเมลก่อน) สำหรับ Youtube Ads แนะนำ Single Opt-in เพื่อให้ Flow ลื่นไหล ไม่เสีย Lead ระหว่างขั้นตอนยืนยัน | ⭐⭐⭐⭐ High | ตั้งค่า Opt-in เป็น Single Opt-in ในหน้า Form Settings ของ Kartra สำหรับแคมเปญ Youtube Ads |
| 4 | **Internal Redirect ดีกว่า External** | Internal Redirect (ภายใน Kartra) ง่ายและเร็วกว่า — แค่เลือกจาก Dropdown External Redirect (URL นอก) ต้องใส่ Full URL ให้ถูก 100% และอาจช้ากว่า แนะนำ Internal Redirect สำหรับ Youtube Ads Campaign | ⭐⭐⭐⭐ High | ใช้ Internal Redirect เป็นค่าเริ่มต้น ใช้ External เฉพาะเมื่อจำเป็นต้อง Redirect ไปเว็บนอก Kartra |
| 5 | **Redirect ครั้งเดียว ห้ามหลายชั้น** | Redirect หลายชั้นทำให้ช้า — ยิ่ง Redirect มากชั้นยิ่งเสียเวลา ควร Redirect ครั้งเดียวจาก Capture Page ไป Thank You Page เลย ถ้าเพจโหลดช้า คนจะปิดหน้าไปก่อนที่จะถึง Thank You Page | ⭐⭐⭐⭐⭐ Critical | ตรวจสอบว่า Redirect ไม่ผ่านหน้ากลาง (intermediate page) ให้ไปตรงจาก Capture → Thank You |
| 6 | **Tracking Pixel 2 จุดเป็นขั้นต่ำ** | ต้องติดตั้งอย่างน้อย 2 Pixel: (1) Google Ads Conversion Tag บน Thank You Page (นับ Lead) (2) Google Analytics Tag บนทั้ง 2 หน้า (วัดพฤติกรรม) Pixel คือโค้ดเล็กๆ ที่ส่งสัญญาณกลับไปบอก Google Ads | ⭐⭐⭐⭐⭐ Critical | ติดตั้ง Pixel ทั้ง 2 จุดใน Kartra (Page Settings → Tracking Code) แล้วเช็คด้วย Google Tag Assistant ก่อนปล่อยแคมเปญ |
| 7 | **ติดตั้ง Pixel ก่อน ไม่ใช่ทีหลัง** | เคล็ดลับสำคัญ: ติดตั้ง Tracking Pixel ก่อนปล่อยแคมเปญ แล้วเช็คให้แน่ใจว่าทำงานถูกต้อง อย่ารอจนปล่อย Ads ไปแล้วค่อยมาเช็ค เพราะถ้า Pixel ไม่ทำงาน = ไม่มีข้อมูล = วัดผลไม่ได้ = เสียเงินฟรี | ⭐⭐⭐⭐⭐ Critical | ก่อนกดปล่อยแคมเปญ ให้ Checklist: Pixel ติดแล้ว ✅ Tag Assistant เช็คแล้ว ✅ ถ้ายังไม่ครบ ห้ามปล่อย! |
| 8 | **ทดสอบเหมือนลูกค้าจริง** | การทดสอบ Conversion Flow ต้องทำทุกขั้นตอนเหมือนเป็นลูกค้าจริง — กรอกฟอร์มจริง ดู Redirect ทำงานไหม Thank You Page ขึ้นมาไหม Conversion ถูกนับใน Google Ads ไหม ให้เพื่อน/ทีมช่วยทดสอบด้วย | ⭐⭐⭐⭐ High | ทดสอบด้วยตัวเอง 1 รอบ + ให้คนอื่นทดสอบอีก 1 รอบ ก่อนปล่อยแคมเปญจริง |
| 9 | **Mobile Test สำคัญกว่า Desktop** | คนส่วนใหญ่ดู Youtube บนมือถือ ดังนั้นเมื่อคลิกลิงก์จากโฆษณา จะเปิด Capture Page บนมือถือ ถ้า Redirect ไม่ทำงานหรือเพจโหลดช้าบนมือถือ = เสีย Lead ทันที แม้ Desktop จะทำงานปกติก็ไม่พอ | ⭐⭐⭐⭐⭐ Critical | ทดสอบ Flow ทั้งหมดบนมือถือจริง (ไม่ใช่แค่ Responsive Mode ในเบราว์เซอร์) ใช้ทั้ง iOS และ Android ถ้าเป็นไปได้ |
| 10 | **Page Speed < 3 วินาที** | ใช้ Google PageSpeed Insights เช็คว่าทั้ง Capture Page และ Thank You Page โหลดเร็วพอ ถ้าช้ากว่า 3 วินาที อาจเสีย Lead ไปเยอะ ความเร็วมีผลโดยตรงต่อ Conversion Rate | ⭐⭐⭐⭐ High | เช็ค PageSpeed Insights ทั้ง 2 หน้า ถ้าช้ากว่า 3 วินาที ให้ Optimize (ลดรูป, ลดโค้ดไม่จำเป็น) |

---

## สรุป Priority Actions

| Priority | Action | Timeline |
|----------|--------|----------|
| P1 | เชื่อม Capture Page → Thank You Page ใน Kartra (After Submission Settings) | วันนี้ |
| P2 | ตั้งค่า Single Opt-in + Internal Redirect | วันนี้ |
| P3 | ติดตั้ง Tracking Pixel 2 จุด (Conversion Tag + GA Tag) | วันที่ 2 |
| P4 | เช็ค Pixel ด้วย Google Tag Assistant | วันที่ 2 |
| P5 | ทดสอบ Full Flow บน Desktop + Mobile + เช็ค PageSpeed | วันที่ 3 |

---

> ทบทวนต่อ: **YTCAMP-003** — Youtube Ads Campaign ตอนที่ 3
> Series: SWP3 Ch19 Youtube Ads Campaign
> PinkCastle Academy © 2026
