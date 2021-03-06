# Asus TUF FX504GE OpenCore
[![GitHub version](https://img.shields.io/badge/OpenCore-0.6.1-brightgreen)](https://github.com/acidanthera/OpenCorePkg)

This is the files and configuration for setting up the ASUS TUF FX504GE laptop using OpenCore. I assume no responsibility from use of the files.

OpenCore EFI file and Shell included. Basically you could just download, copy, paste, modify few things, and use.

I use the Hackintosh primarily for music works. Currently I don't have much free time to tinker and optimize. This is my second commit going through OpenCore 0.6.1. Note that you're going to see your battery performs worse compared to Windows (I did make an SSDT for better frequency vectors suited to works I do). I do plug all the time when using MacOS though.


- MacOS Catalina 10.15.6 (10.15.4-10.15.6)
- 128 GB SATA SSD: Mac, 240 GB M.2 SSD: Windows. Both have their EFI partition (separate bootloaders, less worries. Esc to choose bootloader, go to OpenCore and boot Mac).
- I only use OpenCore to boot Mac. Easiest and works for me. Windows often modifies the EFI partition when updating. I know there's a way to prevent this. I'm just using the simplest solution.
- APFS partition.
- Please take care of your own MLB, Serial Number, and UUID.

**Few Highlights**
- ASUS Fn Keys (brightness keys mapped incorrectly. No plan to fix).
- Trackpad not working (in progress. Using a USB mouse for now).
- Audio: ALC255 (layout 3)

**BIOS Settings**
- Secure Boot: Disabled
- SATA mode: AHCI
- DVMT-Preallocated: 64MB

**Limitations**
- No onboard Wifi (going to use a compatible one when I got some spare time). Using a USB TP-Link one.
- Bluetooth not working (no wifi, no bluetooth).
- After shutdown process, the laptop will hang. Need to use power button to force turning off. It's fine though for now.
- Still a lot to do (https://dortania.github.io/OpenCore-Post-Install/)

![Image of CPU](https://github.com/felixyonathan/Asus-TUF-FX504GE-OpenCore/raw/master/CPU.png)
![Image of OpenCL](https://github.com/felixyonathan/Asus-TUF-FX504GE-OpenCore/raw/master/OpenCL.png)
