<img align="right" src="/beryllium.png" width="350" alt="Windows 11 running on beryllium">


# Running Windows on the Xiaomi Pocophone F1

## Partitioning your device

### Prerequisites
- A brain (most important of all)

- [Recovery]([Ofoxrecovery.zip](https://drive.google.com/file/d/1ZMjx6lC7uB1bTy6NXKjwKkLmKUEywKxu/view?usp=drive_link))

- [Resize.zip](Resize.zip)

- [Magisk](https://github.com/topjohnwu/Magisk/releases/download/v27.0/Magisk-v27.0.apk)

- [mountmodule](mountmodule.zip)

### Notes
> [!WARNING]  
> All your data will be erased! Back up now if needed.
> 
> Do not run the same command twice unless specified.
>  
> Do not run all commands at once, execute them in order!
>
> YOU CAN BREAK YOUR DEVICE WITH THE COMMANDS BELOW IF YOU DO THEM WRONG!!!
>
> DO NOT REBOOT YOUR PHONE! If you think you made a mistake, ask for help in the [Telegram chat](https://t.me/WinOnF1).


> [!IMPORTANT]
> This guide assumes you are rooted, if you aren't, please follow [this guide](root.md) first.
> Your existing recovery should work, if not,  use the provided recovery image in this guide. 

#### Flash recovery
> if your existing recovery not working ...
> Flash Ofoxrecovery.zip through your existing recovery or exterect recovery.img and flash it via fastboot command
```cmd
fastboot flash recovery path\to\twrp.img reboot recovery
```

#### Creat partitioning for Windows
> download resize.zip , reboot to recovery and flash it.
> Your Beryllium is ready for modify partitions
> NOW go to Main screen -> Advanced -> Terminal
> Type   modify   and wait till phone reboots to recovery 
```cmd
modify
```
> on recovery open terminal and type :
```cmd
chmod -x /cache/format
. /cache/format
```
> Reboot system and see if Android still works

#### Root android and flash magisk module
> If your androad is not rooted Download latest magisk and flash it.
> Now flash mountmodule.zip and flash it through magisk.
> Reboot and see two new folder "Windows" and "Winpe" appear in internal storage. 


## [Next step: Installing Windows](/guide/NEW2-install.md)























