<img align="right" src="beryllium.png" width="350" alt="Windows installation on beryllium">


# Windows installation guide for PocoF1

## Installing Windows

### Prerequisites

- [Windows on ARM esd](https://worproject.com/esd)

- [WinPE](https://drive.google.com/file/d/1lfRh5zd3pcaA7Z9WRsF5FM39NuIbZesS/view?usp=sharing)
  
- [BootPE image tianma nvt](pe-tianma-nvt.img)

- [BootPE image edbg fts](pe-edbg-fts.img)

- [Windows Setup image tianma nvt](Setup-tianma-nvt.img)

- [Windows Setup image edbg fts](Setup-edbg-fts.img)
  
- [Drivers](https://drive.google.com/file/d/1YBK2fTmgmhzCaPg5luq-GJyGnM6i94Rf/view?usp=drivesdk)

  
  
#### Checking Touchscreen panel type
> Install [Device Info HW app](https://play.google.com/store/apps/details?id=ru.andr7e.deviceinfohw&pcampaignid=web_share) - open and go to genral - Tuchscreen it should be *NVT-ts* of *FTS-ts*
>
>  you can check it through recovery terminal also 
```cmd
adb shell dmesg | grep dsi_display_bind
```
> This should output either `dsi_ebbg_fhd_ft8719_video_display` or `dsi_tianma_fhd_nt36672a_video_display`
>
> Download all boot image file accordingly.
  
#### Mount windows and WinPE Partition on Android
> Install Magisk and root your android if not already rooted
> 
>  Open magisk manager app and flash [mountmodule.zip](mountmodule.zip)
>
> Reboot and check two new folder (Windows and Winpe) created on your internal storage


#### Copy Installation File
> Download [windowsARM](https://worproject.com/esd) , rename it to install.esd and copy to Internal Storage -> Windows folder
> 
> unzip [Driver.zip](https://drive.google.com/file/d/1YBK2fTmgmhzCaPg5luq-GJyGnM6i94Rf/view?usp=drivesdk) and copy to Internal Storage -> Winpe folder
> 
> unzip [WinPE.zip](https://drive.google.com/file/d/1lfRh5zd3pcaA7Z9WRsF5FM39NuIbZesS/view?usp=sharing) open folder and copy all file to Internal Storage -> Winpe folder
 

#### Backup Importent Pertition
Reboot to Recovery and take backup of boot, EFS, Modem and Persist.


#### Running WinPe
> Reboot to recovery - flash - *bootPE....img* on boot partition (from Download Folder) - reboot to systen

> Select  *UEFI OS on #4*  by pressing vol up and press power button to continue boot.


### Windows installation
> Now you are on winpe.
> 
> Connect Keyboard/Mouse - open Dism++ (from C Drive - other - dism++(Arm64))
> 
> Open File - Apply image -
> enter the path of esd file or you can Browse and select D Drive
```cmd
D:\
```
> Change Target Image as per your requirment.
>
> enter Installation Drive Path or you can Browse and select D Drive
```cmd
D:\install.esd
```

> Check Add Boot and click OK - let windows install.
>
>
### Driver installation
> Click on open Sesion - Drivers - Add -
>
> Select Driver Folder ( from C Drive) let it completed, and close dism++
> 
> Open C Drive - other - right click on miscfix.bat and run as administrator, let it complete.
>
> It will automatically shutdown.
> 
> Your Windows and Driver Installation completed.


#### Boot into Windows
> Press Power + Vol Up - Reboot to recovery - flash - *setup....img* on boot partition - reboot to systen


### Setting up Windows
Your device will now set up Windows. This will take some time. It will eventually reboot, and after that the initial setup (oobe) should launch.

> [!Note]
> To skip the Microsoft Account login, use "g" for the email and password. Windows will then let you make a local account

## [Last step: Setting up dualboot](/guide/dualboot.md)
















