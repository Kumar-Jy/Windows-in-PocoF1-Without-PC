<img align="right" src="beryllium.png" width="350" alt="Windows installation on beryllium">

# Windows installation guide for PocoF1

## Installing Windows

### Prerequisites
- [Windows on ARM esd](https://worproject.com/esd)

- [WinPE](https://drive.google.com/file/d/1ROmr2ki69QigIVFXJV5fRRSSd7K6h17D/view?usp=drive_link)
  
- [PE boot image tianma nvt](pe-tianma-nvt.img)

- [PE boot image edbg fts](pe-ebbg-fts.img)

- [Windows boot image tianma nvt](Setup-tianma-nvt.img)

- [Windows boot image ebbg fts](setup-ebbg-fts.img)
  
- [Drivers](https://drive.google.com/file/d/1YBK2fTmgmhzCaPg5luq-GJyGnM6i94Rf/view?usp=drivesdk)

### Checking Touchscreen panel type
- Install [Device Info HW app](https://play.google.com/store/apps/details?id=ru.andr7e.deviceinfohw&pcampaignid=web_share)
- Go to **General** > **Touchscreen**.
- You should either see **NVT-ts** of **FTS-ts**

> You can check it through recovery terminal also 
```cmd
adb shell dmesg | grep dsi_display_bind
```
> This should output either `dsi_ebbg_fhd_ft8719_video_display` or `dsi_tianma_fhd_nt36672a_video_display`
>
> Download all boot image file accordingly.
  
### Mount Windows and WinPE Partition on Android
> Make sure Windows and Winpe folder are already mounted using the module on the previous page

#### Copy Installation File
- Download [windowsARM](https://worproject.com/esd), rename it to install.esd, and copy it to Internal Storage > Windows
- Unzip [Driver.zip](https://drive.google.com/file/d/1YBK2fTmgmhzCaPg5luq-GJyGnM6i94Rf/view?usp=drivesdk) and copy it to Internal Storage > Windows > Driver
- Unzip [WinPE.zip](https://drive.google.com/file/d/1lfRh5zd3pcaA7Z9WRsF5FM39NuIbZesS/view?usp=sharing) and copy all internal files/folder from it to Internal Storage -> Winpe
> [!Note]
> Be sure all copyed file/folder is in the right place and name must be exectly as mentioned above. otherwize installation process will not work.
 
#### Backup important partitions
Reboot to Recovery and make a backup of boot, EFS, Modem and Persist.

### Running WinPe
- In your recovery, flash **PEboot image** to your boot partition, then reboot.
- Select  *UEFI OS on #4*  by pressing vol up and press power button to continue boot.

### Windows and Driver installation
> Once in Winpe, type ``` C:\install ``` on opennd command prompt and press enter
```cmd
C:\install
```
- Installation process started . After it automatically shutdown.

#### Boot into Windows
- Press Power + Vol Up to reboot to recovery
- Flash > **setup Windows image file** to the boot partition and reboot your device
- Windows installation process has been completed now.

### Setting up Windows
Your device will now set up Windows. This will take some time. It will eventually reboot, and after that the initial setup (oobe) should launch.

> [!Note]
> To skip the Microsoft Account login, use "g" for the email and password. Windows will then let you make a local account
> If Sound and Rotation not working reboot to recovery and flash latest UEFI(https://github.com/n00b69/woa-beryllium/releases/tag/UEFI) on boot partition and it will start working.

## [Last step: Setting up dualboot](/guide/dualboot.md)













