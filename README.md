# HP ProBook 430 G5 OpenCore Configuration
OpenCore Configuration for running macOS Ventura on the HP ProBook 430 G5

## Versions
- macOS 13.4.1 Ventura
- OpenCore 0.9.3
- BIOS 01.24.00

## Hardware
- Intel Core i5-8250U (Coffe-Lake)
- Intel UHD 620 Graphics
- Conexant CX8200 Audio
- 16GB DDR4 2400MHz RAM
- 13.3 Full HD IPS Display
- Synaptics I2C TouchPad
- Intel Dual Band Wireless AC 8265
- Intel Bluetooth
- 2 USB 3.0 Ports, 1 USB Type-C Port
- HDMI Port
- Realtek SD-Card Reader
- Fingerprint Reader
- 256GB Kingston NVMe M.2 SSD (macOS)
- 2TB Samsung QVO 870 SATA SSD (Data)

## How to use?
- you can use this as a reference
- don't just copy & paste the EFI folder, instead you should read and understand the official OpenCore guide as things may change in the future
- also, don't forget to add your own SMBIOS data

### BIOS Settings
#### Before you start
- Main -> Apply Factory Defaults and Exit
- Security -> Restore Security Settings to Factory Defaults
- only then change the following settings: 
#### Security
- Enable System Management Command
#### Advanced -> Boot Options
- Disable Fast Boot
- Disable PXE Boot
- Disable Power On When Lid is Opened
#### Advanced -> Secure Boot Configuration
- Legacy Support Disable and Secure Boot Disable
#### Advanced -> System Options
- Enable VTx
- Disable VTd
- Enable Turbo Boost on DC
- Enable DPTF
- Enable HP Application Driver
#### Advanced -> Built-In Device Options
- Video memory size: 512MB
- Disable Lock Wireless Button
- Disable LAN / WLAN Auto Switching
- Disable Wake on WLAN
- Disable Fingerprint Device
#### Advanced -> Power Management Options
- Disable Wake on USB
- Enable Power Control

## What's working?
- almost everything

## What's not working?
- Fingerprint Reader
- you tell me?

## Credits
- https://github.com/kreizlie/HP-ProBook-430-G5-Hackintosh
- https://dortania.github.io/OpenCore-Install-Guide/
