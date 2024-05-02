<img align="right" src="beryllium.png" width="400" alt="Windows installation on beryllium">

# PocoF1 Windows Installation Guide [Without PC]

## ${\color{blue}Steps\space for\space installation}$ 
${\color{darkorange}1st\space Step - Partitioning}$

${\color{darkorange}2nd\space Step - Installation}$
#
### Prerequisites
- _A Working Brain (most important of all)_
- [_Moded Ofox Recovery_](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/download/Moded-Ofox-Recovery/ModedPE-Ofox-beryllium.zip)
- [_Windows ESD Image_](http://dl.delivery.mp.microsoft.com/filestreamingservice/files/48c0db41-e529-47bb-8049-b8d2f2708271/22631.2861.231204-0538.23H2_NI_RELEASE_SVC_REFRESH_CLIENTCONSUMER_RET_A64FRE_en-us.esd)
- [_Win Installer zip_](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/Win-Installar)

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
- Type ``` panel ``` and note down output. it is necessary to download installation file accordingly. 
- Reboot to check if Android still works.
- If Android doesn't boot, format userdata and Reboot.
#

### ${\color{darkorange}2nd\space Step - Installation}$
- Download [WinInstaller.zip](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/Win-Installar) according to your touch panel.
- Download [Windows ESD file](http://dl.delivery.mp.microsoft.com/filestreamingservice/files/48c0db41-e529-47bb-8049-b8d2f2708271/22631.2861.231204-0538.23H2_NI_RELEASE_SVC_REFRESH_CLIENTCONSUMER_RET_A64FRE_en-us.esd) it must be downloaded from this link and places in `Download` folder of your phone memory, else installation failed.
- Reboot to recovery flash Wininstaller.zip and wait till process complete.
- This will take some time. It will eventually reboot, and after that the initial setup (oobe) should launch.
#

#### ${\color{red}Note}$ :- If Sound and Rotation not working flash latest [UEFI](https://github.com/n00b69/woa-beryllium/releases/tag/UEFI) and it will start working.

#
### ${\color{darkorange}Last\space step\space -Dual\space Boot\ Setup}$
#### _Switch to Android_
- Navigate to C:\sta and create a shortcut of `sta.exe` to your desktop.
- Run the new shortcut on your desktop (you can also pin it to your start menu / taskbar for ease of access)
- If it prompt vcruntime140.dll error install [Microsoft Visual C++](https://aka.ms/vs/17/release/vc_redist.arm64.exe).
#### _Switch to Windows_
- Download and install the [WOA Helper app](https://github.com/Marius586/WoA-Helper-update/releases/tag/WOA), open it and grant root access.
- Download the [UEFI](https://github.com/n00b69/woa-beryllium/releases/tag/UEFI) image for your panel and place it inside the folder named `UEFI` in your internal storage.
- Return to the WOA Helper app and press the `Quickboot` button.
#### ${\color{red}Note}$ :- if above steps failed follow [this](https://github.com/n00b69/woa-beryllium/blob/main/guide/dualboot.md) guide
#























