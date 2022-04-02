# :fire: VMR-MDK-K2-2017R-012x4
VMR-MDK is a script for cracking wps wireless networks

**Mainly used for WPS locked routers**

`Read the "Help Files VMR-MDK-K2-2017R-012x4.txt" file to get a brief on the script what it does and how it works.`

`Read the "configfiledetailed" file to learn more about the config and tweaking the way the script works.`

# INSTALLATION
Open your terminal and run this command

:point_right: `git clone https://github.com/Transmetal/VMR-MDK-K2-2017R-012x4`     

Enter the directory
	
:point_right: `cd VMR-MDK-K2-2017R-012x4`
	
Set your permissions

:point_right: `chmod +x VMR-MDK-K2-2017R-012x4.sh`  [Enter]
	
create the three varmac folders in root [VARMAC_CONFIG, VARMAC_LOGS, VARMAC_WASH]
	
:point_right: `mkdir VARMAC_CONFIG /root/`
:point_right: `mkdir VARMAC_LOGS /root/`
:point_right: `mkdir VARMAC_WASH /root/`

:exclamation: WARNING Before running manually remove any wifi virtual monitor ie wlan0mon0 etc made by the newer airmon-ng

Run by the script 
	
:point_right: `./VMR-MDK-K2-2017R-012x4.sh`  [Enter]

[optional steps]
	
Or place in the user/sbin folder, if you want to be able to call it from anywhere

`chmod +x /user/bin/VMR-MDK-K2-2017R-012x4.sh`  [Enter]

`VMR-MDK-K2-2017R-012x4.sh`   [Enter]

     	

## :rocket: Extra Modifications
I have added a diagnostics tool to it to check if your wireless card is injectable and some extras, all you need to do is, cd into the scripts directory and run it

:point_right: `cd scripts`   <= [enter the scripts dir]

:point_right: `./diagnostics.sh wlan0`    <= [run the diagnostics script]

where wlan0 is whatever your wireless interface is called, you can check this by running

:point_right: `airmon-ng`     <= [shows you your wireless interface, if any]
