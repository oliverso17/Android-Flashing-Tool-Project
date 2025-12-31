# Android-Flashing-Tool-Project
disclamer "any damage made on your device is not my fault and im not gonna pay for it."

A tool inspired by popular unlock tools, with **ADB, Fastboot, Flash, Root, DM-Verity Fix** and more.

---

## ✨ Features
### Credits
- Made By @Oliverso17

### 📱 Device & Status
- Detect connected devices
- Detect ADB / Fastboot mode
- Detect Android version
- Restart ADB service

### 🔄 Reboot Options
- Reboot to system
- Reboot to recovery
- Reboot to bootloader (fastboot)
- Reboot to EDL (Qualcomm – if supported)

### 🔓 Unlock / Reset
- Factory reset (wipe data)
- Bootloader unlock (official)
- Bootloader relock
- Clear cache partition

### 💾 Flash & Repair
- Flash single image (boot / system / recovery / vendor)
- Flash all images from a folder
- Soft-brick fix (boot.img flash)
- Fastboot CDMS communication fix

### 🌱 Root
- Android 5–7 → Magisk ZIP (Recovery / Sideload)
- Android 8–10 → Magisk ZIP
- Android 11–12 → Patched boot.img
- Android 13+ → Patched boot.img
- Android version selection menu

### 🛠 Tools
- Screenshot capture
- Logcat capture
- Backup files (ADB pull)
- Push files to device (ADB push)
- Kill ADB / Fastboot processes

### 🛡 Security Fixes
- **DM-Verity Corruption Fix**
- Disable verity & verification via fastboot

---

## 🧩 DM-Verity Corruption Fix

If your device shows **“DM-Verity Corruption”**, use this method:

- Flash official or patched `boot.img`
- Disable verity & verification
- Clear cache and reboot

### Command used:
```bash
fastboot oem cdms fix
fastboot erase cache
fastboot reboot
