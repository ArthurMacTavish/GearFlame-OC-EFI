# GearFlame-OC-EFI
OpenCore EFI for my Hardware

## PLEASE READ THIS FIRST
Just because your hardware are identical to mine, it doesn't mean you can just copy the EFI over and expect it to work. This is more to reference, so instead, I highly encourage you to go to [Dortania Install Guide](https://dortania.github.io/OpenCore-Install-Guide/) for detailed information.

## Hardware Configuration
- CPU: Intel Core i7-8700 (6 Cores - 12 Threads)
- GPU: [MSI Radeon RX580 8GB OC Edition](https://www.msi.com/Graphics-Card/Radeon-RX-580-ARMOR-8G-OC/)
- RAM: 2x8GB (2400 Mhz)
- Motherboard: [ASRock Z390-Pro4](https://www.asrock.com/mb/Intel/Z390%20Pro4/index.asp#Specification)
- Audio Codec: Realtek ALC892
- Ethernet Card: Intel Gigabit I219V
- Wifi/BT Card: TP-Link TL-WN722N v2
- BIOS revision: V. 4.30

## OpenCore Details ([V. 0.8.6](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.8.6))
- Guide: [Dortania Install Guide](https://dortania.github.io/OpenCore-Install-Guide/), it's really good, really.
- Kexts:
  - [Lilu](https://github.com/acidanthera/Lilu) (Helps with Patching)
  - [WhateverGreen](https://github.com/acidanthera/WhateverGreen) (GPU Patching)
  - [AppleALC](https://github.com/acidanthera/AppleALC) (For Audio)
  - [VirtualSMC, SMCProcessor & SMCSuperIO](https://github.com/acidanthera/VirtualSMC) (SMC Emulator Layer)
  - [IntelMausi](https://github.com/acidanthera/IntelMausi) (Ethernet Kext)
  - [RtWlanU & RtWlanI1827](https://github.com/chris1111/Wireless-USB-OC-Big-Sur-Adapter) (WiFi Kext)*
  - [HoRNDIS](https://github.com/jwise/HoRNDIS) (Enables Android USB Tethering Support)
  - [RadeonSensor & SMCRadeonGPU]() (Enables Temperature Monitoring in macOS)*
  
  \*Requires Apps or Additional Steps

## Things that aren't working
- Broken GPU Encoding (Decoding and DRM works fine, [details here](https://dortania.github.io/OpenCore-Post-Install/universal/drm.html))
- Audio doesn't working through Headphone Jack (HDMI works fine)
