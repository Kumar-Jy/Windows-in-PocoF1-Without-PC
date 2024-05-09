<img align="right" src="beryllium.png" width="400" alt="Windows installation on beryllium">

# PocoF1 Windows Installation Guide [Without PC]

## ${\color{blue}Steps\space for\space Installation}$ 
${\color{darkorange}1st\space Step - Partitioning}$

${\color{darkorange}2nd\space Step - Installation}$

${\color{darkorange}3rd\space Step - Dual\space Boot}$
#
### Prerequisites
- _A Working Brain (most important of all)_
- [_Moded Ofox Recovery_](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/download/Moded-Ofox-Recovery/ModedPE-Ofox-beryllium.zip)
- [_Win Installer zip_](https://drive.google.com/file/d/1n1p0ih5tAtWOVgyR5vd7vsjs7by3PDuk/view?usp=drivesdk)

#
### ${\color{red}WARNING}$
> - _All your data will be erased ! Back up now if needed._
>
> - _Backup Important Partition (Boot, EFS, Modem and Persist) and copy it to outside phone memory_
>
> - _Do not flash/run the same file/command twice unless specified._
>
> - _Follow step by step guide, don't jump or skip any step._
> 
> - _YOU CAN BREAK YOUR DEVICE WITH THE COMMANDS/FILE BELOW IF YOU DO THEM WRONG!!!_
> 
> - _DO NOT REBOOT YOUR PHONE! If you think you made a mistake, ask for help in the [Telegram chat](https://t.me/WinOnF1)._
#


### **${\color{darkorange}1st\space Step - Partitioning}$**
- Flash [Moded Ofox Recovery](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/download/Moded-Ofox-Recovery/ModedPE-Ofox-beryllium.zip) either through your existing recovery or extract recovery.img from zip and flash through fastboot.
- Type ``` partition $ ``` on recovery terminal _[Replace $ with the size of storage in GB you want for Windows, Ex. - for 40GB type `partition 40` (do not add GB at the end.)_
- If it asks you to run it once again, do so 
- Reboot to check if Android still works. If it doesn't boot, format userdata and Reboot.
#

### ${\color{darkorange}2nd\space Step - Installation}$
- Reboot to recovery and flash [WinInstaller.zip](https://drive.google.com/file/d/1n1p0ih5tAtWOVgyR5vd7vsjs7by3PDuk/view?usp=drivesdk) (_at least 6GB free space in phone memory required for flashing_)
- That's all , 
 You don't need to touch you phone just sit back and watch all installation process start automatically and phone will reboot to windows setup.
#

#### ${\color{red}Note}$ :- If Sound and Rotation not working flash latest [UEFI](https://github.com/n00b69/woa-beryllium/releases/tag/UEFI) and it will start working.

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























