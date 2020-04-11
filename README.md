## Nitro-5-an517-51-Hackintosh

![](/images/main1.png)
![](/images/File1.png)
![](/images/File2.png)
# Files are always updated

Supports MacOS 10.15.x, **tested only on catalina but it should work on (10.14.x and 10.13.x)**

##### What's Working...
* Sleep (https://fewtarius.gitbook.io/laptopguide/battery-power-management/correcting-sleep-problems) (Disabling Hibernation)
* Power Managment is very stable most of the time cpu Fan will not load but it depends on what you are doing
* Fully Functional QE/CI Enabled Graphics
* TouchPad Finally after month of trying
* Display brightness with hot keys
* FaceTime, Messages, etc...
* iGPU with disabled dGPU
* Audio & headphone jack
* Battery Management
* All USB ports
* WebCam
* Ethernet
* Sidecar


##### Disabled Devices
* Bluetooth
* GTX 1660Ti
##### BIOS Settings

* Security → Set supervisor password (to disable secure boot)
* Security → Password on boot → Disable
* Boot → Secure Boot → Disable
* Main → click on (calt+s) a new setting will appear to change SATA type to AHCI otherwise you will not be able to see you drive when installing  hackintosh
 # WIP
 ####  Bios Unlock to unlock CFG 
 #### Wifi card replacment 
 
# Not Working
####  intel WiFi/Bluetooth not supported
# Important info 
#### when you switch SATA type to AHCI you might not be able to boot to windows again but do not worry here is a guide i found to switch without getting any issue https://support.thinkcritical.com/kb/articles/switch-windows-10-from-raid-ide-to-ahci
#### OpenCore Guide https://1revenger1.gitbook.io/laptop-guide/
#### Clover Guide https://fewtarius.gitbook.io/laptopguide/

## Do not forget to generate new Smbios with clover configurator and for OC use GenSMBIOS (MacBook pro 16,1)
## &#x1F34F;  UPDATES 10.04.2020-OpenCore
* Brightness with native hot keys
* TouchPad has been fixed 
* OC-Config.plist
* ACPI Patches

## &#x1F34F;  UPDATES 07.04.2020-OpenCore
* better way to enable Apple ALC
* CPUFriend-1.2.0-DevBuild
* WhateverGreen-1.3.8
* Resources Folder
* VirtualSMC-1.1.2
* AppleALC-1.4.8
* OC-Config.plist
* Lilu-1.4.3


## &#x1F34F;  UPDATES 05.04.2020
* Add SystemProfilerMemoryFixup.kext to show memory section in about this Mac
* Add Theme to OpenCore Bootloader
* OC-Config.plist
* OpenCore 0.5.7
* Clover 5108
* New Adds to get better Performance :
* SSDT-DMAC
* SSDT-SBUS
* SSDT-XSPI
* SSDT-MCHC
* SSDT-PMC
* SSDT-MEM2
* SSDT-PPMC
* SSDT-SBUS-MCHC
* SSDT-HPET.aml
* SSDT-EC-USBX.aml

## Bios Version 
1.28 https://www.acer.com/ac/en/US/content/support-product/7966?b=1



