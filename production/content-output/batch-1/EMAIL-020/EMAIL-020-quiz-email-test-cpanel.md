# Quiz: ทดลองส่งอีเมลจากระบบ Cpanel

> **Format:** Multiple Choice Quiz
> **Source:** SWP3 - Email Marketing: ทดลองส่งอีเมลจากระบบ Cpanel
> **Total Questions:** 10
> **Production ID:** EMAIL-020-QUIZ

---

## Question 1

ทำไมต้องทดสอบ Email หลังจากสร้าง Account?

- A) เพราะ Hosting บังคับ
- B) **เพื่อยืนยันว่าทำงานถูกต้องและไม่เข้า Spam** ✓
- C) เพื่อเพิ่ม Quota
- D) ไม่จำเป็นต้องทดสอบ

**Explanation:** การทดสอบช่วยยืนยันว่า Email ทำงานถูกต้องและตั้งค่า Authentication ถูกต้อง

---

## Question 2

URL ใดใช้เข้า Webmail?

- A) yourdomain.com/email
- B) **yourdomain.com/webmail** ✓
- C) yourdomain.com/mail
- D) yourdomain.com/inbox

**Explanation:** Webmail เข้าได้ที่ /webmail หรือ port 2096

---

## Question 3

ควรทดสอบส่ง Email ไปยัง Provider ใดบ้าง?

- A) Gmail อย่างเดียวพอ
- B) ส่งหาตัวเองอย่างเดียว
- C) **Gmail, Yahoo, Hotmail** ✓
- D) ไม่ต้องทดสอบ

**Explanation:** ควรทดสอบกับหลาย providers เพราะแต่ละที่มี spam filter ต่างกัน

---

## Question 4

SPF Record ใช้ทำอะไร?

- A) เข้ารหัส email
- B) **ระบุว่า server ใดมีสิทธิ์ส่ง email ในนามโดเมน** ✓
- C) เก็บ backup email
- D) เพิ่มความเร็วในการส่ง

**Explanation:** SPF = Sender Policy Framework กำหนดว่า IP ใดมีสิทธิ์ส่ง email ของโดเมน

---

## Question 5

วิธีดู Email Headers ใน Gmail คือ?

- A) คลิกขวาที่ email
- B) **คลิก 3 dots → Show original** ✓
- C) กด Ctrl+H
- D) ไปที่ Settings

**Explanation:** ใน Gmail ให้คลิก 3 dots menu แล้วเลือก "Show original"

---

## Question 6

Authentication Results ที่ดีควรเป็นอย่างไร?

- A) SPF: Fail, DKIM: Pass
- B) SPF: Pass, DKIM: Fail
- C) **SPF: Pass, DKIM: Pass, DMARC: Pass** ✓
- D) ไม่มีผลอะไร

**Explanation:** ต้อง Pass ทั้ง 3 เพื่อ Deliverability ที่ดีที่สุด

---

## Question 7

ถ้า Email เข้า Spam ควรทำอย่างไร?

- A) ส่งซ้ำหลายๆ ครั้ง
- B) เปลี่ยน Subject line
- C) **ตั้งค่า SPF, DKIM, DMARC** ✓
- D) ใช้ UPPERCASE

**Explanation:** การตั้งค่า Email Authentication ช่วยให้ email ไม่เข้า Spam

---

## Question 8

Port ใดใช้สำหรับ SMTP SSL?

- A) 993
- B) 143
- C) **465** ✓
- D) 110

**Explanation:** SMTP SSL ใช้ port 465 (หรือ 587 สำหรับ STARTTLS)

---

## Question 9

mail-tester.com ใช้ทำอะไร?

- A) สร้าง Email Account
- B) ส่ง Email ฟรี
- C) **ทดสอบ Spam Score และ Deliverability** ✓
- D) Block Spam

**Explanation:** mail-tester.com ช่วยตรวจสอบว่า email มี spam score เท่าไหร่

---

## Question 10

Bounce Rate ที่ดีควรเป็นเท่าไหร่?

- A) 10%
- B) 5%
- C) **น้อยกว่า 2%** ✓
- D) ไม่สำคัญ

**Explanation:** Bounce rate ควรต่ำกว่า 2% เพื่อรักษา sender reputation

---

## Score Interpretation

- 9-10: Excellent! พร้อมทดสอบ Email
- 7-8: Good! ทบทวนเพิ่มเติม
- 5-6: Fair! ควรดู content ซ้ำ
- 0-4: Need more study!

---

*Production: จูล่ง (Claude Code) | Pink Castle Content Production*
