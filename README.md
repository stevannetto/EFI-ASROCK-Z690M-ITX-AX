# EFI-ASROCK-Z690M-ITX-AX
EFI Setup for the 12th gen Intel Alder Lake in a ASRock Z690M-ITX/ax DDR4 motherboard.


### Hardware tested

- ASRock Z690M-ITX/ax DDR4 motherboard.
- 12th gen Core i5 12400.
- 16GB x 2 3600 DDR4 Klevv Cras X RGB memory kit.
- Sapphire Pulse Radeon RX6600.
- WD SN570 1TB NVME SSD.
- 2TB SATA HDD.


### OS Version Tested

- macOS Monterey 12.x


### BIOS

- Advanced -> CPU Configuration -> CFG Lock -> Disabled
- Advanced -> Chipset Configuration -> Above 4G Decoding -> Disabled
- Advanced -> Chipset Configuration -> C.A.M. (Clever Access Memory) -> Disabled
- Security -> Secure Boot -> Secure Boot -> Disabled

### OpenCore version:

OpenCore: 0.8.3 Release


### Notes:

- For CPU supportin E-cores you might edit the SSDTs in config.plist.
- Both the integrated Intel AX wifi or Fenvi Broadcom cards should work fine. 
