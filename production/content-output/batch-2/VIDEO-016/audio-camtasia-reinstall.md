# Podcast Script: วิธีลบและติดตั้ง Camtasia 2018 ใหม่

**Production ID:** VIDEO-016-AUDIO
**Format:** Podcast Script
**Duration:** 12-15 นาที
**Source:** วิธีลบและติดตั้ง Camtasia 2018

---

## Episode Opening (1 นาที)

**Host:** สวัสดีครับทุกท่าน ยินดีต้อนรับสู่ Podcast วันนี้ครับ

ถ้าคุณกำลังมีปัญหากับ Camtasia เช่น โปรแกรมค้าง crash บ่อย หรือมี error แปลกๆ วิธีที่ได้ผลที่สุดคือการ **Uninstall แล้ว Reinstall** ใหม่อย่างสะอาด

วันนี้ผมจะพาทุกท่านทำ Clean Reinstall ของ Camtasia 2018 แบบ Step-by-step ครับ ไม่ต้องกลัว ทำตามได้เลย!

---

## Segment 1: เมื่อไหร่ควร Reinstall (2 นาที)

**Host:** ก่อนที่จะลบ มาดูก่อนว่าเมื่อไหร่ควร Reinstall:

**สัญญาณที่บอกว่าควร Reinstall:**

1. **โปรแกรม Crash บ่อย** - เปิดแล้วปิดเอง หรือค้างบ่อย
2. **Error Messages** - มี error ขึ้นบ่อยโดยไม่มีเหตุผลชัดเจน
3. **Features ไม่ทำงาน** - บาง function ใช้ไม่ได้ทั้งที่เคยใช้ได้
4. **Performance แย่ลง** - ช้าลงมากเมื่อเทียบกับตอนแรกติดตั้ง
5. **Update ล้มเหลว** - อัพเดทไม่ได้ มี error

**ลองทำก่อน Reinstall:**
- Restart เครื่อง
- Update Graphics Driver
- Check Disk Space

**Host:** ถ้าทำแล้วยังไม่หาย ก็ถึงเวลา Reinstall ครับ

---

## Segment 2: Backup ก่อนลบ (2 นาที)

**Host:** สิ่งสำคัญมาก ก่อนลบโปรแกรม ต้อง Backup ก่อน!

**สิ่งที่ควร Backup:**

**1. Project Files (.tscproj)**
- ไฟล์โปรเจกต์ทั้งหมด
- ปกติอยู่ใน Documents > Camtasia

**2. Media Files**
- Video, Audio, Images ที่ใช้ในโปรเจกต์
- ควร copy ไว้ที่อื่นด้วย

**3. Custom Presets & Templates**
- ถ้าคุณสร้าง Preset เอง
- อยู่ใน: %APPDATA%\TechSmith\Camtasia Studio\18.0

**4. License Key**
- จด Software Key ไว้ หรือ
- เข้าไป TechSmith Account เพื่อดู Key

**Host:** จำไว้ว่า การ Reinstall จะไม่ลบ Project files แต่ Backup ไว้ก็ปลอดภัยกว่าครับ

---

## Segment 3: วิธี Uninstall แบบปกติ (3 นาที)

**Host:** มาเริ่มขั้นตอน Uninstall กันครับ

**วิธี Uninstall ผ่าน Windows:**

**Step 1:** ไปที่ Settings > Apps > Apps & Features
หรือพิมพ์ "Add or remove programs" ใน Start Menu

**Step 2:** หา "Camtasia 2018" ในรายการ

**Step 3:** คลิกที่ Camtasia แล้วกด "Uninstall"

**Step 4:** ยืนยัน Uninstall

**Step 5:** รอจนเสร็จ ประมาณ 2-5 นาที

**สำหรับ Mac:**
- เปิด Finder > Applications
- ลาก Camtasia ไปที่ Trash
- Empty Trash

**Host:** แต่เดี๋ยวก่อน! ถ้าจะทำ Clean Reinstall จริงๆ ยังไม่พอครับ ต้องลบ leftover files ด้วย

---

## Segment 4: Clean Uninstall - ลบให้สะอาด (3 นาที)

**Host:** การ Uninstall ปกติจะยังเหลือไฟล์ค้างอยู่ ถ้าจะ clean จริงๆ ต้องลบเพิ่ม:

**Windows - ลบ Folders เหล่านี้:**

**1. AppData Folder:**
```
C:\Users\[YourName]\AppData\Local\TechSmith
C:\Users\[YourName]\AppData\Roaming\TechSmith
```

**2. ProgramData Folder:**
```
C:\ProgramData\TechSmith
```

**3. Registry (Optional - สำหรับ Advanced users):**
- เปิด Registry Editor (regedit)
- ไปที่ HKEY_CURRENT_USER\Software\TechSmith
- ลบ folder TechSmith

**Mac - ลบ Folders เหล่านี้:**
```
~/Library/Application Support/TechSmith
~/Library/Preferences/com.techsmith.*
```

**Host:** หลังลบเสร็จ แนะนำให้ Restart เครื่องก่อน Install ใหม่ครับ

---

## Segment 5: Reinstall Camtasia (2 นาที)

**Host:** หลังจาก Clean Uninstall และ Restart แล้ว มาติดตั้งใหม่กัน:

**Step 1: Download ใหม่**
- ไปที่ techsmith.com/camtasia
- Download version ล่าสุด (แม้ว่าจะมีไฟล์เก่าอยู่ก็ download ใหม่)

**Step 2: Install**
- Double-click installer
- Accept License Agreement
- เลือก Typical
- รอติดตั้งเสร็จ

**Step 3: Activate License**
- ใส่ Software Key เหมือนเดิม
- หรือ Login ด้วย TechSmith Account

**Step 4: Check for Updates**
- หลังติดตั้งเสร็จ
- Help > Check for Updates
- อัพเดทถ้ามี

**Host:** เสร็จแล้ว! ตอนนี้คุณมี Camtasia ที่สะอาดและทำงานได้ปกติแล้วครับ

---

## Segment 6: Troubleshooting หลัง Reinstall (2 นาที)

**Host:** ถ้า Reinstall แล้วยังมีปัญหา ลองทำสิ่งเหล่านี้:

**1. Compatibility Mode (Windows)**
- คลิกขวาที่ Camtasia shortcut
- Properties > Compatibility
- ลอง Run as Administrator

**2. Graphics Driver**
- อัพเดท Graphics Driver ให้ล่าสุด
- Intel, NVIDIA, AMD ตาม GPU ที่ใช้

**3. Disable Antivirus ชั่วคราว**
- บาง Antivirus block Camtasia
- ลอง disable แล้วเปิด Camtasia ใหม่

**4. Create New User Profile**
- ถ้าปัญหาอยู่ที่ User Profile
- สร้าง Windows User ใหม่แล้วลอง

**5. Contact TechSmith Support**
- ถ้าทำทุกอย่างแล้วยังไม่หาย
- support.techsmith.com

**Host:** ส่วนใหญ่ Clean Reinstall จะแก้ปัญหาได้ครับ

---

## Episode Closing (1 นาที)

**Host:** มาสรุปกันครับ

**ขั้นตอน Clean Reinstall:**
1. Backup Project files และ License Key
2. Uninstall ผ่าน Windows Settings
3. ลบ Leftover files ใน AppData และ ProgramData
4. Restart เครื่อง
5. Download และ Install ใหม่
6. Activate License
7. Check for Updates

**Host:** หวังว่าตอนนี้จะช่วยแก้ปัญหา Camtasia ของทุกท่านได้นะครับ

อย่าลืม Backup ก่อนลบทุกครั้ง และถ้ามีคำถามก็ส่งมาได้เลย

พบกันใหม่ตอนหน้า สวัสดีครับ!

---

## Production Notes

- **Tone:** Helpful, Reassuring
- **Background Music:** Calm, Problem-solving vibe
- **Pacing:** Clear steps, pause between each
- **Supplementary:** Include command line paths in show notes

---

*Generated for Pink Castle Foundation Kit - SWP3 Curriculum*
*Source: วิธีลบและติดตั้ง Camtasia 2018*
