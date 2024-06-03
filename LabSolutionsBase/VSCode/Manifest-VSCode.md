## Lab Profile Manifest

### Virtual Machines

#### VS Code

>[+] Configuration
>
| Item | Detail | | Item | Detail |
|:---------|:---------| |:---------|:---------|
| User | **empty** | | IP Address   | **DHCP** |
| Password | +++PASSWORD+++ | | CPU(s) | **2** |
| Name   | **VS Code** | | RAM | **2 GB** |
| Platform | **Docker** |

>[+] Software
>
>**VS Code**
>
>VS Code has been installed in this container environment and exposed through a web-based interface for access to the graphical VSCode front-end.
>
>Here are some additional resources on using the [code-server](https://registry.hub.docker.com/r/codercom/code-server/) container image.

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
