# ASROCK Z690M ITX/AX OpenCore EFI
OpenCore EFI for the ASRock Z690M-ITX/ax motherboard.<br/>
Current version: 0.9.7
## Overview

### Hardware tested
- ASRock Z690M-ITX/ax DDR4 motherboard.
- 12th gen Core i5 12400.
- 16GB x 2 3600 DDR4.
- Sapphire Pulse Radeon RX6600.
- WD Black SN770 2TB NVME SSD.
- 2TB SATA HDD as supplementary storage.


### OS Version Tested
- macOS Monterey 12.x
- macOS Ventura 13.1

### Working
- RX-6600 + with audio over HDMI.
- Built-in Audio (Realtek ALC897).
- Gigabit Ethernet (Intel I219V).
- 2.5Gbps Ethernet (Realtek RTL8125BG).
- Intel AX Wifi + Bluetooth (no airdrop)
- Broadcom BCM94360NG (optional replacement, airdrop support)
- Sleep
- Dual or Triple boot with Windows and Linux

### Not working
- Humanity making pretend efforts to reverse climate change. I'm serious.

## Instrunctions
### BIOS
Based on a default reset, change:
- Advanced -> CPU Configuration -> CFG Lock -> Disabled
- Advanced -> Chipset Configuration -> Above 4G Decoding -> Disabled
- Advanced -> Chipset Configuration -> C.A.M. (Clever Access Memory) -> Disabled
- Advanced -> Chipset Configuration -> IGPU Multi Monitor -> Disabled
- Security -> Secure Boot -> Secure Boot -> Disabled


### config.plist:
- Set MLB, SystemSerialNumber and SystemUUID.
- For CPU with E-cores you might want to tweak the SSDT sections.
- If using the Broadcom wifi card, disable or remove the following Kexts in your config.plist: AirportItlwm, IntelBTPatcher, IntelBluetoothFirmware, BlueToolFixup.
