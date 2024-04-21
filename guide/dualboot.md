<img align="right" src="beryllium.png" width="350" alt="Windows installation on beryllium">

# Windows installation guide for PocoF1

## Dualboot guide

### Prerequisites
- [UEFI image](https://github.com/n00b69/woaberyllium/releases/tag/UEFI)

- [WOA Helper app](https://github.com/n00b69/woaberyllium/releases/download/Dualboot/woahelper.apk)

- [Switch To Android package](https://github.com/n00b69/woaberyllium/releases/download/Dualboot/beryllium-sta.zip)


## Dualboot guide
This guide assumes you are rooted, if you aren't, please follow [this guide](root.md) first.

### Setup - Windows
- Navigate to C:\sta and create a shortcut of `sta.exe` to your desktop.

#### Booting to Android
  - Run the new shortcut on your desktop (you can also pin it to your start menu / taskbar for ease of access)
  > [!Note]
> ◆ if it prompt vcruntime140.dll error install [Microsoft Visual C++](https://aka.ms/vs/17/release/vc_redist.arm64.exe).
> 
> ◆if the above step failed, press restart in Windows, then as it is restarting boot back to recovery to flash your Android boot.img located in your internal storage /backup folder, and try again.


### Setup - Android
- Reboot to recovery, restore boot.img from 'sdcard/backup' folder, and reboot to system. 
- Download and install the [WOA Helper app](https://github.com/n00b69/woaberyllium/releases/download/Dualboot/woahelper.apk), then open it and grant it root access.
- Download the [UEFI](https://github.com/n00b69/woaberyllium/releases/tag/UEFI) image for your panel and place it inside the folder named `UEFI` in your internal storage.
- Press the `Mount Windows` button to mount Windows to your internal storage at `/sdcard/Windows`

#### Booting to Windows
  - Press `Quickboot to Windows` inside the app, or use the newly created toggle in your quick settings panel
  
## Finished!




















