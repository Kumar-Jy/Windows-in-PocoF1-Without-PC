# PocoF1 Windows Installation [Without PC]
<img align="right" src="beryllium.png" width="400" alt="Windows installation on beryllium">

[![download](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/assets/20044626/3abc8b52-c5c6-4495-b623-d1312195d639)](https://youtu.be/e0fF1_bKQYE)
## ${\color{blue}Steps\space for\space Installation}$ 
- ${\color{darkorange}1st\space Step - Partitioning}$
- ${\color{darkorange}2nd\space Step - Installation}$
- ${\color{darkorange}3rd\space Step - Dual\space Boot}$
#
### Prerequisites
- _A Working Brain (most important of all)_
- [_Moded Ofox Recovery_](https://drive.google.com/file/d/1E8pkY7zLGfZJ0fAAoQr9GLnHf2y0n500/view?usp=drive_link)
- [_Win Installer zip_](https://drive.google.com/file/d/1MzfwyL2pDMEn1B6P9ma0ykun6TmM-pat/view?usp=drive_link)
#
### ${\color{red}[WARNING]}$
> - _All your data will be erased ! Back up now if needed._
> - _Backup Important Partition (Boot, EFS, Modem and Persist) and copy it to outside phone memory_
> - _Do not flash/run the same file/command twice unless specified._
> - _Follow step by step guide, don't jump or skip any step._
> - _YOU CAN BREAK YOUR DEVICE WITH THE COMMANDS/FILE BELOW IF YOU DO THEM WRONG!!!_
> - _DO NOT REBOOT YOUR PHONE! If you think you made a mistake, ask for help in the [Telegram chat](https://t.me/Kumar_Jy)._
#

### **${\color{darkorange}1st\space Step - Partitioning}$**
- Flash [Moded Ofox Recovery](https://drive.google.com/file/d/1E8pkY7zLGfZJ0fAAoQr9GLnHf2y0n500/view?usp=drive_link) either through your existing recovery or extract recovery.img from zip and flash through fastboot.
- Type ` partition $ ` on recovery terminal _[Replace $ with the size of storage in GB you want for Windows, Ex. - for 40GB type `partition 40`] (do not add GB at the end.)_
- If it asks you to run it once again, do so
- Reboot to check if Android still works. If it doesn't boot, format userdata and Reboot.
- #### ${\color{red}Note}$ :- 
> - if your phone encrypted first unmount and format userdata then type above command to creat partition.
> - If you partition table already modified first type ` restore ` then type above command to create new partition. 
#

### ${\color{darkorange}2nd\space Step - Installation}$
- Reboot to recovery and flash [WinInstaller.zip](https://drive.google.com/file/d/1MzfwyL2pDMEn1B6P9ma0ykun6TmM-pat/view?usp=drive_link) (_at least 6GB free space in phone memory required for flashing_)
- That's all , 
 You don't need to touch you phone just sit back and watch all installation process start automatically and phone will reboot to windows setup.
- #### ${\color{red}Note}$ :- 
> - For Sound and Rotation flash latest [UEFI](https://github.com/n00b69/woa-beryllium/releases/tag/UEFI) after windows setup.
> - Restore modem backup if cellular data not working.
> - Wininstallar automatically creates backup of boot, efs and modem so if you forgot to take backup just copy `backup` folder from phone storage or from `cache` folder to MemoryCard/PenDrive.
> - If you have to re-flash WinInstaller, first restore modem and android boot.img then flash wininstaller.zip
> - for any installation error visit _[troubleshooting](troubleshooting.md)_

#
### ${\color{darkorange}Last\space step\space -Dual\space Boot\ Setup}$
#### _Switch to Android_
- Navigate to `` C:\sta `` and Install ` VC.exe `
- create a shortcut of `sta.exe` to your desktop and Run it (you can also pin it to your start menu / taskbar for ease of access)
#### _Switch to Windows_
- Download and install the [WOA Helper app](https://github.com/Marius586/WoA-Helper-update/releases/tag/WOA), open it and grant root access.
- Download the [UEFI](https://github.com/n00b69/woa-beryllium/releases/tag/UEFI) image for your panel and place it inside the folder named `UEFI` in your internal storage.
- Return to the WOA Helper app and press the `Quickboot` button.
#### ${\color{red}Note}$ :- if above steps failed follow [this](https://github.com/n00b69/woa-beryllium/blob/main/guide/dualboot.md) guide
#
# _[Troubleshooting](troubleshooting.md)_






















