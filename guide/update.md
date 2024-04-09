<img align="right" src="https://github.com/n00b69/woaberyllium/blob/main/beryllium.png" width="350" alt="Windows 11 running on beryllium">

# Running Windows on the Xiaomi Pocophone F1

## Updating drivers

### Prerequisites
- [PEinstallar](https://g)
  
- [Drivers](https://github.com/n00b69/woaberyllium/releases/tag/Drivers)
    
- [Recovery](https://r) (should already be installed)

#### Note
> If your existing recovery is not working, flash orangefox recovery.

#### Updating drivers
- Download Driver.zip and extract Driver folder in C: Drive
- Reboot to recovery and Flash **PEinstallar** . Reboot to UEFI and select PEboot option to boot into WinPE
- Dism++ will automatically start in WinPE , Mount Windows Drive - Open Season - select **All Drivers**, and **Delete**
- Now click on 'add Driver' and select Driver folder , after installation finished type ```shutdown -s -t -0 ``` on CMD terminal, your phone will shutdown
- Reboot back into Windows and enjoy.

## Finished!































