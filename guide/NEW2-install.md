<img align="right" src="beryllium.png" width="350" alt="Windows installation on beryllium">

# Windows installation guide for PocoF1

## Installing Windows
:no_entry_sign: Don't try if you have not followed this [partition](NEW1-partition.md) guide
- it assumes `esp on 21`, `pe on 22` and `win on 24` 

### Prerequisites
- [Windows on ARM esd](https://worproject.com/esd) `(Select - Version: 11 Build: 22631.2861 Architecture: ARM64 Edition: CLIENT Language: select your language)`

- [WinInstallar](https://drive.google.com/drive/folders/1RP-AsQ4MkVYeHJFr3HqAPn3rP7rY12-V?usp=drive_link)
    

### Checking Touchscreen panel type
- Install [Device Info HW apk](https://play.google.com/store/apps/details?id=ru.andr7e.deviceinfohw&pcampaignid=web_share)
- Go to **General** > **Touchscreen**.
- You should either see **NVT-ts** of **FTS-ts**
- Download [Wininstallar.zip](https://drive.google.com/drive/folders/1RP-AsQ4MkVYeHJFr3HqAPn3rP7rY12-V?usp=drive_link) accordingly.
- Download [Windows ESD image](https://worproject.com/esd) it should be in `Download` folder of your phone 

### Setup Installation Process
- Boot to recovery open terminal and type
```cmd
chmod +x /cache/format
. /cache/format
```
- Now flash Wininstallar zip file and wait till process complete (have patent it will take somtime)
- Reboot your phone and let it continue boot.
- Windows installation process will start automaticly and then phone automaticly restart to setup windows.

### Setting up Windows
Your device will now set up Windows. This will take some time. It will eventually reboot, and after that the initial setup (oobe) should launch.

> [!Note]
> ◆ To skip the Microsoft Account login, use "g" for the email and password. Windows will then let you make a local account.
>
> ◆ If Sound and Rotation not working reboot to recovery and flash latest [UEFI](https://github.com/n00b69/woa-beryllium/releases/tag/UEFI) and it will start working.

## [Last step: Setting up dualboot](/guide/dualboot.md)













