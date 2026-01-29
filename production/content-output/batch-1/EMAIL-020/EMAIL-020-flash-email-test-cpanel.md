# Flashcards: ทดลองส่งอีเมลจากระบบ Cpanel

> **Format:** Flashcards (Q&A)
> **Source:** SWP3 - Email Marketing: ทดลองส่งอีเมลจากระบบ Cpanel
> **Total Cards:** 15
> **Production ID:** EMAIL-020-FLASH

---

## Card 1
**Q:** ทำไมต้องทดสอบ Email หลังสร้าง Account?
**A:** เพื่อยืนยันว่าส่ง/รับได้ถูกต้อง และไม่เข้า Spam

---

## Card 2
**Q:** URL สำหรับเข้า Webmail คืออะไร?
**A:** yourdomain.com/webmail หรือ yourdomain.com:2096

---

## Card 3
**Q:** ควรทดสอบส่ง Email ไปยัง Provider ใดบ้าง?
**A:** Gmail, Yahoo, Hotmail (ครอบคลุม major providers)

---

## Card 4
**Q:** SPF ย่อมาจากอะไร?
**A:** Sender Policy Framework - ระบุว่า server ใดมีสิทธิ์ส่ง email ในนามโดเมน

---

## Card 5
**Q:** DKIM ย่อมาจากอะไร?
**A:** DomainKeys Identified Mail - ลายเซ็นดิจิทัลยืนยันว่า email ไม่ถูกแก้ไข

---

## Card 6
**Q:** DMARC ย่อมาจากอะไร?
**A:** Domain-based Message Authentication, Reporting & Conformance

---

## Card 7
**Q:** วิธีดู Email Headers ใน Gmail?
**A:** คลิก 3 dots menu → Show original → ดู Authentication-Results

---

## Card 8
**Q:** Authentication result ที่ดีควรเป็นอย่างไร?
**A:** SPF: Pass, DKIM: Pass, DMARC: Pass (ผ่านทั้ง 3)

---

## Card 9
**Q:** ถ้า Email เข้า Spam ควรทำอย่างไร?
**A:** ตั้งค่า SPF, DKIM, DMARC Records ใน DNS

---

## Card 10
**Q:** ถ้าส่ง Email ไม่ได้ ควรเช็คอะไร?
**A:** SMTP Settings: Server, Port (465/587), SSL/TLS, Authentication

---

## Card 11
**Q:** ถ้ารับ Email ไม่ได้ ควรเช็คอะไร?
**A:** IMAP Settings: Port 993, SSL, Username เป็น full email address

---

## Card 12
**Q:** mail-tester.com ใช้ทำอะไร?
**A:** ทดสอบ Email Deliverability และให้คะแนน spam score

---

## Card 13
**Q:** Email Warm-up คืออะไร?
**A:** การส่ง email ทีละน้อยเพื่อสร้าง reputation ก่อนส่งจำนวนมาก

---

## Card 14
**Q:** Bounce Rate ที่ดีควรเป็นเท่าไหร่?
**A:** น้อยกว่า 2% (ยิ่งต่ำยิ่งดี)

---

## Card 15
**Q:** ควรทดสอบ Email กี่ครั้งก่อนใช้งานจริง?
**A:** อย่างน้อย 3 ครั้ง: ส่งออก, รับเข้า, และ Reply chain

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
