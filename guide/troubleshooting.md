<img align="right" src="beryllium.png" width="350" alt="Windows installation on beryllium">


# Running Windows on the Xiaomi Pocophone F1

## Troubleshooting Issues
> Below you will find a list of common problems and their solutions
#
### Sound and Rotation not Working
> Reboot to recovery and flash latest [UEFI](https://github.com/n00b69/woa-beryllium/releases/tag/UEFI)
### Installation failed
Seems you have not followed proper instruction. 
Download installation file only from mentioned link and you Phone memory must have at least 6GB free space. 
#
### Touch does not work after sleep
> Reboot your device. This issue seems to not have a fix.
#
### Cannot write to Windows in Android
> This is caused by shutting down Windows instead of restarting it.
- To solve this, boot to Windows and then press "restart", then as the screen shuts off boot to TWRP and from there load up Android.
- Or, disable hibernation in Windows using [this](https://github.com/n00b69/woa-beryllium/releases/tag/1.0) script 
> Alternatively, if you have already set up the Switch to Android app, simply use this to switch to Android.
#
### USB does not work
Enable USB host mode using this guide :-.
> [!Warning]
> Disable USB host mode if you use a poweref USB hub, as this can irreversibly damage your device. If you don't use a powered USB hub, enable USB host mode or you will not be able to use any USB devices.

Run [USB Host Control](https://github.com/erdilS/Port-Windows-11-Xiaomi-Pad-5/releases/download/USBHost/USB.Host.Mode.Control.V4.0.vbs) to enable/disable USB host mode, confirm that you want to disable/enable USB host mode and then confirm the reboot
#
### 0xc000021a BSOD
This usually means that winlogon.exe has failed, and you may need to reinstall Windows.
#
### The computer restarted unexpectedly or encountered an unexpected error
If you stumble upon this error, you may need to reinstall Windows. Use the [Installation guide](Installation.md)
#
### BlueScreen with DRIVER PNP WATCHDOG error
(may be Bcz of touch panel detection issue)
- Restore android boot.img and reboot to android.
- Download [Device Info HW app](https://play.google.com/store/apps/details?id=ru.andr7e.deviceinfohw&pcampaignid=web_share), check your touch panel type.
- Download firstboot uefi img accordingly from this [link](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/tag/UEFI-Boot-Image)
- Reboot to recovery and Flash wininstaller zip
- Press volumes up button when rebooting to enter in recovery again
- Flash firstboot uefi img on boot partition
- Reboot to system and don't touch your phone till windows setup logo appeared
(Several restart is normal)
#
### INACCESSIBLE_BOOT_DEVICE BSOD
This Blue Screen of Death likely means some broken driver installation. To fix this, reinstall windows using the [Installation guide](Installation.md).
#
### Wifi and mobile data not working
Restart windows. if still not working, restore modem and persist from recovery.
#
