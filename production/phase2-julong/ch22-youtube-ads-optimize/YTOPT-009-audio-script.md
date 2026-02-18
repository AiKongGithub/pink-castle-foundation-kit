# Set Conversion — YTOPT-009 Audio Script
> **Format:** Audio Script (Podcast-style)
> **Source:** SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads ตอนที่ 9
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18 | **Duration:** 0:11:11

---

## SEGMENT 1: เปิดรายการ (00:00 - 02:00)

**Host A:** สวัสดีครับทุกคน กลับมาพบกันอีกครั้งกับ PinkCastle Podcast ตอนที่แล้วเราพูดเรื่องการเริ่มต้นทำแคมเปญใหม่ไปแล้ว วันนี้เราจะมาเรียนรู้เรื่องที่สำคัญมากๆ เรื่อง Set Conversion ครับ ถ้าไม่ตั้ง Conversion โฆษณาของเราก็เหมือนยิงปืนโดยไม่รู้ว่าถูกเป้าหรือเปล่า

**Host B:** ใช่ค่ะ Conversion คือหัวใจสำคัญของการวัดผลโฆษณา ถ้าเราไม่ตั้ง Conversion Tracking เราจะไม่รู้เลยว่าคนที่เห็นโฆษณาแล้วทำอะไรต่อ กรอกฟอร์มหรือเปล่า ซื้อของหรือเปล่า สมัครสมาชิกหรือเปล่า ข้อมูลเหล่านี้สำคัญมากต่อการตัดสินใจค่ะ

**Host A:** ถูกต้องครับ วันนี้เราจะครอบคลุมตั้งแต่ Conversion คืออะไร มีกี่ประเภท วิธีตั้งค่าใน Google Ads เรื่อง Conversion Window เรื่อง Attribution Model การติดตั้ง Conversion Tag ไปจนถึงการตรวจสอบว่า Conversion ทำงานถูกต้องหรือไม่ครับ

---

## SEGMENT 2: Conversion คืออะไร และมีกี่ประเภท (02:00 - 04:00)

**Host B:** เริ่มจากพื้นฐานก่อนค่ะ Conversion คือการกระทำที่เราต้องการให้ลูกค้าทำหลังจากเห็นโฆษณา อาจจะเป็นการกรอกฟอร์มสมัครสมาชิก การซื้อสินค้า การโทรหาเรา หรือการดาวน์โหลดแอป แล้วแต่เป้าหมายของธุรกิจเราค่ะ

**Host A:** ใน Google Ads แบ่ง Conversion เป็น 4 ประเภทหลักครับ ประเภทแรกคือ Website Actions เช่น กรอกฟอร์ม สั่งซื้อสินค้า สมัครสมาชิก หรือคลิกปุ่มบนเว็บไซต์ ประเภทที่สองคือ Phone Calls เช่น โทรหาร้านค้าผ่านเบอร์ที่แสดงในโฆษณา

**Host B:** ประเภทที่สามคือ App Installs ค่ะ สำหรับธุรกิจที่มีแอปและต้องการวัดว่าโฆษณานำไปสู่การติดตั้งแอปกี่ครั้ง และประเภทที่สี่คือ Import หรือ Offline Conversions ค่ะ เหมาะกับธุรกิจที่ Conversion เกิดขึ้นนอกโลกออนไลน์ เช่น ลูกค้าเห็นโฆษณาแล้วมาซื้อที่หน้าร้าน เราสามารถ Import ข้อมูลเข้ามาได้

**Host A:** สำหรับผู้ประกอบการไทยส่วนใหญ่ที่ทำ Landing Page หรือ Sales Funnel ประเภทที่ใช้บ่อยสุดคือ Website Actions ครับ โดยเฉพาะการกรอกฟอร์ม Lead Generation และการสั่งซื้อสินค้าบน Thank You Page

---

## SEGMENT 3: วิธีตั้ง Conversion ใน Google Ads (04:00 - 06:00)

**Host B:** มาดูขั้นตอนการตั้งค่ากันค่ะ เข้า Google Ads เลือกเมนู Tools ด้านบน จากนั้นไปที่ Measurement แล้วคลิก Conversions จะเห็นปุ่ม New Conversion Action ให้คลิกเลยค่ะ

**Host A:** พอคลิกแล้วจะมีให้เลือก 4 ประเภทที่เราพูดไปครับ Website, Phone Calls, App, Import ถ้าเลือก Website ก็ใส่ URL เว็บไซต์ของเรา Google จะสแกนดูว่ามี Tag อะไรอยู่บ้าง จากนั้นเราตั้งชื่อ Conversion Action เลือก Category เช่น Lead, Purchase, Sign-up

**Host B:** ขั้นตอนถัดมาสำคัญมากค่ะ คือการกำหนด Value ว่า Conversion แต่ละครั้งมีมูลค่าเท่าไร ถ้าเป็น E-commerce ใส่ราคาสินค้าจริงได้เลย แต่ถ้าเป็น Lead Generation อาจจะตั้งมูลค่าเฉลี่ยของ Lead หนึ่งราย เช่น Lead หนึ่งคนมีโอกาสปิดการขายได้ 500 บาท ก็ตั้ง Value เป็น 500

**Host A:** อีกอันที่ต้องตั้งคือเรื่อง Count ครับ มีให้เลือก Every กับ One ถ้าเลือก Every หมายความว่านับทุกครั้งที่เกิด Conversion เหมาะกับ E-commerce เพราะลูกค้าคนเดียวอาจซื้อหลายครั้ง แต่ถ้าเลือก One หมายถึงนับแค่ครั้งเดียวต่อคน เหมาะกับ Lead Generation ที่เราสนใจแค่ว่าลูกค้าสมัครหรือยัง

---

## SEGMENT 4: Conversion Window และ Attribution Model (06:00 - 08:30)

**Host B:** มาเรื่อง Conversion Window ค่ะ คือการกำหนดระยะเวลาที่จะนับว่าเป็น Conversion หมายความว่าถ้าลูกค้าเห็นโฆษณาวันนี้ แต่ไปกรอกฟอร์มอีก 15 วันถัดมา จะนับเป็น Conversion หรือเปล่า ขึ้นอยู่กับที่เราตั้งค่า

**Host A:** ตัวเลือกมีตั้งแต่ 7 วัน 30 วัน ไปจนถึง 90 วันครับ ค่าเริ่มต้นคือ 30 วัน สำหรับสินค้าที่ตัดสินใจเร็ว เช่น ของราคาถูก อาจตั้ง 7 วันก็พอ แต่สินค้าที่ต้องใช้เวลาตัดสินใจนาน เช่น คอร์สเรียนราคาแพง อสังหาริมทรัพย์ อาจตั้ง 60-90 วันครับ

**Host B:** ถัดมาคือ Attribution Model ค่ะ เป็นการกำหนดว่าจะให้เครดิต Conversion กับจุดสัมผัสไหนของลูกค้า ตัวเลือกหลักๆ มี Last Click ที่ให้เครดิตทั้งหมดกับคลิกสุดท้าย First Click ที่ให้เครดิตกับคลิกแรก Linear ที่แบ่งเครดิตเท่ากันทุกจุดสัมผัส Time Decay ที่ให้เครดิตมากกว่ากับจุดสัมผัสที่ใกล้ Conversion มากกว่า และ Data-driven ที่ Google ใช้ Machine Learning คำนวณให้

**Host A:** สำหรับผู้เริ่มต้น แนะนำ Last Click ครับ เพราะเข้าใจง่ายที่สุด แต่ถ้ามีข้อมูลมากพอ Data-driven เป็นตัวเลือกที่ดีที่สุดเพราะ Google จะวิเคราะห์ให้ว่าจุดไหนมีผลต่อ Conversion จริงๆ ครับ

---

## SEGMENT 5: ติดตั้ง Conversion Tag (08:30 - 10:00)

**Host B:** พอตั้งค่า Conversion Action เสร็จแล้ว ขั้นตอนถัดไปคือการติดตั้ง Conversion Tag บนเว็บไซต์ค่ะ มี 2 วิธีหลักๆ วิธีแรกคือผ่าน Google Tag Manager ซึ่งแนะนำมากที่สุดเพราะจัดการง่าย ไม่ต้องแก้โค้ดเว็บไซต์ตรงๆ วิธีที่สองคือวาง Global Site Tag ลงในโค้ดเว็บไซต์โดยตรง

**Host A:** หลักการสำคัญคือ Conversion Tag ต้องวางบน Thank You Page หรือหน้ายืนยันการกระทำครับ เช่น ถ้า Conversion คือการกรอกฟอร์ม Tag ต้องอยู่บนหน้าที่แสดงหลังจากกรอกฟอร์มเสร็จ ถ้า Conversion คือการซื้อสินค้า Tag ต้องอยู่บนหน้า Order Confirmation ห้ามวางบนหน้าแรกหรือหน้าสินค้า เพราะจะนับผิดครับ

**Host B:** สำหรับ Google Tag Manager ขั้นตอนคือสร้าง Tag ใหม่ เลือก Google Ads Conversion Tracking ใส่ Conversion ID และ Conversion Label ที่ได้จาก Google Ads จากนั้นตั้ง Trigger เป็น Thank You Page URL เช่น Page View เฉพาะหน้า /thank-you เท่านั้นค่ะ

---

## SEGMENT 6: ตรวจสอบ Conversion และปิดรายการ (10:00 - 11:11)

**Host A:** ขั้นตอนสุดท้ายที่สำคัญมากคือการตรวจสอบว่า Conversion ทำงานถูกต้องหรือไม่ครับ ใน Google Ads ไปที่หน้า Conversions จะเห็น Status ของแต่ละ Conversion Action มี 3 สถานะหลักคือ Recording หมายถึงทำงานปกติ กำลังบันทึกข้อมูล No Recent Conversions หมายถึง Tag ติดตั้งถูกต้องแต่ยังไม่มี Conversion เกิดขึ้น อาจเป็นเพราะยังไม่มีคนกรอกฟอร์ม และ Inactive หมายถึงมีปัญหา Tag อาจไม่ทำงาน

**Host B:** ถ้าเจอสถานะ Inactive ให้ตรวจสอบหลายจุดค่ะ หนึ่ง ตรวจว่า Tag วางถูกหน้าหรือเปล่า สอง ใช้ Google Tag Assistant ตรวจสอบว่า Tag ยิงถูกต้อง สาม ลองทำ Test Conversion ด้วยตัวเอง เข้าเว็บ กรอกฟอร์ม แล้วดูว่า Conversion ถูกนับหรือไม่ สี่ ตรวจว่า Conversion ID และ Label ตรงกับที่ตั้งใน Google Ads

**Host A:** สรุปสำหรับตอนนี้ครับ หนึ่ง Conversion คือการกระทำที่ต้องการวัดผล สอง มี 4 ประเภท Website Phone App Import สาม ตั้งค่าผ่าน Tools Measurement Conversions สี่ เลือก Conversion Window และ Attribution Model ให้เหมาะกับธุรกิจ ห้า ติดตั้ง Tag บน Thank You Page หก ตรวจสอบสถานะให้เป็น Recording

**Host B:** ในตอนต่อไปเราจะไปเรื่อง Google กับ Kartra ทำงานร่วมกัน อย่าลืมกด Subscribe และกดกระดิ่ง แล้วพบกันตอนหน้านะคะ สวัสดีค่ะ

**Host A:** สวัสดีครับ

---

> ทบทวนต่อ: **YTOPT-010** — Google กับ Kartra ทำงานร่วมกัน
> Series: SWP3 Ch22 วิธีปรับแต่งแคมเปญ Youtube Ads
> PinkCastle Academy © 2026

---

*Word count: ~1,100 | Segments: 6 | Estimated read time: 8 minutes*
