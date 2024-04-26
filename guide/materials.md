<img align="right" src="beryllium.png" width="350" alt="Windows installation on beryllium">


# Windows installation guide for PocoF1

## Additional materials
> Below you will find a list of tweaks and materials for Windows on your ARM device

### List of supported apps/games
> This is by no means a comprehensive list, it simply lists apps/games that have been tested by the community
[The link can be found here](https://docs.google.com/spreadsheets/d/1XYuoySgYQE0HL573sA-0RGMX7I4lt5rWJuQ8Z8yRJNY/edit?usp=drivesdk)

> You can also find a list of dedicated ARM software at this [link](https://armrepo.ver.lt/)

### Hide E drive (modem partition)
> [!NOTE]
> This is recommended because this drive should not be modified, while some applications may try to write to it
> - Open a command prompt window and run ```diskpart```
> - Run ```list volume``` to see all available volumes
> - Select the disk that has letter E with ```select volume $```, replacing "$" with the volume number
> - Remove the letter with ```remove letter E```
> - Exit diskpart with ```exit```
#

### Install Microsoft Office / Microsoft 365
- Download this [ISO file](https://mega.nz/file/hjAiSL4T#G7kOKpsUFpyL2UW9RQmY2e96urcQW5xZKdc7ciaNOy8) to the tablet
- Right-click on the iso file and select Mount to open it in explorer
- Double-click on ```Office Tool Plus.exe``` to start the installation wizard
- In the window that appears, click `Yes`
- Wait for the installation to complete
#

### Activate Windows / Office
Follow the instructions by Massgravel [here](https://github.com/massgravel/Microsoft-Activation-Scripts)

#
### How to use the Flashlight
- Download [Flashlight.7z](https://github.com/erdilS/Port-Windows-11-Xiaomi-Pad-5/releases/download/1.0/flashlight_fix.7z) and unzip to any folder
> Run flashlight.exe to enable the flashlight, Press any key to disable it



















