# Google กับ Kartra ทำงานร่วมกัน — YTOPT-010 Audio Script
> **Format:** Audio Script (Podcast-style)
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 10
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:06:52

---

## SEGMENT 1: เปิดรายการ (00:00 - 01:30)

**Host A:** สวัสดีครับทุกคน กลับมาพบกันอีกครั้งกับ PinkCastle Podcast ตอนที่แล้วเราพูดเรื่อง Set Conversion ไปแล้ว วันนี้เราจะมาต่อยอดกันครับ เรื่อง Google กับ Kartra ทำงานร่วมกัน หลายคนใช้ Kartra สร้าง Landing Page แต่ยังไม่ได้เชื่อม Google Ads เข้าไป ทำให้ไม่รู้ว่าคนที่คลิกโฆษณามาแล้วทำอะไรต่อบน Kartra

**Host B:** ใช่ค่ะ นี่คือปัญหาที่พบบ่อยมาก คนลงโฆษณา Google Ads แล้วส่งคนไปที่ Kartra Landing Page แต่ไม่ได้ใส่ Tracking Code เลย ทำให้ Google Ads ไม่รู้ว่ามีคนกรอกฟอร์มหรือซื้อสินค้าจริงหรือเปล่า ข้อมูลขาดหาย Optimize แคมเปญได้ยากมากค่ะ

**Host A:** ถูกต้องครับ วันนี้เราจะครอบคลุมตั้งแต่ทำไมต้องเชื่อม วิธีใส่ Google Tag ใน Kartra ขั้นตอน Conversion Tracking Flow เปรียบเทียบ Google Tag Manager กับ Global Site Tag วิธีตรวจสอบว่า Tag ทำงาน และข้อดีของการเชื่อมระบบทั้งสองเข้าด้วยกันครับ

---

## SEGMENT 2: ทำไมต้องเชื่อม Google Ads กับ Kartra (01:30 - 03:00)

**Host B:** เริ่มจากคำถามพื้นฐานก่อนค่ะ ทำไมเราต้องเชื่อม Google Ads กับ Kartra ให้ทำงานร่วมกัน คำตอบง่ายๆ คือเพื่อ วัด Conversion จริง ค่ะ เราต้องรู้ว่าคนที่คลิกโฆษณาแล้วกรอกฟอร์มหรือซื้อจริงหรือไม่ ถ้าไม่เชื่อมกัน Google Ads จะเห็นแค่ว่ามีคนคลิก แต่ไม่รู้ว่าเกิดอะไรขึ้นหลังจากนั้น

**Host A:** เปรียบเทียบให้เห็นภาพครับ เหมือนเราเปิดร้านค้า ส่งใบปลิวออกไป มีคนหยิบใบปลิวไปเยอะ แต่เราไม่รู้ว่าคนที่หยิบใบปลิวมาซื้อของที่ร้านจริงกี่คน ถ้าเชื่อม Google Ads กับ Kartra ก็เหมือนมีคนนับให้ว่าลูกค้าที่มาจากใบปลิวซื้อกี่คน เท่าไร ทำให้ตัดสินใจได้ว่าใบปลิวนี้คุ้มค่าหรือไม่

**Host B:** และยิ่งไปกว่านั้นค่ะ เมื่อ Google Ads ได้ข้อมูล Conversion จาก Kartra ระบบ Smart Bidding ของ Google จะสามารถปรับราคาประมูลให้อัตโนมัติ เน้นแสดงโฆษณาให้กลุ่มคนที่มีแนวโน้มจะ Convert สูง ทำให้ค่าโฆษณาต่อ Conversion ลดลงเรื่อยๆ ค่ะ

---

## SEGMENT 3: วิธีใส่ Google Tag ใน Kartra (03:00 - 04:30)

**Host A:** มาดูวิธีทำจริงกันครับ ขั้นตอนการใส่ Google Tag ใน Kartra ไม่ยากเลย เข้า Kartra ไปที่หน้า Page ที่ต้องการ คลิก Page Settings จากนั้นมองหาส่วน Tracking Code จะมีช่องให้วาง Code ในส่วน Header ก็คัดลอก Google Tag จาก Google Ads มาวางตรงนี้เลยครับ

**Host B:** ขั้นตอนฝั่ง Google Ads ค่ะ ก่อนอื่นเราต้องไปสร้าง Conversion Action ใน Google Ads ก่อน ซึ่งตอนที่แล้วเราเรียนไปแล้ว จากนั้น Google จะให้ Tag มา 2 ส่วน ส่วนแรกคือ Global Site Tag ที่ต้องวางทุกหน้า และส่วนที่สองคือ Event Snippet ที่วางเฉพาะ Thank You Page ค่ะ

**Host A:** ที่สำคัญมากครับ Conversion Tracking Flow จะเป็นแบบนี้ คนดูโฆษณาบน YouTube หรือ Google Search แล้วคลิก จากนั้นเข้ามาที่ Kartra Landing Page ที่เราสร้างไว้ พอกรอกฟอร์มหรือซื้อสินค้าเสร็จ ก็จะไปถึง Thank You Page ซึ่งมี Conversion Tag ติดอยู่ Tag ก็จะยิงข้อมูลกลับไปที่ Google Ads ว่าเกิด Conversion แล้วครับ

**Host B:** Flow นี้สำคัญมากค่ะ ถ้าขาดตรงไหนตรงหนึ่ง Conversion จะไม่ถูกบันทึก เช่น ถ้าลืมใส่ Tag บน Thank You Page หรือ Thank You Page ไม่ได้อยู่บน Kartra แต่อยู่ที่อื่น ก็จะทำให้ข้อมูลหายค่ะ

---

## SEGMENT 4: GTM vs Global Site Tag และการตรวจสอบ (04:30 - 06:00)

**Host A:** ตอนนี้หลายคนอาจสงสัยว่า ควรใช้ Google Tag Manager หรือ Global Site Tag ดี ผมอธิบายง่ายๆ ครับ Global Site Tag คือการวางโค้ดลงใน Kartra โดยตรง ข้อดีคือง่าย ทำได้เร็ว เหมาะกับมือใหม่ที่มี Tag แค่ 1-2 ตัว

**Host B:** ส่วน Google Tag Manager หรือ GTM ค่ะ จะยืดหยุ่นกว่ามาก เพราะเราวาง GTM Container Code ลงใน Kartra แค่ครั้งเดียว จากนั้นจัดการ Tag ทั้งหมดผ่าน GTM Dashboard ได้เลย ไม่ว่าจะเพิ่ม Google Ads Tag, Facebook Pixel, TikTok Pixel หรืออะไรก็ตาม ไม่ต้องกลับไปแก้ Code ใน Kartra อีก เหมาะกับคนที่ใช้หลายแพลตฟอร์มโฆษณาค่ะ

**Host A:** พอใส่ Tag เสร็จแล้ว ต้องตรวจสอบด้วยนะครับ วิธีง่ายที่สุดคือใช้ Google Tag Assistant ซึ่งเป็น Chrome Extension ฟรี ติดตั้งแล้วเข้าไปที่ Kartra Landing Page ของเรา Tag Assistant จะแสดงว่ามี Tag อะไรติดอยู่บ้าง ยิงถูกต้องหรือไม่ ถ้าเห็นเครื่องหมายถูกสีเขียว แปลว่า Tag ทำงานถูกต้องครับ

**Host B:** อีกวิธีหนึ่งคือเข้าไปที่ Google Ads ดูสถานะ Conversion Action ค่ะ ถ้าแสดงเป็น Recording แปลว่าทุกอย่างทำงานปกติ ถ้าเป็น Inactive ให้กลับไปตรวจ Tag ใน Kartra ใหม่ค่ะ

---

## SEGMENT 5: ข้อดีของการเชื่อมและปิดรายการ (06:00 - 06:52)

**Host A:** สรุปข้อดีของการเชื่อม Google กับ Kartra ครับ ข้อแรก ข้อมูล Conversion แม่นยำ รู้จริงว่าคนจากโฆษณากรอกฟอร์มหรือซื้อกี่คน ข้อสอง Optimize Campaign ได้ดีขึ้น เพราะมีข้อมูลจริงให้ปรับปรุง ข้อสาม ใช้ Smart Bidding ได้ Google จะปรับราคาประมูลให้อัตโนมัติตาม Conversion data

**Host B:** เพิ่มเติมอีกค่ะ ข้อสี่ รู้ว่าโฆษณาชุดไหนคุ้มค่า เพราะเห็น Conversion ระดับ Ad Group และ Ad ข้อห้า ลดการเสียเงินโดยเปล่าประโยชน์ เพราะหยุดโฆษณาที่ไม่ได้ Conversion ได้ทันที และข้อหก ข้อมูลสะสมยิ่งมาก Google ยิ่ง Optimize ดีขึ้นเรื่อยๆ ค่ะ

**Host A:** ในตอนต่อไปเราจะไปเรื่องลงโฆษณา Google Ads ตอนที่ 2 ซึ่งจะลงลึกเรื่องการตั้งค่าแคมเปญจริงครับ อย่าลืมกด Subscribe และกดกระดิ่ง แล้วพบกันตอนหน้านะครับ สวัสดีครับ

**Host B:** สวัสดีค่ะ

---

> ทบทวนต่อ: **YTOPT-012** — ลงโฆษณา Google Ads ตอนที่ 2
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*Word count: ~900 | Segments: 5 | Estimated read time: 7 minutes*
