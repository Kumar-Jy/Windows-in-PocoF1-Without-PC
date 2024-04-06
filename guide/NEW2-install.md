<img align="right" src="beryllium.png" width="350" alt="Windows installation on beryllium">

# Windows installation guide for PocoF1

## Installing Windows

### Prerequisites
- [Windows on ARM esd](https://worproject.com/esd)

- [WinPE](https://drive.google.com/file/d/1ROmr2ki69QigIVFXJV5fRRSSd7K6h17D/view?usp=drivesdk)
  
- [Boot image](https://drive.google.com/drive/folders/1M64iZ3aeNiy0vvhW5refvDj0k0oXyAL1)

- [Drivers](https://drive.google.com/file/d/1YBK2fTmgmhzCaPg5luq-GJyGnM6i94Rf/view?usp=drivesdk)
  

### Checking Touchscreen panel type
- Install [Device Info HW apk](https://play.google.com/store/apps/details?id=ru.andr7e.deviceinfohw&pcampaignid=web_share)
- Go to **General** > **Touchscreen**.
- You should either see **NVT-ts** of **FTS-ts**
- Download all [boot image](https://drive.google.com/drive/folders/1M64iZ3aeNiy0vvhW5refvDj0k0oXyAL1) accordingly.

> You can check it through recovery terminal also 
```cmd
dmesg | grep dsi_display_bind
```
> This should output either `dsi_ebbg_fhd_ft8719_video_display` or `dsi_tianma_fhd_nt36672a_video_display`
>  
### Mount Windows and WinPE Partition on Android
> Make sure Windows and Winpe folder are already mounted using the magisk module on the previous page

#### Copy Installation File
- Download [windowsARM](https://worproject.com/esd), rename it to install.esd, and copy to Internal Storage > Windows
- Unzip [Driver.zip](https://drive.google.com/file/d/1YBK2fTmgmhzCaPg5luq-GJyGnM6i94Rf/view?usp=drivesdk) and copy to Internal Storage > Windows > Driver
- Unzip [WinPE.zip](https://drive.google.com/file/d/1lfRh5zd3pcaA7Z9WRsF5FM39NuIbZesS/view?usp=sharing) and copy all internal files/folder from it to Internal Storage -> Winpe
> [!Note]
> Be sure all copied file/folder is in the right place and name must be exectly as mentioned above. else installation will not start.
 
#### Backup important partitions
Reboot to Recovery and make a backup of boot, EFS, Modem and Persist.

### Running WinPe
- In your recovery, flash **PEboot image** to your boot partition, then reboot.
- Select  *UEFI OS* (it should be on #4* or *#3*) by pressing vol up and press power button to continue boot.

### Windows and Driver installation
> Once in Winpe, type ``` C:\install ``` on command prompt and press enter.
- It will take aprox 5 minutes and then automatically shutdown .

#### Boot into Windows
- Press Power + Vol Up to reboot to recovery
- Flash > **setup Windows image file** to the boot partition and reboot your device
- Windows will start booting .

### Setting up Windows
Your device will now set up Windows. This will take some time. It will eventually reboot, and after that the initial setup (oobe) should launch.

> [!Note]
> ◆ To skip the Microsoft Account login, use "g" for the email and password. Windows will then let you make a local account.
>
> ◆ If Sound and Rotation not working reboot to recovery and flash latest [UEFI](https://github.com/n00b69/woa-beryllium/releases/tag/UEFI) on boot partition and it will start working.

## [Last step: Setting up dualboot](/guide/dualboot.md)













