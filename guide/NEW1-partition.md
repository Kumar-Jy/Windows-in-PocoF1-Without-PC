<img align="right" src="beryllium.png" width="350" alt="Windows installation on beryllium">

# Windows installation guide for PocoF1

## Partitioning your device

### Prerequisites
- A brain (most important of all)

- [OfoxRecovery](https://drive.google.com/file/d/1ZMjx6lC7uB1bTy6NXKjwKkLmKUEywKxu/view?usp=sharing)

- [ModifyPartition.zip](https://drive.google.com/file/d/1aLex1_xi4AXwg5zc533fxTwTyU5zRZgl/view?usp=sharing)

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

### Flash recovery
> If your existing recovery does not work

- Flash [Ofoxrecovery.zip](https://drive.google.com/file/d/1ZMjx6lC7uB1bTy6NXKjwKkLmKUEywKxu/view?usp=sharing) through your existing recovery

#### Create partitions for Windows
- Download [ModifyPartition.zip](https://drive.google.com/file/d/1aLex1_xi4AXwg5zc533fxTwTyU5zRZgl/view?usp=sharing) , reboot to recovery and flash it.
- Open terminal Type `modify` and wait until the phone reboot and back to recovery 
- Open Terminal again and run
```cmd
chmod -x /cache/format
. /cache/format
```
- Reboot your system and see if Android still works

### Root android and flash magisk module
> If your Android is not rooted, use the [root guide](root.md) first.

- Flash [mountmodule.zip](mountmodule.zip) in Magisk.
- Reboot and you will find two folders "Windows" and "Winpe" in internal storage. 

## [Next step: Installing Windows](/guide/NEW2-install.md)




































