<img align="right" src="beryllium.png" width="350" alt="Windows installation on beryllium">

# Windows installation guide for PocoF1

## Partitioning your device

### Prerequisites
- A brain (most important of all)

- [OfoxRecovery](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/download/Moded-Ofox-Recovery/Ofox-beryllium-pe.img)


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



### Flash recovery
- Flash [Ofox-beryllium-pe.img](https://github.com/Kumar-Jy/Windows-in-PocoF1-Without-PC/releases/download/Moded-Ofox-Recovery/Ofox-beryllium-pe.img) either through your existing recovery or through fastboot.


### Create partitions for Windows
- Open terminal in ofox recovery and type `partition $`
- Replace $ with the size of storage in GB you want for Windows (do not add GB at the end, just the number)
- If it asks you to run it once again, do so
- Reboot to check if Android still works.
- If it doesn't boot, format userdata and Reboot


## [Next step: Installing Windows](/guide/NEW2-install.md)




































