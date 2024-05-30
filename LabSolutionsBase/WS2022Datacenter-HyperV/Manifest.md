===

# Lab Profile Manifest{labprofilemanifest}
The virtual machines and profile attributes within this foundational environment are delineated as follows: virtual machine configurations, network parameters, and any pertinent cloud-specific settings or lifecycle actions relevant to this context.

## Virtual Machines
- **WS2022 BASE**

>[+] VM Configuration
>
| Item | Detail |
|:---------|:---------|
| User | +++@lab.VirtualMachine(WS2022 Datacenter).Username+++ |
| Password | +++@lab.VirtualMachine(WS2022 Datacenter).Password+++ |
| Name   | **WS2022 Base** |
| Platform | **Hyper-V** |
| OS | **Windows** |
| IP Address   | **DHCP**   |
| CPU(s) | +++4+++ |
| RAM | +++4.5+++ GB |
| HD 1 | +++100+++ GB |
| NIC(s) | +++1+++ |

>[+]  VM Optimizations
>
> - Skillable Integration\VMware tools 12.3 installed.
>
> - Change Computer name. 
>
> - Module Update PS Help (Get-Help Update).
>
> - Disable IE Security for Admins and Users.
>
> - Install Edge Chromium.
>
> - Install All Current Windows Updates. 
>
> - Installed BGinfo and configured a watermark.
>
> - Disable Lock screen.
>
> - Disable Windows Updates.
>
> - Clear all event logs on local machine.
>
> - Set passwords not to expire.
>
> - Set admin password not to expire.
>
> - Disable requirement for **CTRL + ALT + DEL** to sign in.
>
> - Disable and refuse Domain Password change prompts. 
>
> - Clear PowerShell History.
>
> - Clear Run History.
>
> - Disable Network Notifications.
>
> - Clear out Network Profiles.
>
> - Set Network to Private.
>
> - Enable Remote Desktop Access.
>
> - Optimise Visual performance for user.
>
> - Remove recent Programs.
>
> - Create firewall settings for 192.168.10.0/24 network (outbound, inbound).
>
> - Ensure appropriate power settings (Highest avail Performance, Disable monitor timeout).
>
> - Optimise Edge (Policies).
>
> - Configure Edge settings.
>
> - System tray clean up (Open the new Windows 'Settings' app and search for "Turn System Icons on or off"). Only leave Network and Clock.
>
> - Disable Automatic Windows Updates via GPEDiT.
>
>    - Navigated to **Computer Configuration >  Administrative Templates > Windows Components > Windows update**.  
>
>    - **Adjusted the following**: 
>
>    - Configure Automatic Updates : **Disabled**. 
>
>    - Allow Automatic Updates immediate Installation : **Disabled**. 
>
>    - Do not adjust default option to 'Install Updates and Shut Down' in Shut Down Windows dialog box : **Enabled**.  
>
 >   - No auto-restart with logged on users for scheduled automatic updates installations : **Enabled**. 
 > 
>  - Navigated to **Computer Configuration > Administrative Templates > Windows Components > Store**.  
>
>    - **Adjusted the following**:
>
>    - Turn off Automatic Download and Install of updates : **Enabled**.  
>
>    - Turn off Automatic Download of updates on Win machines : **Enabled**.
>  
> -  Hide Recently added apps in Start Menu.
>
>   - **Settings > Personalization > Start >** Show Recently Added apps toggle **OFF**.
>
>  - **GPEDIT > Computer Configuration > Adminstrative Templates > Start Menu and Taskbar >** Remove "Recently Added" list from start menu **ENABLED**. 
>
> -  Turn Notifications off (System Settings).
>
> -  System Performance Settings, Highest Performance available (Best Performance, Ultimate Performance, Check Smooth Edges Screen Fonts). 
>
> -  Power Display Settings to Never Shut Off. 
>
> -  Clear Windows Updates Cache. 
>
> -  Empty the Recycle Bin. 
>
> -  Power & Sleep > Screen turn off **Never**.
>

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

>[!hint] Want to learn more? Review the documentation on [Building virtual machines](https://docs.skillable.com/v1/docs/best-practices-for-building-virtual-machines) on our platform.

## Networks

- **WebNAT**

>[+] Network Configuration
>
|Item|Detail|
|:----|:----|
|Type|**Web Access (NAT)**|
|Gateway|+++192.168.100.1+++|
|Subnet Mask|+++255.255.255.0+++|
|DHCP Enabled|+++192.168.100.100+++ to +++192.168.100.200+++|

>[!hint] Want to learn more? Review the documentation on [Networking](https://docs.skillable.com/v1/docs/implementing-network-policies-and-managing-restrictions-for-lab-environments) in a lab profile.

## Cloud
There are no Cloud settings in this lab profile.

>[!hint] Want to learn more? Review the documentation on [Skillable Cloud Fabrics](https://docs.skillable.com/docs/cloud-fabric-explanation).

## Life Cycle
This lab profile contains a Life Cycle Action to implement licensing for the Windows Server virtual machine.

>[!hint] Want to learn more? Review the documentation on [Life Cycle Actions](https://docs.skillable.com/docs/life-cycle-actions-5).
