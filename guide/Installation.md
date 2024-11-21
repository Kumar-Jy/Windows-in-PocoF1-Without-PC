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
- Flash [Modified Recovery](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/Modified-Recovery).
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
- Download [windows esd image](https://arkt-7.github.io/woawin/) (It must be in Download folder of your phone memory)
- Download [WinInstaller.zip](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/PocoF1_WinInstaller)
- Reboot to recovery and flash it (_at least 6GB free space in phone memory required for flashing_)
- That's all , 
 You don't need to touch you phone just sit back and watch, all installation process start automatically and phone will reboot to windows setup.
- #### Notes :- 
> - Must format windows partition by typing `format` command on recovery terminal, If you have to re-flash it by-any reasons or there is already windows installed.
> - Remove any attached usb device or charger before flashing, else it may be BSOD error.
> - Visit _[troubleshooting](troubleshooting.md)_ if any error.

#
### Last Step - Dual Boot Setup
#### _Switch to Android_
- Run `Android` Icon from windows desktop to boot into Android.
#### _Switch to Windows_
- Open WOA Helper app (Install it and grant root access, if not already installed) and press ``QUICKBOOT TO WINDOWS``, it will boot in windows.

# 
### Miscellaneous:-
#### _If change to new Android_ 
- You can install any Android Rom but must copy android boot.img of newly installed android to the windows partition.
- For creating backup of android boot.img on windows partition, first root it then boot to modded recovery - open terminal and type ``dd if=/dev/block/by-name/boot of=/win/boot.img`` .

#### _If format userdata_
- Download [Device Info HW app](https://play.google.com/store/apps/details?id=ru.andr7e.deviceinfohw&pcampaignid=web_share), and check your touch panel type
- Creat a folder in the phone storage and rename it to `UEF`  - Download [new-boot.img](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/UEFI-Boot-Image) according to your touch panel and place it in `UEFI` folder.
- Download and install the [WOA Helper app](https://github.com/Marius586/WoA-Helper-update/releases/tag/WOA), open it and grant root access.
- Now you can boot to windows by pressing ``QUICKBOOT TO WINDOWS`` .

#### _Windows re-installation_
- Download WinInstaller.zip and Windows ESD file.
- Boot to modded recovery as per your rom.
- open recovery terminal, type `format` and press enter (it will format previously installed windows)
- Now flash Wininstaller.zip
#
# _[Troubleshooting](troubleshooting.md)_
