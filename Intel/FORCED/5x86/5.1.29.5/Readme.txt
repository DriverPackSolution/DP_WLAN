***************
* Windows XP:
***************

1. If the drivers aren’t signed by WHQL:
	a. Install the MS Test certificate.
	b. Reboot the machine.

2. Put all the drivers' files into a local directory (for example: "C:\WiMAX_Drivers").

3. Open the RegEdit tool and add the directory path into the following registry key:

	Key:                 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion
	Name:                DevicePath
	Type:                REG_EXPAND_SZ
	Value:               String represents the folders' name separated by semi-colon (;).

4. Reboot the machine (or rescan for new devices).

5. All the drivers should be installed now.

 
**************************
* Windows Vista/Windows 7:
**************************

1. If the drivers aren’t signed by WHQL:
	a. Install the MS Test certificate.
	b. Enter into test mode, by running the command: "bcdedit /set testsigning on".
	c. Reboot the machine.
	
2. Remove any WiMAX devices from the Device Manager, even from the unknown devices section.

3. Put all the drivers' files into a local directory (for example: "C:\WiMAX_Drivers").

4. Run the command: "PnpUtil.exe -a {DriversDir}\*.INF", where {DriversDir} is the path where you put the drivers. (in our example: PnpUtil.exe -a C:\WiMAX_Drivers\*.INF)

5. Reboot the machine (or rescan for new devices).

6. All the drivers should be installed now.

