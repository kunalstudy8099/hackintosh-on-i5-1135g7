<div align="center">

<img src="https://upload.wikimedia.org/wikipedia/commons/f/fa/Apple_logo_black.svg" width="70" alt="Apple logo" />

# 🍏 Hackintosh — macOS Sonoma on Lenovo IdeaPad 15ITS04

### ✅ Successful install of **macOS Sonoma 14.8.9** on an Intel 11th Gen Tiger Lake laptop

<p>
  <img src="https://img.shields.io/badge/macOS-Sonoma%2014.8.9-000000?style=for-the-badge&logo=apple&logoColor=white" alt="macOS Sonoma" />
  <img src="https://img.shields.io/badge/Bootloader-OpenCore-0B5FFF?style=for-the-badge&logo=apple&logoColor=white" alt="OpenCore" />
  <img src="https://img.shields.io/badge/Status-Working-2EA44F?style=for-the-badge" alt="Status Working" />
</p>

<p>
  <img src="https://img.shields.io/badge/CPU-Intel%20i5--1135G7-0071C5?style=flat-square&logo=intel&logoColor=white" alt="CPU" />
  <img src="https://img.shields.io/badge/iGPU-Iris%20Xe-0071C5?style=flat-square&logo=intel&logoColor=white" alt="GPU" />
  <img src="https://img.shields.io/badge/RAM-8GB%20DDR4-6E40C9?style=flat-square" alt="RAM" />
  <img src="https://img.shields.io/badge/SSD-Samsung-1428A0?style=flat-square&logo=samsung&logoColor=white" alt="SSD" />
  <img src="https://img.shields.io/badge/Laptop-Lenovo%20IdeaPad-E2231A?style=flat-square&logo=lenovo&logoColor=white" alt="Lenovo" />
</p>

<i>"It just works"... mostly. 😄</i>

</div>

---

## 📖 Table of Contents

- [🖥️ Hardware Specs](#️-hardware-specs)
- [🍎 System Info](#-system-info)
- [📊 What Works / What Doesn't](#-what-works--what-doesnt)
- [⚠️ Known Issues](#️-known-issues)
- [🛠️ Tools Used](#️-tools-used)
- [📸 Screenshot](#-screenshot)
- [🙏 Credits](#-credits)
- [⚖️ Disclaimer](#️-disclaimer)

---

## 🖥️ Hardware Specs

| Component | Details |
| :-- | :-- |
| 💻 **Laptop** | Lenovo IdeaPad 14ITS05 |
| 🧠 **CPU** | Intel® Core™ i5-1135G7 (11th Gen Tiger Lake, 4C/8T, 2.4 GHz) |
| 🎨 **iGPU** | Intel® Iris® Xe Graphics (Tiger Lake-LP GT2), 1536 MB |
| 🧮 **RAM** | 8 GB DDR4 @ 3200 MHz |
| 💾 **Storage** | Samsung NVMe SSD |
| 🖼️ **Display** | 15.6" Full HD (1920 × 1080) |
| 🚀 **Bootloader** | OpenCore |

## 🍎 System Info

| Item | Value |
| :-- | :-- |
| 🌄 **macOS** | macOS Sonoma **14.8.9** |
| 🏷️ **SMBIOS** | MacBook Pro (16-inch, 2019) |
| 🎨 **Graphics shown in macOS** | Intel Iris Xe Graphics (Tiger Lake-LP GT2) 1536 MB |
| 🧮 **Memory shown in macOS** | 8 GB 3200 MHz DDR4 |

> [!NOTE]
> Intel Iris Xe (Tiger Lake) has **no native support** in macOS. Graphics run with community patches and drivers. Expect some limits compared to a real Mac.

---

## 📊 What Works / What Doesn't

<div align="center">

### 🟢 Almost everything works! Only **3** things don't.

</div>

| Feature | Status | Notes |
| :-- | :--: | :-- |
| 🖥️ Booting macOS | ✅ | Boots fine with OpenCore |
| 🎨 Graphics / Display | ✅ | Full 1920 × 1080 |
| 🔆 Brightness Control | ✅ | Working |
| 📶 Wi-Fi | ✅ | Working |
| 🔊 Audio (Speakers / Headphones) | ✅ | Working |
| 🎤 Microphone | ✅ | Working |
| ⌨️ Keyboard | ✅ | Working |
| 🖱️ Trackpad | ❌ | **Not Working•• |
| 🔋 Battery Status | ✅ | Shows percentage |
| 🔌 USB Ports | ✅ | Working |
| 💾 Samsung NVMe SSD | ✅ | Working |
| ⚡ CPU Power Management | ✅ | Working |
| 🛍️ App Store / Software | ✅ | Working |
| 📷 Webcam | ❌  | Dont Know because mine is physically broken |
| 🖱️ Trackpad | ❌ | **Not Working•• |
| 😴 **Sleep / Wake** | ❌ | **Not working** |
| 🦷 **Bluetooth** | ❌ | **Not working** |
| 📡 **AirDrop** | ❌ | **Not working** |

<div align="center">

```
███████████████████████████████████████████████░░░░░  ~ 85% working
```

</div>

---

## ⚠️ Known Issues

<details>
<summary><b>😴 Sleep</b> — not working</summary>

<br>

The laptop does not sleep or wake properly. For now:
- Turn sleep off in **System Settings → Lock Screen / Battery**.
- Shut down instead of closing the lid when you are done.

</details>

<details>
<summary><b>🦷 Bluetooth</b> — not working</summary>

<br>

Bluetooth is not working on this build. Use a **USB dongle** or a wired mouse/keyboard for now.

</details>

<details>
<summary><b>📡 AirDrop</b> — not working</summary>

<br>

AirDrop needs Apple-compatible Wi-Fi + Bluetooth hardware. The stock card in this laptop is not supported for AirDrop or Continuity.
Swapping in a **Broadcom (Fenvi / BCM94360NG)** card is the usual fix.

</details>

---

## 🛠️ Tools Used

- 🚀 [**OpenCore**](https://github.com/acidanthera/OpenCorePkg) — bootloader
- 📘 [**Dortania's OpenCore Install Guide**](https://dortania.github.io/OpenCore-Install-Guide/)
- 🧰 [**OpenCore Configurator / ProperTree**](https://github.com/corpnewt/ProperTree) — config.plist editing
- 🔑 [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) — SMBIOS generation
- 🧩 [**Lilu**](https://github.com/acidanthera/Lilu) & [**WhateverGreen**](https://github.com/acidanthera/WhateverGreen)
- 📶 [**OpenIntelWireless**](https://github.com/OpenIntelWireless) — Intel Wi-Fi
- 💽 **ESP Mounter Pro** — mounting the EFI partition

---

## 📸 Screenshot

<div align="center">

<!-- Replace with your own screenshot: put it in the repo as screenshots/about.png -->
<img src="screenshots/about.png" width="720" alt="About This Mac — macOS Sonoma on Lenovo IdeaPad" />

<sub><i>About This Mac — macOS Sonoma 14.8.9 running on Lenovo IdeaPad 15ITS04</i></sub>

</div>

---

## 🙏 Credits

- 🍎 **Apple** — for macOS
- 🧪 [**Acidanthera**](https://github.com/acidanthera) — OpenCore, Lilu, WhateverGreen, AppleALC, VirtualSMC
- 📘 [**Dortania**](https://dortania.github.io/) — guides
- 📶 [**OpenIntelWireless**](https://github.com/OpenIntelWireless) — Intel Wi-Fi drivers
- 🌍 The whole **Hackintosh community** ❤️

---

## ⚖️ Disclaimer

> [!WARNING]
> This project is for **educational purposes only**. I am **not responsible** for any damage to your hardware or data. Running macOS on non-Apple hardware may break Apple's EULA. **Always back up your data first.**

> [!IMPORTANT]
> If you use this EFI, **create your own SMBIOS** (Serial, MLB, UUID) with GenSMBIOS. **Never share or reuse someone else's serial number.**
> download link https://drive.google.com/file/d/1plqEG7P_jc_ScRrj3r2svyYjkmtuP6rt/view?usp=drive_link

---

<div align="center">

### ⭐ If this helped you, please give the repo a star! ⭐

Made with ❤️ and lots of kernel panics 🍏💥

</div>
