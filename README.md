# Asus TUF FX504GE OpenCore
[![GitHub version](https://img.shields.io/badge/OpenCore-0.5.9-brightgreen)](https://github.com/acidanthera/OpenCorePkg)

This is the files and configuration for setting up the ASUS TUF FX504GE laptop using OpenCore. I assume no responsibility from use of the files.

**Notes**
I use the Hackintosh primarily for music works. Currently I don't have much free time to tinker and optimize. But this first commit is pretty much ready to go reliably. You're going to lose some battery life too compared to Windows (I did make an SSDT for better frequency vectors. Needs testing though).

- MacOS Catalina 10.15.5
- 128 GB SATA SSD: Mac, 240 GB M.2 SSD: Windows. Both have their EFI partition (separate bootloaders, less worries. Esc to choose bootloader, go to OpenCore and boot Mac).
- I only use OpenCore to boot Mac. I advise against using one for Mac and Windows, since the latter often modifies the EFI partition when updating. Makes you going back and forth to restore the bootloader (for now).
- APFS partition
- Do not forget to take care of your own MLB, Serial Number, and UUID.

**BIOS Settings**
- Secure Boot: Disabled
- SATA mode: AHCI
- DVMT-Preallocated: 64MB

**Limitations**
- No onboard Wifi (not planning to buy a compatible card). I use a USB TP-Link one instead.
- Bluetooth not working (no wifi, no bluetooth).
- Trackpad not working (in progress. Using a USB mouse for now).
- ASUS Fn Keys (in progress).
- After shutdown process, the laptop will hang. Need to use power button to force turning off. It's fine though for now.
