# Troodon-V2 Mini Updated Config

This set of config files assumes that the firmware has been updated to at least 3.4.5.

**WARNING** When using this config, please delete the 2 G31 lines out of your config-override.g and reboot. Then recalibrate your AutoZ and Toolhead Probes

# Changelog

# Version 1
Forked from [TeamGloomy/Troodon-V2](https://github.com/TeamGloomy/Troodon-V2)

# Initial Upgrade Instructions

Upload the latest stable version of reprapfirmware from [here](https://github.com/gloomyandy/RepRapFirmware/releases/latest/) selecting the asset with firmware-stm32f4-wifi in the name.  
Click on the System tab and then the Upload System Files button.  
![Show Settings](./Images/upload.png)  
Find the firmware file you downloaded, select it and then click open.  
When asked, apply the update.  
Upload the latest stable version of DuetWebControl from [here](https://github.com/Duet3D/DuetWebControl/releases/latest/) selecting the asset called DuetWebControl-SD.zip. Make sure that the version number is the same as the firmware file you downloaded above. If it isn't, click on releases and find the correct version.
![Show Settings](./Images/releases.png) 
Like above, click on the System tab and then the Upload System Files button, find the DuetWebControl-SD.zip file and click open. DWC (DuetWebControl) will automatically unzip the files and refresh the page when complete.  
Download the config zip file from [here](https://github.com/TeamGloomy/Troodon-V2/releases/latest/).  
Like above, click on the System tab and then the Upload System Files button, find the downloaded config zip file and click open. DWC (DuetWebControl) will automatically unzip the files. When asked, restart the machine.  
Delete the G31 lines out of config-override.g and rerun the probe and autoz offset macros.    

# Updating an already converted machine

Either upload the latest release zip file (be aware that this will overwrite any of the files included in the base config) or manually make the adjustments as detailed in each commit.
