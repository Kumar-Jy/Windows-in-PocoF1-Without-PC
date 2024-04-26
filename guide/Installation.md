<img align="right" src="beryllium.png" width="300" alt="Windows installation on beryllium">

# PocoF1 Windows installation guide [Without PC]

## ${\color{lightblue}Steps\space for\space installation}$ 
${\color{orange}1st\space Step - Partitioning}$

${\color{orange}2nd\space Step - Installation}$
#
### Prerequisites
- _A Working Brain (most important of all)_
- [_Orange Fox Recovery_](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/download/Moded-Ofox-Recovery/Ofox-beryllium-pe.img)
- [_Windows ESD Image_](http://dl.delivery.mp.microsoft.com/filestreamingservice/files/48c0db41-e529-47bb-8049-b8d2f2708271/22631.2861.231204-0538.23H2_NI_RELEASE_SVC_REFRESH_CLIENTCONSUMER_RET_A64FRE_en-us.esd)
- [_Win Installer zip_](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/Win-Installar)

#
### ${\color{red}WARNING}$
> - _All your data will be erased ! Back up now if needed._
> 
> - _Do not run the same command twice unless specified._
>
> - _Follow step by step guide, don't jump or skip any steps_
> 
> - _YOU CAN BREAK YOUR DEVICE WITH THE COMMANDS BELOW IF YOU DO THEM WRONG!!!_
> 
> - _DO NOT REBOOT YOUR PHONE! If you think you made a mistake, ask for help in the [Telegram chat](https://t.me/WinOnF1)._
#


### _**${\color{orange}1st\space Step - Partitioning}$**_
- Flash [Ofox-beryllium-pe.img](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/download/Moded-Ofox-Recovery/Ofox-beryllium-pe.img) either through your existing recovery or through fastboot.
- Type ``` partition $ ``` on recovery terminal _[Replace $ with the size of storage in GB you want for Windows, example - for 40GB type `partition 40` (do not add GB at the end.)]_
- If it asks you to run it once again, do so
- type ``` panel ``` and note down output. it is necessary to download installation file accordingly. 
- Reboot to check if Android still works.
- If Android doesn't boot, format userdata and Reboot.
#

### _**${\color{orange}2nd\space Step - Installation}$**_
- Download [WinInstaller.zip](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/Win-Installar) according to your touch panel.
- Download [Windows ESD file](http://dl.delivery.mp.microsoft.com/filestreamingservice/files/48c0db41-e529-47bb-8049-b8d2f2708271/22631.2861.231204-0538.23H2_NI_RELEASE_SVC_REFRESH_CLIENTCONSUMER_RET_A64FRE_en-us.esd) it must be in `Download` folder of your phone memory and downloaded only from this link, else installation failed.
- Reboot to recovery flash Wininstaller.zip and wait till process complete.
- This will take some time. It will eventually reboot, and after that the initial setup (oobe) should launch.
#

#### _**${\color{yellow}Note}$** :- If Sound and Rotation not working flash latest [UEFI](https://github.com/n00b69/woa-beryllium/releases/tag/UEFI) and it will start working._

#
### _**${\color{orange}Last\space step\space -Dual\space Boot\ Setup}$**_
#### _Switch to Android_
- Navigate to C:\sta and create a shortcut of `sta.exe` to your desktop.
- Run the new shortcut on your desktop (you can also pin it to your start menu / taskbar for ease of access)
- If it prompt vcruntime140.dll error install [Microsoft Visual C++](https://aka.ms/vs/17/release/vc_redist.arm64.exe).
#### _Switch to Windows_
- Download and install the WOA Helper app, open it and grant root access.
- Download the [UEFI](https://github.com/n00b69/woa-beryllium/releases/tag/UEFI) image for your panel and place it inside the folder named `UEFI` in your internal storage.
- Return to the WOA Helper app and press the `Quickboot` button.
#### _**${\color{yellow}Note}$** :- if above steps failed follow [this](https://github.com/n00b69/woa-beryllium/blob/main/guide/dualboot.md) guide_
#






















