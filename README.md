# ASROCK Z690M ITX/AX OpenCore EFI
OpenCore EFI directory for the ASRock Z690M-ITX/ax motherboard.


### Hardware tested

- ASRock Z690M-ITX/ax DDR4 motherboard.
- 12th gen Core i5 12400 and 13th gen Core i5 13400.
- 16GB x 2 3600 DDR4.
- Sapphire Pulse Radeon RX6600.
- WD SN570 1TB NVME SSD.
- 2TB SATA HDD as supplementary storage.


### OS Version Tested

- macOS Monterey 12.x
- macOS Ventura 13.1 (warning: Intel wifi kext in alpha stage!)


### BIOS

- Advanced -> CPU Configuration -> CFG Lock -> Disabled
- Advanced -> Chipset Configuration -> Above 4G Decoding -> Disabled
- Advanced -> Chipset Configuration -> C.A.M. (Clever Access Memory) -> Disabled
- Advanced -> Chipset Configuration -> IGPU Multi Monitor -> Disabled
- Security -> Secure Boot -> Secure Boot -> Disabled

### OpenCore version:

OpenCore: 0.8.3 Release


### Notes:
- You'll have to sey your own SMBIOS in config.plist.
- For CPU supporting E-cores you might want to tweak the SSDT sections in config.plist.
- If using using Broadcom wifi, disable the following Kexts in your config.plist: AirportItlwm, IntelBTPatcher, IntelBluetoothFirmware, BlueToolFixup.
- If using Intel wifi, I'd highly recomment to stay with Mojave for now.
