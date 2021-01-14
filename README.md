<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta http-equiv="X-UA-Compatible" content="ie=edge">
</head>

<body>

<div>

<h2>Nitro-5-an517-51-Hackintosh</h2>

</div>


<details>  
<summary><strong>Images</strong></summary>
<br>

<img width="70%" src="images/main1.png" alt="main">

<br>

<img width="70%" src="images/File1.png" alt="geekbench_score">

<br>


<img width="70%" src="images/File2.png" alt="Opencl_score">

<br>



</details>


<details>  
<summary><strong>What's working </strong></summary>
<br>
<table border="1px">

<tr>
<td>
<p> WiFi + Bluetooth + Airdrop + Universal Clipboard + Handoff + Continuity Camera + iPhone Cellular Calls (DW1820a) </p>
</td>

</tr>

<tr>
<td>
<p>Power Managment is very stable most of the time cpu Fan will not load but it depends on what you are doing </p>
</td>
</tr>

<tr>
<td>
<p>TouchPad + all gestures Finally after month of researching </p>
</td>
</tr>

<tr>
<td>
<p> Fully Functional QE/CI Enabled Graphics </p>
</td>
</tr>

<tr>
<td>
<p> intel bluetooth and WiFi on AX200 card </p>
</td>
</tr>

<tr>
<td>
<p> Display brightness with hot keys </p>
</td>
</tr>

<tr>
<td>
<p> FaceTime, Messages, etc... </p>
</td>
</tr>

<tr>
<td>
<p> iGPU with disabled dGPU </p>
</td>
</tr>

<tr>
<td>
<p>Audio & headphone jack </p>
</td>
</tr>

<tr>
<td>
<p>Battery Management  </p>
</td>
</tr>

<tr>
<td>
<p> All USB ports</p>
</td>
</tr>

<tr>
<td>
<p>WebCam  </p>
</td>
</tr>

<tr>
<td>
<p> Ethernet </p>
</td>
</tr>

<tr>
<td>
<p>Sidecar</p>
</td>
</tr>

<tr>
<td>
<p> <a style="text-decoration:none" href="https://dortania.github.io/OpenCore-Post-Install/universal/sleep.html">Sleep (Preparations section)</a></p>
</td>
</tr>

</table>
</details>

<details>

<summary><strong>Disabled Devices </strong></summary>
<br>

<p>GTX 1660Ti </p>


</details>

<details>

<summary><strong>Bios Settings </strong></summary>
<br>

<table border="1px">
<tr>
<td>
<p>Main → click on (calt+s) a new setting will appear to change SATA type to AHCI otherwise you will not be able to see you drive when installing hackintosh </p>
</td>
</tr>


<tr>
<td>
<p>Security → Set supervisor password (to disable secure boot)</p>
</td>
</tr>


<tr>
<td>
<p>Security → Password on boot → Disable</p>
</td>
</tr>


<tr>
<td>
<p>Boot → Secure Boot → Disable</p>
</td>
</tr>

</table>

</details>

<details>

<summary><strong>Not Working </strong></summary>
<br>



<p>HDMI (Nvidia Optimus is hardwire to HDMI)</p>



</details>

<details>
<summary><strong>Info</strong></summary>
<br>

<table border="1px">
<tr>
<td>
<p>When you switch SATA type to AHCI you might not be able to boot to windows again but do not worry here is a guide i found to switch without getting any issue <a href="https://support.thinkcritical.com/kb/articles/switch-windows-10-from-raid-ide-to-ahci">Here</a></p>
</td>
</tr>


<tr>
<td>
<p>You need to disable SystemProfilerMemoryFixup.kext if you wanna enter recovery mode or you will get kernel panic</p>
</td>
</tr>


<tr>
<td>
<p>To get right click to work go to touchpad settings in (Secondary click) choose (click in bottom right corner)</p>
</td>
</tr>


<tr>
<td>
<p>If apple Continuity did not worked try logout and login again on all your devices your hackintosh too</p>
</td>
</tr>

<tr>
<td>
<p>OpenCore Guide <a href="https://dortania.github.io/OpenCore-Install-Guide/">Here</a></p>
</td>
</tr>

</table>

</details>



<details>

<summary><strong>Updates</strong></summary>
<br>

<table border="1px"> 
   
<tr>
<td>
<p> UPDATES 14.06.2020-OpenCore <br><br> Add itlwmx.kext to get Intel-AX200 wifi to work but it's still in beta it will take time to improve (AX200 will work as Ethernet) read here for more info <a href="https://github.com/zxystd/itlwm">Here</a></p>
</td>
</tr>


<tr>
<td>
<p> UPDATES 09.06.2020-OpenCore <br><br> Bluetooth has been fixed you need to pin-masking <a href="https://osxlatitude.com/forums/topic/11540-dw1820a-the-general-troubleshooting-thread/?do=findComment&comment=91179">Here</a>  </p>
</td>
</tr>


<tr>
<td>
<p> UPDATES 26.05.2020-OpenCore <br><br> Add kext for intel Bluetooth for WiFi you can now search but still no internet so for now i will only add kext to get bluetooth to work intel-Bluetooth </p>
</td>
</tr>


<tr>
<td>
<p> UPDATES 23.05.2020-OpenCore <br><br> Remove igfxpavp=1 and igfxfw=2 boot arg to fix an issue where gpu usage will stay high after playing video on appstore  </p>
</td>
</tr>

<tr>
<td>
<p> UPDATES 20.05.2020-OpenCore <br><br> Fix USB Power Managment SSDT-USBX</p>
</td>
</tr>

<tr>
<td>
<p>UPDATES 18.05.2020-OpenCore <br><br> OC-DW1820a <br> Kexts</p>
</td>
</tr>

<tr>
<td>
<p> UPDATES 15.05.2020-OpenCore <br><br>  OpenCore 0.5.8 <br> Resources Folder <br> OC-Config.plist <br> Kexts </p>
</td>
</tr>

<tr>
<td>
<p> UPDATES 14.04.2020-OpenCore <br><br>Add SSDT-USBX.aml for USB-Power because after i tested usb-stick 3.1 gen i noticed it did not worked so now all port work normaly with super speed too <br> OC-Config.plist </p>
</td>
</tr>

<tr>
<td>
<p> UPDATES 12.04.2020-OpenCore <br><br> Fix an issue when usb is pluged-in the laptop will not sleep with SSDT-GPRW <br> Replace SSDT-NoHybGfx with SSDT-NDGP_OFF to make sleep faster <br> OC-Config.plist </p>
</td>
</tr>

<tr>
<td>
<p> UPDATES 11.04.2020-OpenCore <br><br> Replace DSDT with SSDT-BRKEY and SSDT-I2C-TPAD because placing DSDT will cause conflict with other patches <br>  Add NVMeFix.kext to get better power managment for NVMe <br> OC-Config.plist  </p>
</td>
</tr>

<tr>
<td>
<p> UPDATES 10.04.2020-OpenCore <br><br>Brightness with native hot keys <br> TouchPad has been fixed <br> OC-Config.plist <br> ACPI Patches </p>
</td>
</tr>

<tr>
<td>
<p> UPDATES 07.04.2020-OpenCore <br><br> better way to enable Apple ALC <br> CPUFriend-1.2.0-DevBuild <br>  WhateverGreen-1.3.8 <br> Resources Folder <br> VirtualSMC-1.1.2 <br> AppleALC-1.4.8 <br> OC-Config.plist <br> Lilu-1.4.3  </p>
</td>
</tr>


</table>

</details>


</body>

</html> 

