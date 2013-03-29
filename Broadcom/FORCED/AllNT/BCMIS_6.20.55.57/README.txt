To install the bcmis driver (without going through the wl driver install),
copy the driver and the INF file to a directory on the target machine: 

(Note: The same bcmis driver can install on Vista/Win7)

Installation:
- Uninstall current driver if it installed(see 'Uninstallation' section below).
- Double-click the 'Network and Sharing Center' in Control Panel.
- For Vista, click the 'Manage network connections'.
  For Win7, click the 'Change adapter settings'.
- Find 'Broadcom Virtual Wireless Adapter' and right-click on the device icon.
- Select 'Properties'.
- Click 'Install'.
- Select 'Service' and click 'Add'
- Click 'Have Disk'.
- Click 'Browse' and navigate to the location where driver was saved. 
- Highlight the inf file and click 'Open' and then click 'OK'
- Click on the desired entry, and then click 'OK'. 

3G network configuration:
- If using VZAccess Manager for Verizon 3G broadband network, make sure NDIS mode is used:
  - Select 'Option' from VZAccess Manager menu.
  - Select 'Preferences'.
  - Under 'WWAN connection type:', select 'NDIS Mode - xxx'.

Uninstallation:
- Double-click the 'Network and Sharing Center' in Control Panel.
- For Vista, click the 'Manage network connections'.
  For Win7, click the 'Change adapter settings'.
- Find 'Broadcom Virtual Wireless Adapter' and right-click on the device icon.
- Select 'Properties'.
- Highlight 'Broadcom NAT LW Filter Driver' and click 'Uninstall'.
