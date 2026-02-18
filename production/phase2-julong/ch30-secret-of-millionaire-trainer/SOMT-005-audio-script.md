# วิธี Deploy Membership System — SOMT-005
> **Format:** Audio Script (Podcast-Style)
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 5
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

## SEGMENT 1: เปิดตัว — ถึงเวลา Deploy!

**Host A:** สวัสดีครับผู้ฟังทุกท่าน วันนี้เป็นตอนสุดท้ายของซีรีส์ Secret Of Millionaire Trainer ครับ ตอนนี้เป็นตอนพิเศษเพราะเราจะมาลงมือทำจริง — Deploy Membership System บน Kartra!

**Host B:** ใช่ค่ะ ตอนนี้สั้นแต่เข้มข้น เหมือน Quick Start Guide ที่จะพาคุณจาก "ยังไม่มีอะไร" ไปเป็น "Membership พร้อมใช้งาน" ใน 7 นาทีค่ะ

**Host A:** เนื้อหาจะเน้น Step-by-Step เลยครับ ทำตามทีละขั้น ครอบคลุม Technical Setup, Domain Configuration, SSL Setup และ Basic Settings ที่จำเป็น

**Host B:** พร้อมแล้วก็เริ่มเลยค่ะ!

---

## SEGMENT 2: ขั้นตอนการ Deploy บน Kartra

**Host A:** มาเริ่มกันเลยครับ ขั้นตอนการ Deploy Membership System บน Kartra มีทั้งหมด 6 ขั้นตอนหลัก

**ขั้นตอนที่ 1: สร้าง Membership Portal**

**Host B:** เข้า Kartra Dashboard ไปที่เมนู "Memberships" แล้วกด "New Membership" ค่ะ ตั้งชื่อ Membership ของคุณ เลือก Template (หรือสร้างจากศูนย์) ใส่ Description และ Welcome Message

**Host A:** เลือก Template ที่ดีจะช่วยประหยัดเวลามากครับ Kartra มี Template สำเร็จรูปหลายแบบ ทั้ง Modern, Classic, Sidebar Navigation เลือกที่เหมาะกับ Brand ของคุณ

**ขั้นตอนที่ 2: ตั้งค่า Membership Levels**

**Host A:** หลังจากสร้าง Portal แล้ว ให้สร้าง Levels ครับ กด "Add Level" สร้าง Silver Level และ Gold Level ตั้งค่าว่าแต่ละ Level เข้าถึง Content อะไรได้บ้าง

**Host B:** สำคัญค่ะ — ตั้ง Access Rules ให้ถูกต้อง Silver เข้าได้เฉพาะ Category ที่กำหนด Gold เข้าได้ทุก Category สามารถตั้ง Drip Schedule ว่า Content ไหนเปิดเมื่อไหร่

**ขั้นตอนที่ 3: Domain Configuration**

**Host B:** ถ้าคุณมี Custom Domain (เช่น members.yourbrand.com) ให้เข้า "My Domains" ใน Kartra ค่ะ เพิ่ม Domain ตั้งค่า DNS Record ที่ Domain Registrar ชี้ CNAME ไปที่ Kartra

**Host A:** ถ้าไม่มี Custom Domain ก็ใช้ Subdomain ของ Kartra ได้ครับ เช่น yourbrand.kartra.com ใช้งานได้เลยโดยไม่ต้องตั้งค่า DNS

**ขั้นตอนที่ 4: SSL Setup**

**Host A:** SSL สำคัญมากครับ เพราะทำให้เว็บไซต์เป็น HTTPS (มีกุญแจล็อคในแถบ URL) สร้างความเชื่อมั่นให้ลูกค้าและจำเป็นสำหรับการรับ Payment

**Host B:** Kartra มี SSL ฟรีให้ค่ะ แค่เปิดใช้งานใน Domain Settings กด "Enable SSL" แล้วรอสักครู่ ระบบจะ provision SSL Certificate ให้อัตโนมัติ ใช้เวลาไม่เกิน 24 ชั่วโมง

---

## SEGMENT 3: Basic Settings และ Go Live

**ขั้นตอนที่ 5: Payment Setup**

**Host B:** เข้า "My Integrations" เชื่อมต่อ Stripe หรือ PayPal ค่ะ ใส่ API Keys จากบัญชี Stripe/PayPal ของคุณ ทดสอบด้วย Test Mode ก่อน ตรวจสอบว่า Recurring Billing ทำงานถูกต้อง

**Host A:** อย่าลืมสร้าง Products สำหรับแต่ละ Level ครับ Silver Product ราคา 990 บาท/เดือน, Gold Product ราคา 2,990 บาท/เดือน เชื่อมต่อ Product กับ Membership Level

**ขั้นตอนที่ 6: ทดสอบและ Go Live**

**Host A:** ขั้นตอนสุดท้ายแต่สำคัญที่สุดครับ — ทดสอบทุกอย่าง!

**Host B:** Checklist การทดสอบค่ะ:
1. ทดสอบ Signup Flow — สมัครสมาชิกได้ไหม?
2. ทดสอบ Payment — ชำระเงินได้ไหม? (ใช้ Test Card)
3. ทดสอบ Access Control — Silver เข้าถึง Gold Content ไม่ได้ใช่ไหม?
4. ทดสอบ Content Dripping — เนื้อหาเปิดตามตารางไหม?
5. ทดสอบ Welcome Email — สมาชิกใหม่ได้รับ Email ไหม?
6. ทดสอบ Cancellation — Cancel แล้วเข้าถึง Content ไม่ได้ใช่ไหม?

**Host A:** เมื่อทุกอย่างผ่าน ก็พร้อม Go Live ครับ! เปิดรับสมาชิกได้เลย

---

## SEGMENT 4: สรุปซีรีส์ทั้งหมด

**Host B:** ก่อนจบ มาสรุปซีรีส์ Secret Of Millionaire Trainer ทั้ง 5 ตอนกันค่ะ:

**Host A:**
- **ตอนที่ 1:** Identity & Mindset — รู้จักตัวเอง หา Niche สร้าง Authority
- **ตอนที่ 2:** Revenue Strategies — 6 ช่องทางรายได้ + Pricing Strategies
- **ตอนที่ 3:** Empire Model — Value Ladder + Product Ecosystem + Positioning
- **ตอนที่ 4:** Membership System — Recurring Revenue + Community Building
- **ตอนที่ 5:** Deploy — ลงมือทำจริงบน Kartra (ตอนนี้!)

**Host B:** จาก Mindset สู่ Strategy สู่ Framework สู่ Implementation ครบวงจรค่ะ ถ้าคุณทำตามทั้ง 5 ตอน คุณจะมี Membership System ที่ทำงานอัตโนมัติ สร้าง Recurring Revenue ทุกเดือน

**Host A:** ขอบคุณที่ติดตามฟังทั้งซีรีส์ครับ ความสำเร็จอยู่ที่การ "ลงมือทำ" ไม่ใช่แค่ "รู้" วันนี้คุณมีทั้งความรู้และเครื่องมือแล้ว สิ่งที่เหลือคือเริ่มลงมือสร้าง Empire ของตัวเอง!

**Host B:** สวัสดีค่ะ และขอให้สนุกกับการสร้าง Membership!

**Host A:** สวัสดีครับ!

---

*สิ้นสุด Audio Script — SOMT-005 | ความยาวโดยประมาณ: 7-8 นาที*
