# PocoF1 Windows Installation [Without PC]
<img align="right" src="beryllium.png" width="300" alt="Windows installation on beryllium">

[![download](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/assets/20044626/3abc8b52-c5c6-4495-b623-d1312195d639)]()

[![telegram](https://img.shields.io/badge/chat-telegram-brightgreen.svg?logo=telegram&style=flat-square)](https://t.me/wininstaller)
#
## Prerequisites
- Unlocked bootloader
- Other Android Devices/Computer - ```for booting into modded recovery```
- USB otg cable - ``` for connecting your Android phone/Computer with your Poco F1```
#
### [WARNING]
> - _All your data will be erased ! Back up now if needed._
> - _Backup Boot, EFS, Modem and Persist and save it to outside phone memory_
> - _Do not flash/run the same file/command twice unless specified._
> - _Follow step by step guide, don't jump or skip any step._
> - _YOU CAN BREAK YOUR DEVICE WITH THE COMMANDS/FILE BELOW IF YOU DO THEM WRONG!!!_
> - _IF ANY ERROR, DO NOT REBOOT YOUR PHONE! just ask for help in the [Telegram chat](https://t.me/WinInstaller)._
#

### 1st Step - Partitioning
#### Perquisites :-
- *[Moddified-twrp/Ofox-Recovery](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/Modified-Recovery)* - Download in Other Android Phone/PC
- *[Magisk Manager](https://github.com/topjohnwu/Magisk/releases/tag/v29.0)* - Download into PocoF1

- Flash modded recovery using bugjager app or PC [``` fastboot flash recovery modded-recovery.img```] and install Magisk.zip - `If not already rooted`
- Must take backup of Boot, Modem, EFS and Persist and save it to outside of your phone memory.
- Open recovery terminal [```Advance - Terminal```] and type ` partition ` and If it asks you to "run it once again", do so .
- Enter the size of storage in GB you want for Windows and Reboot to system.
- If it failed to boot into Android, boot back to recovery and format userdata [``wipe-format-type`` **yes**]
- Setup Android and Install Magisk/KernalSU.apk
#

### 2nd Step - Installation
#### Perquisites :-
- [windows esd image](https://arkt-7.github.io/woawin/) [Do not use 24H2] 
- Download [WinInstaller.zip](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/PocoF1_WinInstaller)

- Download/Copy Windows ESD/WIM/ISO image and WinInstaller.zip.
- Boot to Modded-recovery and flash wininstaller.zip [```Install - Select Wininstaller.zip and Swip to Flash```]
- That's all , 
 You don't need to touch you phone just sit back and watch, all installation process start automatically and phone will reboot to windows setup.

- #### Notes :- 
> - If you have to re-flash/re-install it by-any reasons, type `format` recovery terminal then only you can install/flash,
> - Remove any attached usb device or charger before flashing, else it may be BSOD error.
> - Visit _[troubleshooting](troubleshooting.md)_ if any error.

#
### Last Step - Dual Boot Setup
#### _Switch to Android_
- Run `Android` Icon from windows desktop to boot into Android.
#### _Switch to Windows_
- Install Woa-Helper.apk from Download folder or download it from [here](https://github.com/n00b69/woa-helper/releases)], allow root permission, and press ``QUICKBOOT TO WINDOWS``.

# 
### Miscellaneous:-
#### _If change to new Android_ 
- You can install any Android Rom but must copy android boot.img of newly installed android to the windows partition.
- For creating backup of android boot.img on windows partition, first root it then boot to modded recovery - open terminal and type ``dd if=/dev/block/by-name/boot of=/win/boot.img`` .

#### _If format userdata_
- Download [Device Info HW app](https://play.google.com/store/apps/details?id=ru.andr7e.deviceinfohw&pcampaignid=web_share), and check your touch panel type
- Creat a folder in the phone storage and rename it to `UEF`  - Download [new-boot.img](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/UEFI-Boot-Image) according to your touch panel and place it in `UEFI` folder.
- Download and install the [WOA Helper app](https://github.com/n00b69/woa-helper/releases), open it and grant root access.
- Now you can boot to windows by pressing ``QUICKBOOT TO WINDOWS`` .

#### _Windows re-installation_
- Download WinInstaller.zip and Windows ESD file.
- Boot to modded recovery.
- open recovery terminal, type `format` and press enter (it will format previously installed windows)
- Now reboot to recovery again and flash Wininstaller.zip
#
# _[Troubleshooting](troubleshooting.md)_


## Support My Work

#### If you find my projects helpful, consider supporting my work! Your contributions will help me keep developing and sharing useful resources.

<p align="left">
  <a href="https://www.buymeacoffee.com/kumarjy" target="_blank">
    <img src="https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/blob/main/guide/buymecoffee.png" alt="Buy Me A Coffee" style="height: 60px !important; width: 217px !important;">
  </a>
</p>

