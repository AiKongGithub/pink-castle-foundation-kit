# Flashcards: วิธีลบและติดตั้ง Camtasia 2018 ใหม่

**Production ID:** VIDEO-016-FLASH
**Format:** 15 Flashcards
**Source:** วิธีลบและติดตั้ง Camtasia 2018

---

## Flashcard 1

**Front:**
สัญญาณอะไรบ้างที่บอกว่าควร Reinstall Camtasia?

**Back:**
**สัญญาณที่ควร Reinstall:**

1. **โปรแกรม Crash บ่อย** - เปิดแล้วปิดเอง
2. **Error Messages** - Error ขึ้นบ่อยโดยไม่มีเหตุผล
3. **Features ไม่ทำงาน** - บาง function ใช้ไม่ได้
4. **Performance แย่ลงมาก** - ช้าผิดปกติ
5. **Update ล้มเหลว** - อัพเดทไม่ได้

---

## Flashcard 2

**Front:**
ก่อน Reinstall ควรลองทำอะไรก่อน?

**Back:**
**ลองทำก่อน Reinstall:**

1. **Restart เครื่อง** - แก้ปัญหา temporary ได้ 20%
2. **Update Graphics Driver** - แก้ได้ 30%
3. **Check Disk Space** - ต้องมีพื้นที่เพียงพอ
4. **Clear Temp Files** - ลบ cache
5. **Run as Administrator** - แก้ปัญหา permissions

---

## Flashcard 3

**Front:**
ก่อนลบ Camtasia ต้อง Backup อะไรบ้าง?

**Back:**
**สิ่งที่ต้อง Backup:**

| รายการ | Priority |
|--------|----------|
| Project Files (.tscproj) | Critical |
| Media Files (video, audio, images) | Critical |
| License Key | Critical |
| Custom Presets | Medium |
| Templates | Medium |

**ตำแหน่ง Project:** Documents > Camtasia

---

## Flashcard 4

**Front:**
จะหา License Key ของ Camtasia ได้ที่ไหน?

**Back:**
**3 วิธีหา License Key:**

1. **ในโปรแกรม:** Help > About Camtasia

2. **TechSmith Account:**
   - techsmith.com > My Account > Licenses

3. **Email:**
   - ค้นหา email ที่มีคำว่า "TechSmith" หรือ "Camtasia"

---

## Flashcard 5

**Front:**
ขั้นตอน Standard Uninstall ใน Windows มีกี่ขั้นตอน?

**Back:**
**5 ขั้นตอน Standard Uninstall:**

1. เปิด **Settings > Apps > Apps & Features**
2. พิมพ์หา **"Camtasia"**
3. คลิก Camtasia แล้วกด **"Uninstall"**
4. **ยืนยัน** Uninstall
5. **รอ** 2-5 นาที

**แต่!** Standard Uninstall ยังเหลือ leftover files

---

## Flashcard 6

**Front:**
Folders อะไรบ้างที่ต้องลบใน Clean Uninstall (Windows)?

**Back:**
**3 Folders ที่ต้องลบ:**

1. **AppData\Roaming:**
   ```
   %APPDATA%\TechSmith
   ```

2. **AppData\Local:**
   ```
   %LOCALAPPDATA%\TechSmith
   ```

3. **ProgramData:**
   ```
   C:\ProgramData\TechSmith
   ```

**Tips:** ใช้ Run (Win+R) แล้วพิมพ์ path

---

## Flashcard 7

**Front:**
Command อะไรใช้เปิด AppData folder?

**Back:**
**Windows Commands (Win+R):**

| Command | เปิด |
|---------|------|
| **%APPDATA%** | AppData\Roaming folder |
| **%LOCALAPPDATA%** | AppData\Local folder |

**วิธีใช้:**
1. กด Win+R
2. พิมพ์ command
3. กด Enter
4. หา folder TechSmith แล้วลบ

---

## Flashcard 8

**Front:**
หลัง Clean Uninstall ต้องทำอะไรก่อน Install ใหม่?

**Back:**
**ต้อง RESTART เครื่องก่อน!**

**เหตุผล:**
- Clear memory
- Release file locks
- Reset system state
- ทำให้ clean install สมบูรณ์

**สำคัญ:** อย่าข้ามขั้นตอนนี้!

---

## Flashcard 9

**Front:**
ทำไมต้อง Download installer ใหม่ แม้จะมีไฟล์เก่าอยู่?

**Back:**
**เหตุผลที่ต้อง Download ใหม่:**

1. **Version ล่าสุด** - มี bug fixes
2. **ไฟล์ไม่ corrupt** - ไฟล์เก่าอาจเสียหาย
3. **Complete package** - ได้ครบทุก component
4. **Matching checksums** - ไฟล์ตรงกับ server

**Download จาก:** techsmith.com/camtasia เท่านั้น

---

## Flashcard 10

**Front:**
หลัง Reinstall ต้องทำอะไรบ้าง?

**Back:**
**Post-Installation Checklist:**

1. **Activate License**
   - Help > Enter Software Key

2. **Check for Updates**
   - Help > Check for Updates

3. **Test Functions**
   - ลอง Record
   - ลอง Import
   - ลอง Export

4. **Restore Custom Presets** (ถ้ามี)

---

## Flashcard 11

**Front:**
ถ้า Reinstall แล้วยังมีปัญหา ควรลองอะไร?

**Back:**
**Troubleshooting หลัง Reinstall:**

1. **Run as Administrator**
   - คลิกขวา > Run as Administrator

2. **Update Graphics Driver**
   - Intel/NVIDIA/AMD

3. **Disable Antivirus ชั่วคราว**
   - บาง AV block Camtasia

4. **Create New User Profile**
   - ถ้าปัญหาอยู่ที่ User Profile

5. **Contact Support**
   - support.techsmith.com

---

## Flashcard 12

**Front:**
Error "License already in use" แก้อย่างไร?

**Back:**
**วิธีแก้ "License already in use":**

1. **Deactivate จากเครื่องเก่า:**
   - เปิด Camtasia บนเครื่องเก่า
   - Help > Deactivate

2. **ถ้าเข้าเครื่องเก่าไม่ได้:**
   - Login ที่ techsmith.com
   - My Account > Manage Licenses
   - Deactivate จาก web

3. **ติดต่อ Support** ถ้าทำไม่ได้

---

## Flashcard 13

**Front:**
Compatibility Mode คืออะไร และใช้เมื่อไหร่?

**Back:**
**Compatibility Mode:**

**คืออะไร:** ทำให้โปรแกรมทำงานเหมือนอยู่บน Windows version เก่า

**ใช้เมื่อ:**
- โปรแกรมไม่ compatible กับ Windows version ปัจจุบัน
- มี error ที่เกี่ยวกับ compatibility

**วิธีตั้ง:**
1. คลิกขวา Camtasia shortcut
2. Properties > Compatibility
3. ติ๊ก "Run in compatibility mode"
4. เลือก Windows version (เช่น Windows 8)

---

## Flashcard 14

**Front:**
Clean Reinstall มี Success Rate ประมาณเท่าไหร่?

**Back:**
**Success Rate ของวิธีแก้ปัญหาต่างๆ:**

| วิธี | Success Rate |
|------|--------------|
| Restart Computer | 20% |
| Update Drivers | 30% |
| Clear Cache | 35% |
| Run as Admin | 25% |
| **Clean Reinstall** | **90%** |
| Contact Support | 95% |

**Clean Reinstall แก้ได้ 90% ของปัญหา!**

---

## Flashcard 15

**Front:**
Clean Reinstall Checklist มีขั้นตอนอะไรบ้าง?

**Back:**
**Complete Checklist:**

**Before:**
- [ ] Backup Project files
- [ ] Backup Media files
- [ ] Note License Key

**Uninstall:**
- [ ] Uninstall via Settings
- [ ] Delete %APPDATA%\TechSmith
- [ ] Delete %LOCALAPPDATA%\TechSmith
- [ ] Delete C:\ProgramData\TechSmith
- [ ] Restart Computer

**Reinstall:**
- [ ] Download latest version
- [ ] Install (Typical)
- [ ] Activate License
- [ ] Check for Updates
- [ ] Test all functions

---

## Study Tips

1. **จำ Folder paths** - ใช้บ่อยในการแก้ปัญหา
2. **Backup ก่อนเสมอ** - กันไว้ดีกว่าแก้
3. **Download ใหม่ทุกครั้ง** - ไม่ใช้ไฟล์เก่า
4. **Test หลัง Install** - ทดสอบทุก function หลัก

---

*Generated for Pink Castle Foundation Kit - SWP3 Curriculum*
*Source: วิธีลบและติดตั้ง Camtasia 2018*
