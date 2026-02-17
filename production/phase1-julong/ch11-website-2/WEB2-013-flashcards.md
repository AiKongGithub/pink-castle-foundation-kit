# Flashcards: วิธีการตั้งค่า UpdraftPlus — WEB2-013
> **Format:** Flashcards (Q&A)
> **Source:** SWP3 Ch11 สร้างเว็บไซต์ Part 2 ตอนที่ 13
> **Production:** PinkCastle Academy | จูล่ง CTO
> **Date:** 2026-02-17

---

=== CARD 1 ===

**Q:** UpdraftPlus คืออะไร?

**A:** ปลั๊กอิน Backup ยอดนิยมอันดับ 1 ของ WordPress ช่วยสำรองข้อมูลเว็บไซต์ทั้งหมดแบบอัตโนมัติ ตั้ง Schedule ได้ เก็บไว้บน Remote Storage กู้คืนด้วยคลิกเดียว และรองรับการ Migrate/Clone เว็บไซต์

---

=== CARD 2 ===

**Q:** ทำไมการ Backup เว็บไซต์จึงสำคัญ?

**A:** เพราะปัญหาเกิดขึ้นได้ตลอดเวลา 4 สาเหตุหลัก ได้แก่ (1) อัปเดตปลั๊กอิน/ธีม แล้วเว็บพัง (2) ถูกแฮก (3) ความผิดพลาดของมนุษย์ เช่น ลบไฟล์ผิด (4) ปัญหาจากโฮสติ้ง เช่น server ล่ม ถ้าไม่มี Backup ต้องเริ่มใหม่ตั้งแต่ศูนย์

---

=== CARD 3 ===

**Q:** ทำไมต้องตั้ง Backup Schedule แยกระหว่าง Database กับ Files?

**A:** เพราะ Database เปลี่ยนแปลงบ่อยกว่า (ทุกครั้งที่มี comment, บทความ, order ใหม่) จึงควร Backup เป็น Daily ส่วน Files (ปลั๊กอิน ธีม รูปภาพ) ไม่ค่อยเปลี่ยน ตั้งเป็น Weekly ก็เพียงพอ ช่วยประหยัดพื้นที่จัดเก็บ

---

=== CARD 4 ===

**Q:** Retain ใน UpdraftPlus คืออะไร และควรตั้งเท่าไร?

**A:** Retain คือจำนวนชุด Backup ที่เก็บไว้ เมื่อมีชุดใหม่ ชุดเก่าสุดจะถูกลบ แนะนำตั้ง 4-7 ชุด เพื่อมีหลาย version ย้อนหลัง ในกรณีที่ไม่รู้ว่าปัญหาเกิดขึ้นตั้งแต่เมื่อไร จะได้มีหลายจุดให้เลือกกู้คืน

---

=== CARD 5 ===

**Q:** ทำไมไม่ควรเก็บ Backup ไว้บน server เดียวกับเว็บไซต์?

**A:** เพราะถ้า server พัง ทั้งเว็บไซต์และ Backup จะหายไปด้วย ต้องเก็บ Backup ไว้บน Remote Storage ที่แยกต่างหาก เช่น Google Drive, Dropbox หรือ Amazon S3 เพื่อให้มี Backup สำรองแม้ server จะล่ม

---

=== CARD 6 ===

**Q:** Remote Storage ที่แนะนำมากที่สุดสำหรับ UpdraftPlus คืออะไร เพราะอะไร?

**A:** Google Drive เพราะฟรีมีพื้นที่ 15 GB เชื่อมต่อง่ายมาก แค่กดเลือก Google Drive ในการตั้งค่า แล้ว Authorize ด้วย Google Account ก็เสร็จ เพียงพอสำหรับเว็บไซต์ส่วนใหญ่

---

=== CARD 7 ===

**Q:** UpdraftPlus สำรองข้อมูลอะไรบ้าง?

**A:** 5 ส่วน ได้แก่ (1) Database — หัวใจของเว็บ เก็บบทความ หน้า ความคิดเห็น การตั้งค่า (2) Plugins — ปลั๊กอินทั้งหมด (3) Themes — ธีมทั้งหมด (4) Uploads — ไฟล์สื่อ รูปภาพ วิดีโอ PDF (5) Others — ไฟล์อื่นๆ

---

=== CARD 8 ===

**Q:** ขั้นตอนการ Restore (กู้คืน) ด้วย UpdraftPlus ทำอย่างไร?

**A:** (1) ไปที่แท็บ Existing Backups (2) เลือกชุด Backup ที่ต้องการ กดปุ่ม Restore (3) เลือกส่วนที่จะ Restore: Database, Plugins, Themes, Uploads หรือทั้งหมด (4) กด Restore ระบบจะจัดการให้ UpdraftPlus จะเก็บเวอร์ชันก่อน Restore ไว้ด้วยเป็น safety net

---

=== CARD 9 ===

**Q:** UpdraftPlus ช่วย Migrate/Clone เว็บไซต์ได้อย่างไร?

**A:** ใช้ Backup จาก UpdraftPlus ไป Restore บน server ใหม่ได้ ในเวอร์ชันฟรีต้อง Backup จากเว็บเก่า แล้วอัปโหลด Backup ไป Restore บนเว็บใหม่ด้วยตนเอง ส่วนเวอร์ชัน Premium มี Migrator tool ที่ทำให้อัตโนมัติ

---

=== CARD 10 ===

**Q:** ทำไมต้อง "ทดสอบ" Backup เป็นประจำ?

**A:** เพราะ Backup ที่ Restore ไม่ได้ก็ไม่มีค่าอะไรเลย แนะนำทดสอบอย่างน้อย 3-6 เดือนครั้ง โดยสร้าง staging site แล้วลอง Restore ดูว่าข้อมูลครบถ้วนและเว็บทำงานปกติหรือไม่

---

=== CARD 11 ===

**Q:** UpdraftPlus Free กับ Premium ต่างกันอย่างไร?

**A:** Free ทำได้เกือบทุกอย่าง ทั้ง Schedule, Remote Storage, Restore ส่วน Premium เพิ่ม Incremental Backup (backup เฉพาะไฟล์ที่เปลี่ยน ประหยัดพื้นที่), Migrator tool (ย้ายเว็บอัตโนมัติ) และ Remote Storage เพิ่มเติม สำหรับเว็บทั่วไปเวอร์ชันฟรีเพียงพอ

---

=== CARD 12 ===

**Q:** กฎ 3-2-1 ของการ Backup คืออะไร?

**A:** สำรองข้อมูลไว้ 3 ชุด บน 2 สื่อที่ต่างกัน (เช่น server + cloud) และ 1 ชุดต้องอยู่นอกสถานที่ (off-site) เช่น Google Drive หรือ Dropbox ที่ไม่ใช่ server เดียวกับเว็บ เพื่อป้องกันการสูญเสียข้อมูลทุกกรณี

---

*จำนวน Flashcards ทั้งหมด: 12 ใบ*
