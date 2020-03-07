## Nitro-5-an517-51-Hackintosh

Supports MacOS 10.15.x, **tested only on catalina but it should work on (10.14.x and 10.13.x)**

##### What's Working...
* Power Managment is very stable most of the time cpu Fan will not load but it depends on what you are doing
* Display brightness with hot keys (Fn+(F11,F12))
* Fully Functional QE/CI Enabled Graphics
* FaceTime, Messages, etc...
* iGPU with disabled dGPU
* Audio & headphone jack
* Battery Management
* Ethernet
* WebCam

##### BIOS Settings

* Security → Set supervisor password (to disable secure boot)
* Security → Password on boot → Disable
* Boot → Secure Boot → Disable
* Main → press (calt+s) a new setting will appear to change SATA type to AHCI otherwise you will not be able to see you drive when installing  hackintosh
 
# WIP

#### USBmap
#### touchpad
#### Sleep
#### OpenCore Bootloader

## Do not forget to generate new serial number and uuid with clover configurator
# Important info 
#### when you switch SATA type to AHCI you might not be able to boot to windows again but do not worry here is a guide i found https://support.thinkcritical.com/kb/articles/switch-windows-10-from-raid-ide-to-ahci
