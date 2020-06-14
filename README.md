## Nitro-5-an517-51-Hackintosh

![](/images/main1.png)
![](/images/11.png)
![](/images/File1.png)
![](/images/File2.png)
![](/images/12.png)
# Files are always updated

Supports MacOS 10.15.x, **tested only on catalina but it should work on (10.14.x and 10.13.x)**

##### What's Working...
* intel bluetooth and WiFi on AX200 card (you will need to change add your ssid and password manually open the kext and find info.plist in WiFiConfig section)
* Sleep (https://dortania.github.io/oc-laptop-guide/battery-power-management/correcting-sleep-problems.html) (Disabling Hibernation)
* WiFi + Bluetooth + Airdrop + Universal Clipboard + Handoff + Continuity Camera + iPhone Cellular Calls (DW1820a)
* Power Managment is very stable most of the time cpu Fan will not load but it depends on what you are doing
* TouchPad + all gestures Finally after month of researching
* Fully Functional QE/CI Enabled Graphics
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
* intel Bluetooth
* GTX 1660Ti
##### BIOS Settings

* Security → Set supervisor password (to disable secure boot)
* Security → Password on boot → Disable
* Boot → Secure Boot → Disable
* Main → click on (calt+s) a new setting will appear to change SATA type to AHCI otherwise you will not be able to see you drive when installing  hackintosh
 # WIP
 ####  Bios Unlock to unlock CFG and have full control over your laptop (done without programmer)
 
 https://github.com/SaeedHaidar/Acer-Nitro-5-AN517-51-Bios-Unlocking
 
 https://www.amazon.de/-/en/KeeYees-SOIC8-EEPROM-CH341A-Programmer/dp/B07SNTL5V6/ref=sr_1_2?dchild=1&keywords=ch341a&qid=1587467368&sr=8-2
# Working but still in beta
#### Intel-AX200 wifi
![](/images/15.png)
# Not Working
####  HDMI (Nvidia Optimus is hardwire to HDMI)
# Important info 
#### When you switch SATA type to AHCI you might not be able to boot to windows again but do not worry here is a guide i found to switch without getting any issue https://support.thinkcritical.com/kb/articles/switch-windows-10-from-raid-ide-to-ahci
#### If apple Continuity did not worked try logout and login again on all your devices your hackintosh too 
#### OpenCore Guide https://dortania.github.io/oc-laptop-guide/
#### To get right click to work go to touchpad settings in (Secondary click) choose (click in bottom right corner)

## Do not forget to generate new Smbios with clover configurator and for OC use GenSMBIOS (MacBook pro 16,1)
## &#x1F34F;   UPDATES 14.06.2020-OpenCore
* Add itlwmx.kext to get Intel-AX200 wifi to work but it's still in beta it will take time to improve (AX200 will work as Ethernet) read here for more info https://github.com/zxystd/itlwm
## &#x1F34F;   UPDATES 09.06.2020-OpenCore
* Bluetooth has been fixed you need to pin-masking https://osxlatitude.com/forums/topic/11540-dw1820a-the-general-troubleshooting-thread/?do=findComment&comment=91179
and do not forget to add the kexts too 
## &#x1F34F;   UPDATES 26.05.2020-OpenCore
* Add kext for intel Bluetooth for WiFi you can now search but still no internet so for now i will only add kext to get  bluetooth to work intel-Bluetooth
## &#x1F34F;   UPDATES 23.05.2020-OpenCore
* Remove igfxpavp=1 and igfxfw=2 boot arg to fix an issue where gpu usage will stay high after playing video on appstore 
## &#x1F34F;   UPDATES 20.05.2020-OpenCore
* Fix USB Power Managment SSDT-USBX
## &#x1F34F;   UPDATES 18.05.2020-OpenCore
* OC-DW1820a 
* Kexts

## &#x1F34F;   UPDATES 15.05.2020-OpenCore
* OpenCore 0.5.8
* Resources Folder 
* OC-Config.plist
* Kexts
## &#x1F34F;   UPDATES 14.04.2020-OpenCore
* Add SSDT-USBX.aml for USB-Power because after i tested usb-stick 3.1 gen i noticed it did not worked so now all port work   normaly with super speed too 
* OC-Config.plist
## &#x1F34F;   UPDATES 12.04.2020-OpenCore
* Fix an issue when usb is pluged-in the laptop will not sleep with SSDT-GPRW 
* Replace SSDT-NoHybGfx with SSDT-NDGP_OFF to make sleep faster 
* OC-Config.plist

## &#x1F34F;   UPDATES 11.04.2020-OpenCore
* Replace DSDT with SSDT-BRKEY and SSDT-I2C-TPAD because placing DSDT will cause conflict with other patches
* Add NVMeFix.kext to get better power managment for NVMe
* OC-Config.plist

## &#x1F34F;   UPDATES 10.04.2020-OpenCore
* Brightness with native hot keys
* TouchPad has been fixed 
* OC-Config.plist
* ACPI Patches

## &#x1F34F;   UPDATES 07.04.2020-OpenCore
* better way to enable Apple ALC
* CPUFriend-1.2.0-DevBuild
* WhateverGreen-1.3.8
* Resources Folder
* VirtualSMC-1.1.2
* AppleALC-1.4.8
* OC-Config.plist
* Lilu-1.4.3


## &#x1F34F;   UPDATES 05.04.2020
* Add SystemProfilerMemoryFixup.kext to show memory section in about this Mac
* Add Theme to OpenCore Bootloader
* OC-Config.plist
* OpenCore 0.5.7
* Clover 5108
* Some missing parts :
* SSDT-DMAC
* SSDT-SBUS
* SSDT-XSPI
* SSDT-MCHC
* SSDT-PMC
* SSDT-MEM2
* SSDT-PPMC
* SSDT-SBUS-MCHC
* SSDT-HPET.aml

## Bios Version 
1.28 https://www.acer.com/ac/en/US/content/support-product/7966?b=1



