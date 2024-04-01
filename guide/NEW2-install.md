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
  
  
#### Copy Installation File
> Download [windowsARM](https://worproject.com/esd) and copy to Internal Storage -> Windows folder
> 
> unzip [Driver.zip](https://drive.google.com/file/d/1YBK2fTmgmhzCaPg5luq-GJyGnM6i94Rf/view?usp=drivesdk) and copy to Internal Storage -> Windows folder
> 
> unzip [WinPE.zip](https://drive.google.com/file/d/1lfRh5zd3pcaA7Z9WRsF5FM39NuIbZesS/view?usp=sharing) open folder and copy all file to Internal Storage -> Winpe folder
 

#### Backup Importent Pertition
Use the recovery backup feature to backup boot, EFS, Modem, Persist.


#### Running WinPe
> Reboot to recovery - flash - *bootPE....img* on boot partition (from Download Folder) - reboot to systen
> Select  *UEFI OS on #4*  by pressing vol up and press power button to continue boot.


### Windows installation
> Now you are on winpe.
> 
> Connect Mouse - open Dism++ (from C Drive - other - dism++(Arm64))
> 
> File - Apply image - select install.esd (D Drive) -
>
> select target Image - select installation Path (D Drive) -  Add Boot - OK - let it complete)
> 
> Click on open Sesion - Drivers - Add -
>
> Select Driver Folder ( from D Drive) after driver installation completed, close dism++
> 
> Open C Drive - other - right click on miscfix.bat and run as administrator, let it complete.
>
> It will automatically shutdown.
> 
> Your Windows Installation completed.


#### Boot into Windows
> Press Power + Vol Up - Reboot to recovery - flash - *setup....img* on boot partition - reboot to systen


### Setting up Windows
Your device will now set up Windows. This will take some time. It will eventually reboot, and after that the initial setup (oobe) should launch.

> [!Note]
> To skip the Microsoft Account login, use "g" for the email and password. Windows will then let you make a local account

## [Last step: Setting up dualboot](/guide/dualboot.md)
















