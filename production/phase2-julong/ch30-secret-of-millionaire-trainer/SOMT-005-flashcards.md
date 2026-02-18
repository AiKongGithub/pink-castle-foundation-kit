# วิธี Deploy Membership System — SOMT-005
> **Format:** Flashcards
> **Source:** SWP3 Ch30 The Secret Of Millionaire Trainer ตอนที่ 5
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-18

---

=== CARD 1 ===

**Q:** 6 ขั้นตอนการ Deploy Membership บน Kartra คืออะไร? เรียงลำดับ

**A:**
1. สร้าง Membership Portal (ตั้งชื่อ + เลือก Template)
2. ตั้งค่า Membership Levels (Silver/Gold + Access Rules)
3. Domain Configuration (Custom Domain หรือ Kartra Subdomain)
4. SSL Setup (Enable HTTPS)
5. Payment Setup (Stripe/PayPal + Products + Recurring Billing)
6. ทดสอบ + Go Live (6-point Testing Checklist)

---

=== CARD 2 ===

**Q:** เมื่อสร้าง Membership Portal ใน Kartra ต้องทำอะไรบ้าง?

**A:** เข้า Kartra Dashboard → Memberships → New Membership แล้ว:
1. ตั้งชื่อ Membership
2. เลือก Template (Modern, Classic, Sidebar Navigation)
3. ใส่ Description (คำอธิบาย)
4. ใส่ Welcome Message (ข้อความต้อนรับ)
เลือก Template ที่ตรงกับ Brand ช่วยประหยัดเวลาสร้างได้มาก

---

=== CARD 3 ===

**Q:** การตั้งค่า Levels ใน Kartra ต้องกำหนดอะไรบ้าง?

**A:** สำหรับแต่ละ Level ต้องกำหนด:
- **Access Rules** — Silver เข้าถึง Category ไหน, Gold เข้าถึง Category ไหน
- **Content Dripping** — เนื้อหาเปิดเมื่อไหร่ (ตามสัปดาห์/วันที่สมัคร)
- **Locked Content** — Content ที่ต้อง Upgrade ถึงจะเปิดได้ พร้อมหน้า "Upgrade"

---

=== CARD 4 ===

**Q:** Custom Domain กับ Kartra Subdomain ต่างกันอย่างไร?

**A:**
- **Custom Domain** (เช่น members.yourbrand.com): Professional, Brand เป็นของตัวเอง แต่ต้องตั้ง DNS (CNAME Record ชี้ไป Kartra)
- **Kartra Subdomain** (เช่น yourbrand.kartra.com): ง่าย ใช้งานได้ทันทีโดยไม่ต้องตั้ง DNS แต่ดูน่าเชื่อถือน้อยกว่า
แนะนำใช้ Custom Domain ถ้าเป็นไปได้

---

=== CARD 5 ===

**Q:** SSL คืออะไร? ทำไมถึงจำเป็นสำหรับ Membership?

**A:** SSL (Secure Sockets Layer) ทำให้เว็บไซต์เป็น HTTPS มีกุญแจล็อคในแถบ URL จำเป็นเพราะ:
1. **ความปลอดภัย** — เข้ารหัสข้อมูลระหว่างผู้ใช้กับเซิร์ฟเวอร์
2. **ความน่าเชื่อถือ** — ลูกค้าเชื่อมั่นเว็บที่มี HTTPS
3. **Payment** — Stripe/PayPal บังคับใช้ HTTPS สำหรับรับเงิน
Kartra ให้ SSL ฟรี กด Enable แล้วรอไม่เกิน 24 ชั่วโมง

---

=== CARD 6 ===

**Q:** การตั้ง Payment ใน Kartra ต้องทำอะไรบ้าง?

**A:**
1. เข้า "My Integrations" เชื่อมต่อ Stripe หรือ PayPal (ใส่ API Keys)
2. สร้าง Products สำหรับแต่ละ Level (Silver 990/เดือน, Gold 2,990/เดือน)
3. เชื่อม Product กับ Membership Level
4. ตั้ง Recurring Billing (เก็บเงินอัตโนมัติทุกเดือน)
5. ทดสอบด้วย Test Mode ก่อน Go Live

---

=== CARD 7 ===

**Q:** Testing Checklist 6 ข้อก่อน Go Live คืออะไร?

**A:**
1. **Signup Flow** — สมัครสมาชิกได้ไหม?
2. **Payment** — ชำระเงินได้ไหม? (ใช้ Test Card)
3. **Access Control** — Silver เข้า Gold Content ไม่ได้ใช่ไหม?
4. **Content Dripping** — เนื้อหาเปิดตามตารางไหม?
5. **Welcome Email** — สมาชิกใหม่ได้รับ Email ไหม?
6. **Cancellation** — Cancel แล้วเข้าถึง Content ไม่ได้ใช่ไหม?
ทุกข้อต้องผ่านก่อน Go Live!

---

=== CARD 8 ===

**Q:** ทำไมควร Soft Launch ก่อน Public Launch?

**A:** Soft Launch (เปิดให้ 5-10 Beta Members) ช่วย:
1. ทดสอบระบบกับผู้ใช้จริง
2. เก็บ Feedback จากมุมมองลูกค้า
3. แก้ไขปัญหาก่อนเปิดให้คนจำนวนมาก
4. สร้าง Testimonials แรกสำหรับใช้ใน Public Launch
5. ลดความเสี่ยงที่ลูกค้าจำนวนมากจะเจอปัญหาพร้อมกัน

---

=== CARD 9 ===

**Q:** ซีรีส์ Secret Of Millionaire Trainer ทั้ง 5 ตอนครอบคลุมอะไรบ้าง?

**A:**
- **ตอน 1:** Identity & Mindset — รู้จักตัวเอง หา Niche สร้าง Authority
- **ตอน 2:** Revenue Strategies — 6 ช่องทางรายได้ + Pricing
- **ตอน 3:** Empire Model — Value Ladder + Product Ecosystem
- **ตอน 4:** Membership System — Recurring Revenue + Community
- **ตอน 5:** Deploy — Technical Setup + Go Live
เส้นทาง: Mindset → Strategy → Framework → Design → Implementation

---

=== CARD 10 ===

**Q:** ทำไมต้องทดสอบ Payment ด้วย Test Mode ก่อน?

**A:** เพราะ:
1. ไม่ต้องใช้เงินจริงในการทดสอบ (Stripe มี Test Card เช่น 4242 4242 4242 4242)
2. ตรวจสอบว่า Recurring Billing ทำงานถูกต้อง
3. ทดสอบ Dunning Management ว่าส่ง Email เมื่อ Payment ล้มเหลว
4. ยืนยันว่า Product เชื่อมกับ Membership Level ถูกต้อง
5. ป้องกันปัญหาด้านเงินกับลูกค้าจริง

---

=== CARD 11 ===

**Q:** ควรเตรียม Content อย่างน้อยกี่สัปดาห์ก่อน Go Live? เพราะอะไร?

**A:** อย่างน้อย 2 สัปดาห์ เพราะลูกค้าที่จ่ายเงินแล้วต้องเห็น Content ทันที ถ้า Go Live โดยมีแค่ Welcome Message ลูกค้าจะรู้สึกผิดหวังและอาจ Cancel ทันที ต้องเตรียม Content พร้อม Content Dripping Schedule ให้พร้อมก่อนเปิดรับสมาชิก

---

=== CARD 12 ===

**Q:** CNAME Record ใช้ทำอะไรในการตั้ง Custom Domain?

**A:** CNAME (Canonical Name) Record ใช้ชี้ Custom Domain ของคุณ (เช่น members.yourbrand.com) ไปที่เซิร์ฟเวอร์ของ Kartra ตั้งค่าที่ Domain Registrar (เช่น Namecheap, Cloudflare) หลังตั้งแล้วรอ DNS Propagation ประมาณ 1-48 ชั่วโมง

---

*สิ้นสุด Flashcards — SOMT-005 | จำนวน 12 ใบ*
