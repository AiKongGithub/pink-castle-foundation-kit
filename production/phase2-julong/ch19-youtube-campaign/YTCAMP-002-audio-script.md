# วิธีเชื่อม Capture Page กับ Thankyou Page — YTCAMP-002
> **Format:** Audio Script (Podcast-style)
> **Source:** SWP3 Ch19 Youtube Ads Campaign ตอนที่ 2
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

## SEGMENT 1: เปิดรายการ (00:00 - 02:00)

**Host A:** สวัสดีครับ กลับมาพบกันอีกครั้งกับ PinkCastle Podcast ซีรีส์ Youtube Ads Campaign ตอนที่ 2 แล้วนะครับ วันนี้เป็นตอนที่ยาวที่สุดเลย เพราะเราจะลงมือทำจริงกัน

**Host B:** ใช่ค่ะ ตอนนี้เราจะมาเรียนรู้วิธีเชื่อม Capture Page กับ Thank You Page ใน Kartra ซึ่งเป็นพื้นฐานที่สำคัญมากก่อนจะไปทำ Youtube Ads ค่ะ

**Host A:** ผมอยากให้ทุกคนเข้าใจว่า Capture Page และ Thank You Page เป็นเหมือนประตูหน้าบ้านกับห้องรับแขกครับ ถ้าประตูเปิดไม่ได้ หรือเปิดแล้วไปผิดห้อง ลูกค้าก็หายไปเลย

**Host B:** เปรียบเทียบได้ดีมากค่ะ วันนี้เราจะสอนแบบ Step-by-step เลยนะคะ ตั้งแต่สร้างเพจ ตั้งค่า Redirect เชื่อมทั้งสองหน้าเข้าด้วยกัน ติดตั้ง Tracking Pixel และทดสอบ Flow ทั้งหมด

---

## SEGMENT 2: Kartra Page Linking — การเชื่อมเพจใน Kartra (02:00 - 05:00)

**Host A:** เริ่มจากหลักการก่อนครับ ใน Kartra เราจะมีหน้าเพจ 2 หน้าที่ต้องเชื่อมกัน หน้าแรกคือ Capture Page ที่มีฟอร์มกรอกข้อมูล หน้าที่สองคือ Thank You Page ที่จะแสดงหลังจากคนกรอกฟอร์มเสร็จ

**Host B:** วิธีเชื่อมใน Kartra ไม่ยากเลยค่ะ เข้าไปที่ Page Builder เลือก Capture Page ของเรา แล้วคลิกที่ Form Element จากนั้นไปที่ After Submission Settings

**Host A:** ตรงนี้จะมีตัวเลือกให้เลือกว่าหลังจากกรอกฟอร์มแล้วจะให้ไปที่ไหน ให้เลือก Redirect to Page แล้วเลือก Thank You Page ที่เราสร้างไว้ครับ

**Host B:** สิ่งที่ต้องระวังคือ URL ต้องถูกต้องนะคะ ถ้าใช้ Custom Domain ก็ต้องตั้งค่า Domain ให้ตรงกัน ไม่งั้น Redirect อาจจะไม่ทำงาน

**Host A:** อีกเรื่องที่สำคัญคือ Opt-in Confirmation ครับ ในหน้า Settings ของฟอร์ม เราสามารถเลือกได้ว่าจะให้ส่ง Confirmation Email ก่อนหรือไม่ สำหรับ Youtube Ads Campaign แนะนำให้ใช้ Single Opt-in ครับ เพื่อให้ Flow ลื่นไหล

---

## SEGMENT 3: Redirect Setup — ตั้งค่า Redirect (05:00 - 08:00)

**Host B:** มาพูดถึงเรื่อง Redirect ให้ละเอียดขึ้นนะคะ Redirect คือการส่งต่อผู้ใช้จากหน้าหนึ่งไปอีกหน้าหนึ่งโดยอัตโนมัติ

**Host A:** ใน Kartra มี Redirect แบบหลักๆ 2 แบบครับ แบบแรกคือ Internal Redirect คือส่งไปยังหน้าอื่นภายใน Kartra เดียวกัน แบบนี้ง่ายที่สุด แค่เลือกหน้าจาก Dropdown

**Host B:** แบบที่สองคือ External Redirect ค่ะ คือส่งไปยัง URL ภายนอก เช่น เว็บไซต์ของเราเอง แบบนี้ต้องใส่ Full URL ให้ถูกต้อง

**Host A:** สำหรับ Youtube Ads Campaign แนะนำให้ใช้ Internal Redirect ครับ เพราะง่ายกว่าและเร็วกว่า แต่ถ้าจำเป็นต้อง Redirect ไปเว็บนอก ก็ต้องมั่นใจว่า URL ถูกต้อง 100%

**Host B:** เรื่อง Redirect Speed ก็สำคัญมากนะคะ ถ้าเพจโหลดช้า คนอาจจะปิดหน้าไปก่อน ยิ่ง Redirect หลายชั้นยิ่งช้า ควร Redirect ครั้งเดียวจาก Capture Page ไป Thank You Page เลย

**Host A:** ถูกต้องครับ และอย่าลืม Test ด้วยมือถือด้วยนะครับ เพราะคนส่วนใหญ่จะเข้ามาจาก Youtube บนมือถือ ถ้า Redirect ไม่ทำงานบนมือถือก็เสีย Lead ไปเลย

---

## SEGMENT 4: Tracking Pixels — ติดตั้ง Pixel (08:00 - 11:00)

**Host B:** มาถึงเรื่อง Tracking Pixels กันค่ะ ส่วนนี้สำคัญมากเพราะเป็นสิ่งที่ทำให้เราวัดผล Campaign ได้

**Host A:** Tracking Pixel คือโค้ดเล็กๆ ที่เราฝังไว้ในหน้าเว็บครับ เมื่อมีคนเข้ามาถึงหน้านั้น Pixel จะส่งสัญญาณกลับไปบอก Google Ads ว่า "มีคนมาถึงหน้านี้แล้วนะ"

**Host B:** สำหรับ Youtube Ads Campaign เราต้องติดตั้ง Pixel อย่างน้อย 2 จุดค่ะ จุดแรกคือ Google Ads Conversion Tag บน Thank You Page เพื่อนับจำนวน Conversion

**Host A:** จุดที่สองคือ Google Analytics Tag ทั้งบน Capture Page และ Thank You Page ครับ เพื่อดูพฤติกรรมผู้ใช้ เช่น มีคนเข้า Capture Page กี่คน กรอกฟอร์มกี่คน อัตรา Conversion เป็นเท่าไหร่

**Host B:** วิธีติดตั้งใน Kartra ไม่ยากเลยค่ะ เข้าไปที่ Page Settings เลือก Tracking Code แล้ววาง Pixel Code ตรงนี้ได้เลย Kartra มีช่องให้ใส่ทั้ง Header Code และ Body Code

**Host A:** เคล็ดลับคือ ติดตั้ง Pixel ก่อนปล่อยแคมเปญ แล้วเข้าไปเช็คใน Google Tag Assistant ว่า Pixel ทำงานถูกต้องหรือไม่ครับ อย่ารอจนปล่อย Ads ไปแล้วค่อยมาเช็ค

---

## SEGMENT 5: Conversion Flow — ทดสอบ Flow ทั้งหมด (11:00 - 13:30)

**Host B:** ขั้นตอนสุดท้ายที่สำคัญมากคือการทดสอบ Flow ทั้งหมดค่ะ ก่อนปล่อยแคมเปญจริง ต้องทดสอบด้วยตัวเองก่อนเสมอ

**Host A:** Conversion Flow ที่สมบูรณ์จะเป็นแบบนี้ครับ คนดูโฆษณาบน Youtube → คลิกลิงก์ → มาถึง Capture Page → กรอกฟอร์ม → Redirect ไป Thank You Page → Pixel ส่งสัญญาณ Conversion → Google Ads บันทึกว่าได้ Lead 1 คน

**Host B:** การทดสอบให้ทำทุกขั้นตอนเหมือนเป็นลูกค้าจริงค่ะ กรอกฟอร์มจริง ดูว่า Redirect ทำงานไหม Thank You Page ขึ้นมาหรือเปล่า และเช็คใน Google Ads ว่า Conversion ถูกนับไหม

**Host A:** ทดสอบทั้งบน Desktop และ Mobile นะครับ และถ้าเป็นไปได้ ลองให้เพื่อนหรือคนในทีมทดสอบด้วย เพราะบางครั้งเราอาจมองข้ามบางอย่างไป

**Host B:** อีกเรื่องคือทดสอบ Speed ค่ะ ใช้ Google PageSpeed Insights เช็คว่าทั้ง Capture Page และ Thank You Page โหลดเร็วพอไหม ถ้าช้ากว่า 3 วินาที อาจเสีย Lead ไปเยอะ

**Host A:** สรุปสำหรับตอนนี้ เราได้เรียนรู้วิธีเชื่อม Capture Page กับ Thank You Page ใน Kartra ตั้งค่า Redirect ติดตั้ง Tracking Pixel และทดสอบ Conversion Flow ทั้งหมด ในตอนหน้าเราจะเข้าสู่เรื่อง Youtube Ads โดยตรงแล้วครับ

**Host B:** อย่าลืมทำตามทุกขั้นตอนก่อนไปตอนต่อไปนะคะ แล้วพบกันค่ะ สวัสดีค่ะ

**Host A:** สวัสดีครับ

---

*Word count: ~800 | Segments: 5 | Estimated read time: 6 minutes*
