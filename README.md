This hackintosh build using [Opencore 0.7.0](https://dortania.github.io/)
# Working
- Battery Info
- USB
- Webcam
- Graphic Accelaration
- Ethernet and Wifi
- Touchpad
- [Audio](#audio-problem)
# Untested
- Docking
- 

# Installation
- Clone with `git --recursive https://github.com/romariorobby/T440P-OC` to include all necessary tools `
- Copy `OC` Folder to Mac Drive EFI/USB with [MountEFI](https://github.com/corpnewt/MountEFI)
- Generating [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
  - cd `tools/GenSMBIOS` and `./GenSMBIOS.command`
  - Select Option `3` (Generating SMBIOS)
  - Type SMBIOS Model : ` ` but i'd recommended `MacbookPro11,1`
  - Open `config.plist`
  - Copy output of GenSMBIOS to `PlatformInfo > Generic` with the following:
    - Board Serial -> MLB
    - Type -> SystemProductName
    - Serial -> SystemSerialNumber
    - SmUUID -> SystemUUID

## Audio Problem
- `cd T440P-OC/tools/ALCPlugFix/`
- Run this command

```bash
sudo spctl --master--disable
./install.sh
```
- Reboot Your machine
## Fn Keys
To fix this you can install [ThinkpadAssistant](https://github.com/MSzturc/ThinkpadAssistant/releases/tag/v1.9.2.1)
## FHD Screen
If you have Full HD Screen. Install [One Key HiDPI](https://github.com/xzhih/one-key-hidpi)
## Customizing About This Mac

# TODO
- [X] Shortcut Key (Brightness, Volume)
