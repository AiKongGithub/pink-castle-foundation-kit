# วิธีเชื่อม Capture Page กับ Thank You Page — YTCAMP-002
> Format: Flashcards (12 Cards)
> Source: SWP3 Ch19 Youtube Ads Campaign ตอนที่ 2
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 0:42:23

---

=== CARD 1 ===
Q: Capture Page และ Thank You Page เปรียบเทียบได้กับอะไร?
A: Capture Page เปรียบเหมือน **ประตูหน้าบ้าน** ที่รับลูกค้าเข้ามา ส่วน Thank You Page เปรียบเหมือน **ห้องรับแขก** ที่ต้อนรับหลังเข้ามาแล้ว ถ้าประตูเปิดไม่ได้หรือเปิดแล้วไปผิดห้อง ลูกค้าจะหายไปเลย ดังนั้นการเชื่อมทั้ง 2 หน้าเข้าด้วยกันอย่างถูกต้องจึงสำคัญมาก

---

=== CARD 2 ===
Q: วิธีเชื่อม Capture Page กับ Thank You Page ใน Kartra ทำอย่างไร?
A: **(1)** เข้า Page Builder → เลือก Capture Page **(2)** คลิกที่ Form Element **(3)** ไปที่ **After Submission Settings** **(4)** เลือก **Redirect to Page** **(5)** เลือก Thank You Page ที่สร้างไว้ สิ่งที่ต้องระวังคือ URL ต้องถูกต้อง ถ้าใช้ Custom Domain ต้องตั้งค่า Domain ให้ตรงกัน

---

=== CARD 3 ===
Q: Opt-in Confirmation มี 2 แบบอะไร และแบบไหนแนะนำสำหรับ Youtube Ads?
A: **(1) Single Opt-in** — กรอกฟอร์มแล้วเข้า Thank You Page ได้เลย ไม่ต้องยืนยันอีเมล **(2) Double Opt-in** — ต้องยืนยันอีเมลก่อนจึงเข้า Thank You Page ได้ สำหรับ Youtube Ads Campaign **แนะนำ Single Opt-in** เพื่อให้ Flow ลื่นไหล ไม่สูญเสีย Lead ระหว่างทาง

---

=== CARD 4 ===
Q: Redirect ใน Kartra มีกี่แบบ แบบไหนแนะนำ?
A: มี 2 แบบ: **(1) Internal Redirect** — ส่งไปยังหน้าอื่นภายใน Kartra เดียวกัน แค่เลือกจาก Dropdown **แนะนำแบบนี้** เพราะง่ายกว่าและเร็วกว่า **(2) External Redirect** — ส่งไปยัง URL ภายนอก ต้องใส่ Full URL ให้ถูกต้อง 100% ใช้เมื่อจำเป็นต้อง Redirect ไปเว็บนอก Kartra

---

=== CARD 5 ===
Q: ทำไม Redirect Speed จึงสำคัญ?
A: เพราะ **ถ้าเพจโหลดช้า คนจะปิดหน้าไปก่อน** — ยิ่ง Redirect หลายชั้นยิ่งช้า ควร **Redirect ครั้งเดียว** จาก Capture Page ไป Thank You Page เลย ไม่ผ่านหน้าอื่น และต้อง **ทดสอบบนมือถือ** ด้วย เพราะคนส่วนใหญ่เข้ามาจาก Youtube บนมือถือ ถ้า Redirect ไม่ทำงานบนมือถือ = เสีย Lead ทันที

---

=== CARD 6 ===
Q: Tracking Pixel คืออะไร ทำงานอย่างไร?
A: **Tracking Pixel** คือโค้ดเล็กๆ ที่ฝังไว้ในหน้าเว็บ เมื่อมีคนเข้ามาถึงหน้านั้น Pixel จะ **ส่งสัญญาณกลับไปบอก Google Ads** ว่า "มีคนมาถึงหน้านี้แล้ว" ทำให้เราสามารถวัดผลแคมเปญได้ เช่น นับจำนวน Conversion ดูพฤติกรรมผู้ใช้ และคำนวณอัตราการแปลง

---

=== CARD 7 ===
Q: ต้องติดตั้ง Tracking Pixel อย่างน้อยกี่จุด ที่ไหนบ้าง?
A: อย่างน้อย **2 จุด**: **(1) Google Ads Conversion Tag** — ติดบน **Thank You Page** เพื่อนับจำนวน Conversion (Lead) **(2) Google Analytics Tag** — ติดบนทั้ง **Capture Page และ Thank You Page** เพื่อดูพฤติกรรมผู้ใช้ เช่น มีคนเข้า Capture Page กี่คน กรอกฟอร์มกี่คน อัตรา Conversion เท่าไร

---

=== CARD 8 ===
Q: วิธีติดตั้ง Tracking Pixel ใน Kartra ทำอย่างไร?
A: เข้าไปที่ **Page Settings** → เลือก **Tracking Code** → วาง Pixel Code ได้เลย Kartra มีช่องให้ใส่ทั้ง **Header Code** และ **Body Code** เคล็ดลับสำคัญ: **ติดตั้ง Pixel ก่อนปล่อยแคมเปญ** แล้วเช็คใน **Google Tag Assistant** ว่า Pixel ทำงานถูกต้อง อย่ารอจนปล่อย Ads ไปแล้วค่อยมาเช็ค

---

=== CARD 9 ===
Q: Conversion Flow ที่สมบูรณ์มีขั้นตอนอะไรบ้าง?
A: **(1)** คนดูโฆษณาบน Youtube → **(2)** คลิกลิงก์ → **(3)** มาถึง Capture Page → **(4)** กรอกฟอร์ม → **(5)** Redirect ไป Thank You Page → **(6)** Pixel ส่งสัญญาณ Conversion → **(7)** Google Ads บันทึกว่าได้ Lead 1 คน ทุกขั้นตอนต้องทำงานได้สมบูรณ์ ถ้าขาดขั้นใดขั้นหนึ่ง = เสีย Lead

---

=== CARD 10 ===
Q: การทดสอบ Conversion Flow ต้องทำอะไรบ้าง?
A: **(1)** กรอกฟอร์มจริงเหมือนเป็นลูกค้า **(2)** ตรวจว่า Redirect ทำงาน → Thank You Page ขึ้นมา **(3)** เช็คใน Google Ads ว่า Conversion ถูกนับ **(4)** ทดสอบทั้ง **Desktop และ Mobile** **(5)** ให้เพื่อน/ทีมทดสอบด้วย **(6)** เช็ค Page Speed ด้วย **Google PageSpeed Insights** — ถ้าช้ากว่า 3 วินาที อาจเสีย Lead เยอะ

---

=== CARD 11 ===
Q: ทำไมต้องทดสอบบน Mobile?
A: เพราะ **คนส่วนใหญ่ดู Youtube บนมือถือ** ดังนั้นเมื่อเขาคลิกลิงก์จากโฆษณา ก็จะเปิด Capture Page บนมือถือ ถ้า Redirect ไม่ทำงานบนมือถือ หรือเพจโหลดช้าบนมือถือ ก็จะ **เสีย Lead ทันที** แม้บน Desktop จะทำงานได้ปกติก็ตาม ต้องทดสอบทั้งสองแพลตฟอร์มเสมอ

---

=== CARD 12 ===
Q: สรุป 5 ข้อสำคัญจาก YTCAMP-002?
A: **(1) เชื่อม Capture Page → Thank You Page** ผ่าน After Submission Settings ใน Kartra **(2) ใช้ Internal Redirect + Single Opt-in** เพื่อ Flow ลื่นไหล **(3) ติดตั้ง Tracking Pixel 2 จุด** (Conversion Tag + GA Tag) ก่อนปล่อยแคมเปญ **(4) ทดสอบ Flow ทั้งหมด** ทั้ง Desktop และ Mobile **(5) เช็ค Page Speed < 3 วินาที** ด้วย PageSpeed Insights

---

> ทบทวนต่อ: **YTCAMP-003** — Youtube Ads Campaign ตอนที่ 3
> Series: SWP3 Ch19 Youtube Ads Campaign
> PinkCastle Academy © 2026
