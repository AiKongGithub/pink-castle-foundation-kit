# Data Tables: วิธีลบและติดตั้ง Camtasia 2018 ใหม่

**Production ID:** VIDEO-016-DATA
**Format:** Data Tables Collection
**Source:** วิธีลบและติดตั้ง Camtasia 2018

---

## Table 1: Symptoms Requiring Reinstall

| Symptom | Description | Severity | Try First |
|---------|-------------|----------|-----------|
| Frequent Crashes | โปรแกรมปิดเองบ่อย | High | Restart, Update drivers |
| Error Messages | Error ขึ้นบ่อยโดยไม่มีเหตุผล | High | Clear cache |
| Features Not Working | บาง function ใช้ไม่ได้ | Medium | Run as Admin |
| Performance Degradation | ช้าลงมากผิดปกติ | Medium | Check disk space |
| Update Failures | อัพเดทไม่สำเร็จ | Medium | Manual download |
| Corrupted Interface | UI แสดงผลผิดปกติ | High | Graphics driver |
| Audio/Video Sync Issues | เสียง/ภาพไม่ตรงกัน | Medium | Reinstall codecs |

---

## Table 2: Pre-Reinstall Troubleshooting

| Solution | Success Rate | Time Required | Difficulty |
|----------|--------------|---------------|------------|
| Restart Computer | 20% | 2-5 min | Easy |
| Update Graphics Driver | 30% | 10-30 min | Medium |
| Clear Temp Files | 35% | 5-10 min | Easy |
| Run as Administrator | 25% | 2 min | Easy |
| Check Disk Space | 15% | 5 min | Easy |
| Disable Antivirus | 25% | 5 min | Easy |
| **Clean Reinstall** | **90%** | **30-60 min** | **Medium** |
| Contact Support | 95% | Variable | N/A |

---

## Table 3: Items to Backup Before Uninstall

| Item | Location | Priority | Notes |
|------|----------|----------|-------|
| Project Files (.tscproj) | Documents\Camtasia | Critical | Main work files |
| Media Files | Various | Critical | Video, audio, images |
| License Key | TechSmith Account | Critical | Required for activation |
| Custom Presets | %APPDATA%\TechSmith | Medium | Transitions, callouts |
| Templates | %APPDATA%\TechSmith | Medium | Custom templates |
| Preferences | %APPDATA%\TechSmith | Low | Settings, shortcuts |

---

## Table 4: License Key Locations

| Source | Path/URL | Notes |
|--------|----------|-------|
| In Application | Help > About Camtasia | Shows partial key |
| TechSmith Account | techsmith.com > My Account > Licenses | Full key available |
| Purchase Email | Search "TechSmith" or "Camtasia" | Original purchase |
| Registration Confirmation | Email from TechSmith | Sent after registration |

---

## Table 5: Standard Uninstall Steps (Windows)

| Step | Action | Time | Details |
|------|--------|------|---------|
| 1 | Open Settings | 5 sec | Win + I |
| 2 | Navigate to Apps | 5 sec | Apps > Apps & Features |
| 3 | Search Camtasia | 10 sec | Use search box |
| 4 | Select Camtasia | 5 sec | Click the entry |
| 5 | Click Uninstall | 5 sec | Confirm when prompted |
| 6 | Wait for completion | 2-5 min | Do not interrupt |
| **Total** | - | **~5 min** | Standard only |

---

## Table 6: Leftover Files to Delete (Windows)

| Location | Path | Contains | Size |
|----------|------|----------|------|
| AppData Roaming | %APPDATA%\TechSmith | User prefs, presets | ~50-200 MB |
| AppData Local | %LOCALAPPDATA%\TechSmith | Cache, temp files | ~100-500 MB |
| ProgramData | C:\ProgramData\TechSmith | Shared app data | ~10-50 MB |
| Registry (Optional) | HKEY_CURRENT_USER\Software\TechSmith | App settings | N/A |

---

## Table 7: Leftover Files to Delete (macOS)

| Location | Path | Contains |
|----------|------|----------|
| Application Support | ~/Library/Application Support/TechSmith | App data, presets |
| Preferences | ~/Library/Preferences/com.techsmith.* | Settings |
| Caches | ~/Library/Caches/com.techsmith.* | Cache files |
| Logs | ~/Library/Logs/TechSmith | Log files |

---

## Table 8: Windows Quick Commands

| Command (Win+R) | Opens | Purpose |
|-----------------|-------|---------|
| %APPDATA% | AppData\Roaming folder | Delete TechSmith folder |
| %LOCALAPPDATA% | AppData\Local folder | Delete TechSmith folder |
| appwiz.cpl | Programs and Features | Alternative uninstall |
| regedit | Registry Editor | Clean registry (advanced) |
| msconfig | System Configuration | Clean boot |
| control | Control Panel | System settings |

---

## Table 9: Reinstall Steps

| Step | Action | Time | Notes |
|------|--------|------|-------|
| 1 | Download from techsmith.com | 5-15 min | Always download fresh |
| 2 | Run installer | 30 sec | Accept UAC |
| 3 | Accept License | 30 sec | Read and accept |
| 4 | Choose Typical | 10 sec | Recommended |
| 5 | Installation | 5-10 min | Varies by system |
| 6 | Activate License | 1-2 min | Enter key or login |
| 7 | Check Updates | 2-5 min | Install if available |
| **Total** | - | **~20-35 min** | - |

---

## Table 10: Post-Reinstall Verification

| Test | How to Verify | Expected Result |
|------|---------------|-----------------|
| Launch | Double-click shortcut | Opens without error |
| Screen Recording | Click Record, capture 10 sec | Recording works |
| Webcam | Enable webcam in recorder | Video visible |
| Audio | Record with mic | Audio captured |
| Import | File > Import Media | Files import correctly |
| Timeline | Drag media to timeline | Media appears |
| Effects | Apply transition | Effect works |
| Export | Share > Local File | Video exports correctly |

---

## Table 11: Common Post-Reinstall Issues

| Issue | Cause | Solution |
|-------|-------|----------|
| License invalid | Not deactivated from old install | Deactivate via account |
| Recording fails | Permission denied | Run as Administrator |
| Black screen | Graphics driver issue | Update GPU driver |
| No audio | Wrong device selected | Check audio settings |
| Still crashes | Incomplete clean | Delete ALL TechSmith folders |
| Slow performance | Background processes | Close other apps |
| Export fails | Insufficient disk space | Free up space |

---

## Table 12: Troubleshooting Solutions

| Solution | When to Use | Steps |
|----------|-------------|-------|
| Run as Administrator | Permission errors | Right-click > Run as Admin |
| Compatibility Mode | Old system issues | Properties > Compatibility > Windows 8 |
| New User Profile | Profile corruption | Create new Windows user |
| Safe Mode | Software conflicts | Boot to Safe Mode |
| Clean Boot | Service conflicts | msconfig > Selective startup |
| Graphics Driver Update | Display/rendering issues | Download from Intel/NVIDIA/AMD |
| Disable Antivirus | AV blocking Camtasia | Temporarily disable or whitelist |

---

## Table 13: Clean Reinstall Complete Checklist

| Phase | Step | Completed |
|-------|------|-----------|
| **BACKUP** | Backup Project files | [ ] |
| | Backup Media files | [ ] |
| | Note License Key | [ ] |
| | Backup Custom Presets | [ ] |
| **UNINSTALL** | Standard uninstall via Settings | [ ] |
| | Delete %APPDATA%\TechSmith | [ ] |
| | Delete %LOCALAPPDATA%\TechSmith | [ ] |
| | Delete C:\ProgramData\TechSmith | [ ] |
| | Empty Recycle Bin | [ ] |
| | Restart Computer | [ ] |
| **REINSTALL** | Download latest installer | [ ] |
| | Run installer | [ ] |
| | Choose Typical installation | [ ] |
| | Wait for completion | [ ] |
| | Activate License | [ ] |
| | Check for Updates | [ ] |
| **VERIFY** | Test Screen Recording | [ ] |
| | Test Import | [ ] |
| | Test Export | [ ] |
| | Restore Custom Presets | [ ] |

---

## Table 14: Time Estimates

| Phase | Minimum Time | Maximum Time | Notes |
|-------|--------------|--------------|-------|
| Backup | 5 min | 30 min | Depends on project count |
| Standard Uninstall | 2 min | 5 min | - |
| Clean Leftover | 5 min | 15 min | Including registry |
| Restart | 1 min | 3 min | - |
| Download | 5 min | 20 min | Depends on internet |
| Installation | 5 min | 10 min | - |
| Activation | 1 min | 5 min | - |
| Verification | 5 min | 15 min | - |
| **Total** | **30 min** | **90 min** | - |

---

## Table 15: Support Resources

| Resource | URL | Best For |
|----------|-----|----------|
| TechSmith Support | support.techsmith.com | Official help |
| Knowledge Base | techsmith.com/learn | Self-service solutions |
| Community Forum | feedback.techsmith.com | Peer assistance |
| Video Tutorials | YouTube "TechSmith Camtasia" | Visual learning |
| Contact Form | support.techsmith.com/contact | Direct support |

---

## Summary Statistics

| Metric | Value |
|--------|-------|
| Clean Reinstall Success Rate | 90% |
| Standard Uninstall Time | 2-5 minutes |
| Clean Uninstall Time | 10-20 minutes |
| Reinstall Time | 15-30 minutes |
| Total Process Time | 30-60 minutes |
| Folders to Delete (Windows) | 3 |
| Folders to Delete (macOS) | 3-4 |

---

*Generated for Pink Castle Foundation Kit - SWP3 Curriculum*
*Source: วิธีลบและติดตั้ง Camtasia 2018*
