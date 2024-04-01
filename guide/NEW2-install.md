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

### Checking Touchscreen panel type
- Install [Device Info HW app](https://play.google.com/store/apps/details?id=ru.andr7e.deviceinfohw&pcampaignid=web_share)
- Go to **General** > **Touchscreen**.
- You should either see **NVT-ts** of **FTS-ts**

> You can also check it through recovery terminal also 
```cmd
adb shell dmesg | grep dsi_display_bind
```
> This should output either `dsi_ebbg_fhd_ft8719_video_display` or `dsi_tianma_fhd_nt36672a_video_display`
>
> Download all boot image file accordingly.
  
### Mount Windows and WinPE Partition on Android
> Make sure Windows and WinPE are already mounted using the module on the previous page

#### Copy Installation File
- Download [windowsARM](https://worproject.com/esd), rename it to install.esd, and copy it to Internal Storage > Windows
- Unzip [Driver.zip](https://drive.google.com/file/d/1YBK2fTmgmhzCaPg5luq-GJyGnM6i94Rf/view?usp=drivesdk) and copy it to Internal Storage > Winpe
- Unzip [WinPE.zip](https://drive.google.com/file/d/1lfRh5zd3pcaA7Z9WRsF5FM39NuIbZesS/view?usp=sharing) and copy all files to Internal Storage -> Winpe
 
#### Backup important partitions
Reboot to Recovery and make a backup of boot, EFS, Modem and Persist.

### Running WinPe
- In your recovery, flash **bootPE....img** to your boot partition (from the Downloads folder), then reboot your device
- Select  *UEFI OS on #4*  by pressing vol up and press power button to continue boot.

### Windows installation
> Once in Winpe, connect a Keyboard/Mouse - Open Dism++ (from C Drive - other - dism++(Arm64))
- Open File > Apply image
- Enter the path of the **install.esd** file or you can Browse and select D Drive
```cmd
D:\
```
- Change Target Image as per your requirment.
- Enter the installation drive Path or you can Browse and select D Drive
```cmd
D:\install.esd
```
- Check Add Boot and click OK, then wait for Windows to install


### Driver installation
- Click on open Session > Drivers > Add
- Select the driver folder ( from C Drive)
- Wait for it to finish, then close Dism++
- Open C Drive > other > right click on miscfix.bat and run as administrator, let it complete.
- After it automatically shuts down, your installation is complete

#### Boot into Windows
- Press Power + Vol Up to reboot to recovery
- Flash > **setup....img** to the boot partition and reboot your device

### Setting up Windows
Your device will now set up Windows. This will take some time. It will eventually reboot, and after that the initial setup (oobe) should launch.

> [!Note]
> To skip the Microsoft Account login, use "g" for the email and password. Windows will then let you make a local account

## [Last step: Setting up dualboot](/guide/dualboot.md)





















