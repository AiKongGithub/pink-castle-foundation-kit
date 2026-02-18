# สร้างบทความ ด้วย Content Builder ตอนที่ 2 — CMKTG-015 Flashcards
> Format: Flashcards (12 Cards)
> Source: SWP3 Ch28 Content Marketing Mastery ตอนที่ 15
> Production: PinkCastle Academy | จูล่ง CTO
> Date: 2026-02-18 | Duration: 0:26:27

---

=== CARD 1 ===
Q: Custom CSS/Styling ใน Content Builder ทำอะไรได้บ้าง และข้อควรระวังคืออะไร?
A: ทำได้หลายอย่าง เช่น เปลี่ยนสี Heading ให้ตรง Brand, เพิ่ม Border/Shadow ให้กล่องข้อความ, สร้าง Callout Box เน้นข้อมูลสำคัญ, ปรับ Font ให้เข้ากับ Brand Identity ข้อควรระวังคือต้อง Test Responsive บนมือถือทุกครั้ง และใช้ Media Query สำหรับหน้าจอขนาดต่างๆ

=== CARD 2 ===
Q: Embed Code สำหรับ YouTube/Podcast มีเคล็ดลับสำคัญอะไรบ้าง 3 ข้อ?
A: 1) ใช้ Responsive Embed — wrap iframe ด้วย Container ที่มี CSS `position: relative; padding-bottom: 56.25%` สำหรับ 16:9 2) ไม่ Embed มากเกินไป — แนะนำไม่เกิน 2-3 Embed ต่อบทความเพราะทำให้หน้าโหลดช้า 3) ใช้ Lazy Loading สำหรับ Embed เพื่อไม่ให้โหลดจนกว่าผู้อ่านจะ Scroll มาถึง

=== CARD 3 ===
Q: Content Upgrade คืออะไร และต่างจาก Lead Magnet ทั่วไปอย่างไร?
A: Content Upgrade คือสิ่งที่เสนอให้ผู้อ่านดาวน์โหลดฟรีแลกกับอีเมล โดยเนื้อหาต้องเจาะจงและเกี่ยวข้องกับบทความที่กำลังอ่าน ต่างจาก Lead Magnet ทั่วไปที่ใช้แบบกว้างๆ ทุกหน้า Content Upgrade มี Conversion Rate สูงกว่า Lead Magnet ทั่วไปถึง 5-10 เท่า

=== CARD 4 ===
Q: Content Upgrade ที่ดีควรมีลักษณะอย่างไร และวางตำแหน่งไว้ตรงไหน?
A: ต้องเป็นไฟล์ที่มีประโยชน์เช่น PDF Checklist, Template หรือ Worksheet ที่เกี่ยวข้องกับเนื้อหาบทความ ใช้ Opt-in Form ฝังในบทความพร้อมข้อความดึงดูด ตำแหน่งที่ดีที่สุดคือหลังจากเนื้อหาส่วนที่น่าสนใจที่สุดในบทความ

=== CARD 5 ===
Q: Related Posts Widget มีกี่แบบ และแบบไหนดีที่สุด?
A: มี 3 แบบ คือ 1) Manual — เลือกเองซึ่งแม่นยำที่สุด 2) Auto — ดึงจาก Category/Tag เดียวกัน 3) Hybrid — ผสมทั้งสองแบบ ช่วยลด Bounce Rate และเพิ่ม Time on Site โดยแสดงบทความที่เกี่ยวข้องท้ายบทความหรือ Sidebar

=== CARD 6 ===
Q: Social Share Buttons ต้องมีกี่แพลตฟอร์มอะไรบ้าง และตำแหน่งที่ดีที่สุดคือตรงไหน?
A: ต้องมี 5 แพลตฟอร์ม คือ Facebook, LINE, Twitter/X, LinkedIn และ Copy Link วางไว้ 2 จุด คือใต้ Title กับด้านล่างก่อน Related Posts ต้องตั้งค่า Open Graph Tags ให้ถูกต้องเพื่อให้รูป/Title/Description แสดงสวยเมื่อคนแชร์

=== CARD 7 ===
Q: Blog Analytics ผ่าน GA4 มีตัวเลขอะไรบ้าง 5 ตัวที่ต้องดู?
A: 1) Page Views — จำนวนคนเข้ามาดู 2) Average Engagement Time — อ่านนานแค่ไหน 3) Bounce Rate — อ่านหน้าเดียวแล้วออก 4) Scroll Depth — อ่านถึงตรงไหนของบทความ 5) Conversion Rate — กดปุ่ม CTA กี่เปอร์เซ็นต์ ใช้ร่วมกับ GTM ตั้ง Custom Events

=== CARD 8 ===
Q: Image Compression มีวิธีทำอย่างไร และใช้เครื่องมืออะไร?
A: 4 วิธีหลัก คือ 1) ใช้รูปแบบ WebP แทน PNG/JPEG เล็กกว่า 30-50% คุณภาพเท่าเดิม 2) Compress ด้วย TinyPNG, Squoosh หรือ ShortPixel 3) ขนาดรูปไม่เกิน 1200px กว้างสำหรับ Full-width, 800px สำหรับ In-content 4) ใช้ Srcset ให้ Browser เลือกขนาดที่เหมาะกับหน้าจอ

=== CARD 9 ===
Q: Lazy Loading คืออะไร และช่วยเพิ่ม Page Speed ได้เท่าไร?
A: Lazy Loading คือเทคนิคที่ทำให้รูปภาพและ Embed โหลดก็ต่อเมื่อผู้อ่าน Scroll มาถึงเท่านั้น ไม่โหลดทุกอย่างตั้งแต่แรก วิธีทำคือเพิ่ม `loading="lazy"` ในแท็ก `<img>` หรือใช้ Plugin ของ CMS ผลลัพธ์คือ Page Speed Score เพิ่มขึ้น 20-40 คะแนน

=== CARD 10 ===
Q: Content Calendar ควร Publish บทความบ่อยแค่ไหน และ Batch Process คืออะไร?
A: แนะนำ 1-2 บทความต่อสัปดาห์ Publish สม่ำเสมอดีกว่า Publish เป็นพักๆ เพราะ Google ชอบเว็บที่อัปเดตสม่ำเสมอ Batch Process คือเขียนหลายบทความในวันเดียวแล้วตั้ง Schedule ให้ Publish ทีละบทความตามวันที่กำหนด ช่วยประหยัดเวลาและรักษาความสม่ำเสมอ

=== CARD 11 ===
Q: Repurpose Blog เป็น Social Media Content ทำได้กี่แบบ และหลักการคืออะไร?
A: ทำได้ 7 แบบ คือ 1) Carousel Post 2) Quote Card 3) Thread บน X 4) Podcast Episode 5) Short Video (Reels/TikTok) 6) Infographic 7) Newsletter หลักการคือ "สร้างครั้งเดียว แจกจ่ายหลายที่" บทความ 1 ชิ้นแตกเป็นคอนเทนต์ได้ 10-15 ชิ้น ไม่ต้องคิด Content ใหม่ทุกครั้ง

=== CARD 12 ===
Q: หน้าที่โหลดช้าเกิน 3 วินาที สูญเสียผู้อ่านเท่าไร และวิธีแก้ 2 อย่างหลักคืออะไร?
A: สูญเสียผู้อ่านถึง 53% ถ้าโหลดนานเกิน 3 วินาที วิธีแก้ 2 อย่างหลักคือ 1) Image Compression — ใช้ WebP + Compress ขนาดไม่เกิน 200 KB + ใช้ Srcset 2) Lazy Loading — โหลดรูป/Embed เมื่อ Scroll มาถึง ผลลัพธ์คือ Page Speed Score เพิ่ม 20-40 คะแนน

---
*12 cards | สำหรับทบทวนความรู้เรื่อง Content Builder ตอน 2 — Advanced Techniques, GA4, Performance, Repurpose*

---

> จบ Ch28 Content Marketing Mastery — ทั้งหมด 15 ตอน
> Series: SWP3 Ch28 Content Marketing Mastery
> PinkCastle Academy © 2026
