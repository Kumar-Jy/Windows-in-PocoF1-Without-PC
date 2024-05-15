<img align="right" src="beryllium.png" width="350" alt="Windows installation on beryllium">

# Windows installation guide for PocoF1

## Installing Windows
:no_entry_sign: Don't try if you have not followed this [partition](NEW1-partition.md) guide
- it assumes `esp on 21`, `win on 23` and `pe on 24`
- if you have same partition table you can do this.
- your phone must be decrypted.

### Prerequisites
- [Windows ESD Image](http://dl.delivery.mp.microsoft.com/filestreamingservice/files/48c0db41-e529-47bb-8049-b8d2f2708271/22631.2861.231204-0538.23H2_NI_RELEASE_SVC_REFRESH_CLIENTCONSUMER_RET_A64FRE_en-us.esd)
- [WinInstaller](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/Win-Installar)

    

### Checking Touchscreen panel type
- On your android install [Device Info HW apk](https://play.google.com/store/apps/details?id=ru.andr7e.deviceinfohw&pcampaignid=web_share) , open app and go to **General** > **Touchscreen**.
- You should either see **NVT-ts** of **FTS-ts**
- Download [WinInstaller.zip](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/Win-Installar) accordingly.
- Download [Windows ESD image](http://dl.delivery.mp.microsoft.com/filestreamingservice/files/48c0db41-e529-47bb-8049-b8d2f2708271/22631.2861.231204-0538.23H2_NI_RELEASE_SVC_REFRESH_CLIENTCONSUMER_RET_A64FRE_en-us.esd) it should be in `Download` folder of your phone memory.

### Windows Installation
- Reboot to recovery and flash Wininstaller zip and wait till process complete.
- This will take some time. It will eventually reboot, and after that the initial setup (oobe) should launch.


> [!Note]
> ◆ To skip the Microsoft Account login, use "g" for the email and password. Windows will then let you make a local account.
>
> ◆ If Sound and Rotation not working reboot to recovery and flash latest [UEFI](https://github.com/n00b69/woa-beryllium/releases/tag/UEFI) and it will start working.

## [Last step: Setting up dualboot](/guide/dualboot.md)













