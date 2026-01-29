# Mind Map: วิธีลบและติดตั้ง Camtasia 2018 ใหม่

**Production ID:** VIDEO-016-MIND
**Format:** Mind Map (Text-based)
**Source:** วิธีลบและติดตั้ง Camtasia 2018

---

## Central Topic: Camtasia Clean Reinstall

```
                                    ┌─────────────────────┐
                                    │     CAMTASIA        │
                                    │  CLEAN REINSTALL    │
                                    │   ลบและติดตั้งใหม่    │
                                    └──────────┬──────────┘
                                               │
           ┌───────────────┬───────────────┬───┴───┬───────────────┬───────────────┐
           │               │               │       │               │               │
           ▼               ▼               ▼       ▼               ▼               ▼
    ┌──────────┐    ┌──────────┐    ┌──────────┐  ┌──────────┐    ┌──────────┐
    │   WHEN   │    │  BACKUP  │    │UNINSTALL │  │REINSTALL │    │TROUBLE-  │
    │TO REINSTALL│  │  FIRST   │    │  CLEAN   │  │  FRESH   │    │ SHOOTING │
    └────┬─────┘    └────┬─────┘    └────┬─────┘  └────┬─────┘    └────┬─────┘
         │               │               │             │               │
```

---

## Branch 1: When to Reinstall (เมื่อไหร่ควร Reinstall)

```
WHEN TO REINSTALL
    │
    ├── สัญญาณที่บอกว่าควร Reinstall
    │   │
    │   ├── โปรแกรม Crash บ่อย
    │   │   ├── เปิดแล้วปิดเอง
    │   │   ├── ค้างบ่อย
    │   │   └── Not Responding
    │   │
    │   ├── Error Messages
    │   │   ├── Error ขึ้นบ่อย
    │   │   ├── ไม่มีเหตุผลชัดเจน
    │   │   └── Error ที่ไม่เคยเจอ
    │   │
    │   ├── Features ไม่ทำงาน
    │   │   ├── Record ไม่ได้
    │   │   ├── Export ไม่ได้
    │   │   └── Effects ไม่ทำงาน
    │   │
    │   ├── Performance แย่ลง
    │   │   ├── ช้ากว่าปกติมาก
    │   │   ├── Preview กระตุก
    │   │   └── Export นานขึ้น
    │   │
    │   └── Update ล้มเหลว
    │       ├── อัพเดทไม่ได้
    │       └── Error ตอน Update
    │
    └── ลองทำก่อน Reinstall
        ├── Restart เครื่อง
        ├── Update Graphics Driver
        ├── Check Disk Space
        ├── Clear Temp Files
        └── Disable Antivirus ชั่วคราว
```

---

## Branch 2: Backup First (Backup ก่อนลบ)

```
BACKUP FIRST
    │
    ├── Project Files (.tscproj)
    │   ├── ตำแหน่ง
    │   │   └── Documents > Camtasia
    │   │
    │   ├── วิธี Backup
    │   │   ├── Copy ทั้ง folder
    │   │   └── ไปที่ External Drive หรือ Cloud
    │   │
    │   └── สำคัญ
    │       └── Project files จะไม่ถูกลบ แต่ backup ไว้ปลอดภัย
    │
    ├── Media Files
    │   ├── Video files ที่ใช้
    │   ├── Audio files
    │   ├── Images
    │   └── Copy แยกไว้ที่อื่น
    │
    ├── Custom Presets & Templates
    │   ├── ตำแหน่ง (Windows)
    │   │   └── %APPDATA%\TechSmith\Camtasia Studio\18.0
    │   │
    │   └── สิ่งที่ต้อง backup
    │       ├── Custom transitions
    │       ├── Custom callouts
    │       └── Templates ที่สร้างเอง
    │
    └── License Key
        ├── วิธีหา
        │   ├── Help > About Camtasia
        │   ├── Email ที่ซื้อ
        │   └── TechSmith Account
        │
        └── จดไว้หรือ Screenshot
```

---

## Branch 3: Uninstall Clean (ลบให้สะอาด)

```
UNINSTALL CLEAN
    │
    ├── Standard Uninstall (Windows)
    │   │
    │   ├── Step 1: เปิด Settings
    │   │   └── Settings > Apps > Apps & Features
    │   │
    │   ├── Step 2: หา Camtasia
    │   │   └── พิมพ์ "Camtasia" ในช่อง Search
    │   │
    │   ├── Step 3: Uninstall
    │   │   └── คลิก > Uninstall
    │   │
    │   ├── Step 4: ยืนยัน
    │   │   └── กด Yes/Confirm
    │   │
    │   └── Step 5: รอ
    │       └── 2-5 นาที
    │
    ├── Standard Uninstall (Mac)
    │   ├── Finder > Applications
    │   ├── ลาก Camtasia ไป Trash
    │   └── Empty Trash
    │
    └── Clean Leftover Files
        │
        ├── Windows Folders ที่ต้องลบ
        │   │
        │   ├── AppData\Roaming
        │   │   └── C:\Users\[Name]\AppData\Roaming\TechSmith
        │   │
        │   ├── AppData\Local
        │   │   └── C:\Users\[Name]\AppData\Local\TechSmith
        │   │
        │   └── ProgramData
        │       └── C:\ProgramData\TechSmith
        │
        ├── Mac Folders ที่ต้องลบ
        │   ├── ~/Library/Application Support/TechSmith
        │   └── ~/Library/Preferences/com.techsmith.*
        │
        ├── Registry (Windows - Optional)
        │   ├── เปิด regedit
        │   ├── HKEY_CURRENT_USER\Software\TechSmith
        │   └── ลบ folder TechSmith
        │
        └── สุดท้าย
            └── RESTART เครื่อง!
```

---

## Branch 4: Reinstall Fresh (ติดตั้งใหม่)

```
REINSTALL FRESH
    │
    ├── Step 1: Download ใหม่
    │   ├── ไปที่ techsmith.com/camtasia
    │   ├── Download version ล่าสุด
    │   └── อย่าใช้ไฟล์เก่า!
    │
    ├── Step 2: Run Installer
    │   ├── Double-click .exe
    │   └── Accept UAC prompt
    │
    ├── Step 3: Installation Wizard
    │   ├── Accept License Agreement
    │   ├── เลือก "Typical"
    │   └── ใช้ Default location
    │
    ├── Step 4: Wait
    │   └── 5-10 นาที
    │
    ├── Step 5: Activate License
    │   ├── Help > Enter Software Key
    │   ├── ใส่ Email + Key
    │   └── หรือ Login TechSmith Account
    │
    ├── Step 6: Check for Updates
    │   ├── Help > Check for Updates
    │   └── Install ถ้ามี
    │
    └── Step 7: Test
        ├── ลอง Record
        ├── ลอง Import
        └── ลอง Export
```

---

## Branch 5: Troubleshooting (แก้ปัญหาเพิ่มเติม)

```
TROUBLESHOOTING
    │
    ├── ถ้ายังมีปัญหาหลัง Reinstall
    │   │
    │   ├── Run as Administrator
    │   │   ├── คลิกขวา Camtasia shortcut
    │   │   ├── Properties > Compatibility
    │   │   └── ติ๊ก "Run as Administrator"
    │   │
    │   ├── Compatibility Mode
    │   │   ├── Properties > Compatibility
    │   │   └── ลอง Run ใน Windows 8 mode
    │   │
    │   ├── Update Graphics Driver
    │   │   ├── Intel: intel.com/drivers
    │   │   ├── NVIDIA: nvidia.com/drivers
    │   │   └── AMD: amd.com/drivers
    │   │
    │   ├── Disable Antivirus
    │   │   ├── ปิดชั่วคราว
    │   │   ├── Add Camtasia to Whitelist
    │   │   └── ปิด Real-time protection
    │   │
    │   ├── Create New User Profile
    │   │   ├── สร้าง Windows User ใหม่
    │   │   ├── Install Camtasia บน User ใหม่
    │   │   └── ทดสอบว่าทำงานไหม
    │   │
    │   └── Contact Support
    │       └── support.techsmith.com
    │
    └── Common Error Solutions
        │
        ├── "License already in use"
        │   └── Deactivate จากเครื่องเก่าก่อน
        │
        ├── "Failed to initialize"
        │   └── Update Graphics Driver
        │
        ├── "Recording failed"
        │   ├── Run as Admin
        │   └── Check Permissions
        │
        └── "Export failed"
            ├── Check Disk Space
            └── Try different format
```

---

## Quick Reference: Clean Reinstall Checklist

```
CLEAN REINSTALL CHECKLIST
    │
    ├── Before Uninstall
    │   □ Backup Project files
    │   □ Backup Media files
    │   □ Note down License Key
    │   □ Backup Custom Presets
    │
    ├── Uninstall
    │   □ Uninstall via Windows Settings
    │   □ Delete AppData\Roaming\TechSmith
    │   □ Delete AppData\Local\TechSmith
    │   □ Delete ProgramData\TechSmith
    │   □ Restart Computer
    │
    ├── Reinstall
    │   □ Download latest version
    │   □ Run Installer
    │   □ Choose Typical installation
    │   □ Activate License
    │   □ Check for Updates
    │
    └── Verify
        □ Test Screen Recording
        □ Test Video Import
        □ Test Export
        □ Restore Custom Presets
```

---

## File Paths Quick Reference

```
WINDOWS PATHS
    │
    ├── AppData Roaming
    │   └── %APPDATA%\TechSmith
    │       = C:\Users\[Name]\AppData\Roaming\TechSmith
    │
    ├── AppData Local
    │   └── %LOCALAPPDATA%\TechSmith
    │       = C:\Users\[Name]\AppData\Local\TechSmith
    │
    ├── ProgramData
    │   └── C:\ProgramData\TechSmith
    │
    └── Registry
        └── HKEY_CURRENT_USER\Software\TechSmith

MAC PATHS
    │
    ├── Application Support
    │   └── ~/Library/Application Support/TechSmith
    │
    └── Preferences
        └── ~/Library/Preferences/com.techsmith.*
```

---

*Generated for Pink Castle Foundation Kit - SWP3 Curriculum*
*Source: วิธีลบและติดตั้ง Camtasia 2018*
