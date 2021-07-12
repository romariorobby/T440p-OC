This hackintosh build using [Opencore](https://dortania.github.io/)
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
- Copy EFI to Mac Drive EFI/USB with [MountEFI](https://github.com/corpnewt/MountEFI)
- Generating [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)

## Audio Problem
- `cd T440P-OC/tools/ALCPlugFix/`
- Run this command

```bash
sudo spctl --master--disable
./install.sh
```

# TODO
- [ ] Shortcut Key (Brightness, Volume)
