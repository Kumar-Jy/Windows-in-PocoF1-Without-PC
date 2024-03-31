<img align="right" src="https://github.com/n00b69/woaberyllium/blob/main/beryllium.png" width="350" alt="Windows 11 running on beryllium">


# Running Windows on the Xiaomi Pocophone F1

## Updating drivers

### Prerequisites

- [UEFI image](https://github.com/n00b69/woaberyllium/releases/tag/UEFI)
  
- [Drivers](https://github.com/n00b69/woaberyllium/releases/tag/Drivers)
    
- [Recovery](https://github.com/n00b69/woaberyllium/releases/download/Recoveries/twrp.img) (should already be installed)

#### Boot to recovery
> If Xiaomi has replaced your recovery back to stock, flash it again in fastboot with:
```cmd
fastboot flash recovery path\to\twrp.img reboot recovery
```

#### update Driver
> Reboot to recovery flash PEboot.img according to your touch panel
> Boot to WinPE open Dism++ Select all Driver and Delete
> Now install New Driver
> type ```cmd shutdown -s -t -0 ``` on command windows 


##### Boot back into Windows
> Reboot your device to recovery. reflash uefi-beryllium-....img on boot partition this boots you to windows.


## Finished!



















