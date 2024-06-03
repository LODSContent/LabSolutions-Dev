## Lab Profile Manifest

### Virtual Machines

#### LAMP VM

>[+] VM Configuration
>
| Item | Detail | | Item | Detail |
|:---------|:---------| |:---------|:---------|
| User | +++@lab.VirtualMachine(ubuntudesktop22.04).Username+++ | | IP Address   | **DHCP**   |
| Password | +++@lab.VirtualMachine(ubuntudesktop22.04).Password+++ | | CPU(s) | **4** |
| Name   | **labuser-virtual-machine** | | RAM | **4 GB** |
| Platform | **ESX** | | HD 1 | **100 GB** |
| OS | **Ubuntu Desktop v22.04** | | NIC(s) | **2** |


>[+]  VM Optimizations
>
- Updated Ubuntu:
>
    ```bash
    set -e
    sudo apt-get update
    sudo apt-get upgrade
    sudo apt-get dist-upgrade
    ```
- Installed Python 3: ++sudo apt install python3-pip++
- Installed VMware Tools: ++sudo apt-get install open-vm-tools-desktop -y++
- Disabled automatic updates:
>
    ```bash
    sudo systemctl disable --now unattended-upgrades
    echo 'APT::Periodic::Update-Package-Lists "0";' | sudo tee /etc/apt/apt.conf.d/20auto-upgrades
    echo 'APT::Periodic::Unattended-Upgrade "0";' | sudo tee -a /etc/apt/apt.conf.d/20auto-upgrades
    ```
- Removed background image and set the background to dark grey:   
>
    ```bash
    gsettings set org.gnome.desktop.background picture-uri none
    gsettings set org.gnome.desktop.background primary-color '#333333'
    ```
- Cleared history: ++history -c++

>[+]  Software
>
This is a base VM with basic tools and Python language available. There are no additional tools currently on this machine. 

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
