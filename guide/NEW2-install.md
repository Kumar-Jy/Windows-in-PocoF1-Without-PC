<img align="right" src="beryllium.png" width="350" alt="Windows 11 running on beryllium">


# Running Windows on the Xiaomi Pocophone F1

## Installing Windows

### Prerequisites

- [Windows on ARM esd](https://worproject.com/esd)

- [WinPE](https://drive.google.com/file/d/1q2jijIKCF7xuFUX0J2SjYfo7nDvRAyOE/view?usp=sharing)
  
- [BootPE image tianma nvt](pe-tianma-nvt.img)

- [BootPE image edbg fts](pe-edbg-fts.img)

- [Windows Setup image tianma nvt](Setup-tianma-nvt.img)

- [Windows Setup image edbg fts](Setup-edbg-fts.img)
  
- [Drivers](https://github.com/n00b69/woaberyllium/releases/tag/Drivers)

  
  
#### Checking Touchscreen panel type
> Install *Device Info HW app* - open and go to genral - Tuchscreen it should be *NVT-ts* of *FTS-ts*
>
>  you can check it through recovery terminal also 
```cmd
adb shell dmesg | grep dsi_display_bind
```
> This should output either `dsi_ebbg_fhd_ft8719_video_display` or `dsi_tianma_fhd_nt36672a_video_display`
>
> Download all boot image file accordingly.
  
  
#### Copy Installation File
> Copy windows esd file to Internal Storage -> Windows folder
> 
> unzip Driver.zip and copy to Internal Storage -> Windows folder
> 
> unzip WinPE.zip open folder and copy all file to Internal Storage -> Winpe folder
 

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
> apply image (File - Apply image - select install.esd (D Drive) -
>
>  select target Image - select installation Path (D Drive) - Add Boot - OK - let it complete)
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
















