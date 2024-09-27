# PocoF1 Windows Installation [Without PC]
<img align="right" src="beryllium.png" width="350" alt="Windows installation on beryllium">

[![download](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/assets/20044626/3abc8b52-c5c6-4495-b623-d1312195d639)]()
## Steps for Installation
- 1st Step - Partitioning
- 2nd Step - Installation
- 3rd Step - Dual Boot
#
### Prerequisites
- _A Working Brain (most important of all)_

- _Unlocked bootloader_ 

- _Rooted and Installed Custom Recovery_
#
### [WARNING]
> - _All your data will be erased ! Back up now if needed._
> - _Backup Important Partition (Boot, EFS, Modem and Persist) and copy it to outside phone memory_
> - _Your phone must be rooted, if it is not, follow [root](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/blob/main/guide/root.md) guide before start the process._
> - _Do not flash/run the same file/command twice unless specified._
> - _Follow step by step guide, don't jump or skip any step._
> - _YOU CAN BREAK YOUR DEVICE WITH THE COMMANDS/FILE BELOW IF YOU DO THEM WRONG!!!_
> - _DO NOT REBOOT YOUR PHONE! If you think you made a mistake, ask for help in the [Telegram chat](https://t.me/WinInstaller)._
#

### 1st Step - Partitioning
- Flash [Modded Ofox Recovery](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/Moded-Ofox-Recovery) either through your existing recovery or extract recovery.img from zip and flash through fastboot.
- Type ` partition $ ` on recovery terminal _[Replace $ with the size of storage in GB you want for Windows, Ex. - for 40GB type `partition 40`] (do not add GB at the end.)_
- If it asks you to run it once again, do so
- Reboot to check if Android still works. If it doesn't boot, format userdata and Reboot.
- Root it (if not already rooted), Install Magisk/KernalSU
- Download and install the [WOA Helper app](https://github.com/Marius586/WoA-Helper-update/releases/tag/WOA), open it and grant root access.
- #### Notes :- 
> - if your phone encrypted first unmount and format userdata then type above command to create partition.
> - If you already modified or installed Windows, first type ` restore ` then type above command to create new partition. 
#

### 2nd Step - Installation
- Download windows esd image of your choice from [here](https://arkt-7.github.io/woawin/)
- Download [WinInstaller.zip](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/PocoF1_WinInstaller)
- Reboot to recovery and flash it (_at least 6GB free space in phone memory required for flashing_)
- That's all , 
 You don't need to touch you phone just sit back and watch, all installation process start automatically and phone will reboot to windows setup.
- #### Notes :- 
> - Must remove any attached usb device or charger before flashing, or it may be BSOD error.
> - for any installation error visit _[troubleshooting](troubleshooting.md)_

#
### Last Step - Dual Boot Setup
#### _Switch to Android_
- Run `Android` Icon from windows desktop to boot into Android.
#### _Switch to Windows_
- Open WOA Helper app (Install it and grant root access, if not already installed) and press ``QUICKBOOT TO WINDOWS``, it will boot in windows.
 
#### Notes :- 
> - whenever you install new Android Rom, must creat backup of boot.img of newly installed android.
> - for creating backup , open Woa Helper app, graant root access - First tap on ``MOUNT WINDOWS`` then tape on `` BACKUP BOOT IMAGE `` and select ``WINDOWS`` .
#
# _[Troubleshooting](troubleshooting.md)_






















