## Lab Profile Manifest

### Virtual Machines

#### WS2022 BASE

>[+] VM Configuration
>
| Item | Detail | | Item | Detail |
|:---------|:---------| |:---------|:---------|
| User |+++@lab.VirtualMachine(WS2022).Username+++| | IP Address   | **DHCP**   |
| Password |+++@lab.VirtualMachine(WS2022).Password+++| | CPU(s) | **6** |
| Name   | **WS2022 Base** | | RAM | **4.5 GB** |
| Platform | **ESX** | | HD 1 | **100 GB** |
| OS | **Windows** | | NIC(s) | **1** |

>[+]  VM Optimizations
 - Skillable Integration\VMware tools 12.3 installed.
 - Change Computer name.
 - Module Update PS Help (Get-Help Update).
 - Disable IE Security for Admins and Users.
 - Install Edge Chromium.
 - Install All Current Windows Updates. 
 - Installed BGinfo and configured a watermark.
 - Disable Lock screen.
 - Disable Windows Updates.
 - Clear all event logs on local machine.
 - Set passwords not to expire.
 - Set admin password not to expire.
 - Disable requirement for **CTRL + ALT + DEL** to sign in.
 - Disable and refuse Domain Password change prompts. 
 - Clear PowerShell History.
 - Clear Run History.
 - Disable Network Notifications.
 - Clear out Network Profiles.
 - Set Network to Private.
 - Enable Remote Desktop Access.
 - Optimize Visual performance for user.
 - Remove recent Programs.
 - Create firewall settings for 192.168.10.0/24 network (outbound, inbound).
 - Ensure appropriate power settings (Highest avail Performance, Disable monitor timeout).
 - Optimize Edge (Policies).
 - Configure Edge settings.
 - System tray clean up (Open the new Windows 'Settings' app and search for "Turn System Icons on or off"). Only leave Network and Clock.
 - Disable Automatic Windows Updates via GPEDiT.
    - Navigated to **Computer Configuration >  Administrative Templates > Windows Components > Windows update**.  
    - **Adjusted the following**: 
    - Configure Automatic Updates : **Disabled**. 
    - Allow Automatic Updates immediate Installation : **Disabled**. 
    - Do not adjust default option to 'Install Updates and Shut Down' in Shut Down Windows dialog box : **Enabled**.  
    - No auto-restart with logged on users for scheduled automatic updates installations : **Enabled**.  
  - Navigated to **Computer Configuration > Administrative Templates > Windows Components > Store**.  
    - **Adjusted the following**:
    - Turn off Automatic Download and Install of updates : **Enabled**.  
    - Turn off Automatic Download of updates on Win machines : **Enabled**.  
 -  Hide Recently added apps in Start Menu.
   - **Settings > Personalization > Start >** Show Recently Added apps toggle **OFF**.
   - **GPEDIT > Computer Configuration > Administrative Templates > Start Menu and Taskbar >** Remove "Recently Added" list from start menu **ENABLED**. 
 -  Turn Notifications off (System Settings).
 -  System Performance Settings, Highest Performance available (Best Performance, Ultimate Performance, Check Smooth Edges Screen Fonts) .
 -  Power Display Settings to Never Shut Off. 
 -  Clear Windows Updates Cache. 
 -  Empty the Recycle Bin. 
 -  Power & Sleep > Screen turn off **Never**.
 -  Resize VM (Display settings-change to 1024 x 768).

>[+] VM Software
>
|Product|Version|Vendor|
|:--|:--|:--|
|Microsoft Edge|                                                     **125.0.2535.51**|  Microsoft Corporation| 
|Microsoft Edge Update|                                              **1.3.187.37**|     Microsoft Corporation|                           
|Microsoft Visual C++ 2022 X86 Minimum Runtime - 14.38.33135|        **14.38.33135**|    Microsoft Corporation|     
|Microsoft Visual C++ 2015-2022 Redistributable (x86) - 14.38.33135| **14.38.33135.0**|  Microsoft Corporation|     
|Microsoft Visual C++ 2022 X86 Additional Runtime - 14.38.33135|     **14.38.33135**|    Microsoft Corporation|     
|Microsoft Visual C++ 2015-2022 Redistributable (x64) - 14.38.33135| **14.38.33135.0**|  Microsoft Corporation| 

### Networks

#### WebNAT

>[+] Network Configuration
>
|Item|Detail|
|:----|:----|
|Type|**Web Access (NAT)**|
|Gateway|**192.168.100.1**|
|Subnet Mask|**255.255.255.0**|
|DHCP Enabled|**192.168.100.100** to **192.168.100.200**|

### Cloud
There are no Cloud settings in this lab profile.

### Life Cycle
There are no Life Cycle settings in this lab profile.