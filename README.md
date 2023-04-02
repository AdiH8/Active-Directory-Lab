# Basic Home Lab Running Active Directory

This repository contains steps on how i set up a basic home lab running Active Directory following a tutorial by [Josh Madakor](https://www.youtube.com/@JoshMadakor)

## Diagram
![Diagram](active_directory_diagram.jpg)

## Download and install Oracle VirtualBox from the official website.
[Oracle Virtual Box](https://www.virtualbox.org/)

## Download the Windows 10 and Server 2019 ISO files.
[Windows 10 iso](https://www.microsoft.com/en-us/software-download/windows10ISO)
[Windows Server 2019](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019)

## Create a new virtual machine by clicking on "New" in VirtualBox, naming it "Domain Controller," and selecting the "Windows Server 2019" ISO file as the boot media.

![](attachments/Pasted%20image%2020230402145533.png)

![](attachments/Pasted%20image%2020230402145610.png)

##  Configure the virtual machine by giving it two network adapters: one for connecting to the internet and the other for the private network.

![](attachments/Pasted%20image%2020230402145806.png)

![](attachments/Pasted%20image%2020230402145820.png)

##  Install Server 2019 on the virtual machine and assign IP addressing for the internal network.

![](attachments/Pasted%20image%2020230402150458.png)

![](attachments/Pasted%20image%2020230402150538.png)
##  Name the server and install Active Directory to create the domain.
![](attachments/Pasted%20image%2020230402150727.png)

![](attachments/Pasted%20image%2020230402153253.png)

##  Configure routing so that clients on the private network can access the internet through the domain controller.

![](attachments/Pasted%20image%2020230402153829.png)

![](attachments/Pasted%20image%2020230402153904.png)

![](attachments/Pasted%20image%2020230402154123.png)

##  Set up DHCP on the domain controller.
![](attachments/Pasted%20image%2020230402154312.png)

![](attachments/Pasted%20image%2020230402154041.png)

![](attachments/Pasted%20image%2020230402154439.png)


##  Run the PowerShell script to create 1000 users in Active Directory.

[Power Shell script for creating users](https://github.com/joshmadakor1/AD_PS)

##  Create a new virtual machine named "Client1" and install Windows 10 on it.

![](attachments/Pasted%20image%2020230402155056.png)


##  Connect the client machine to the private network and join it to the domain.

![](attachments/Pasted%20image%2020230402155713.png)

![](attachments/Pasted%20image%2020230402155807.png)

##  Log into the client machine with a domain account.

![](attachments/Pasted%20image%2020230402160005.png)

![](attachments/Pasted%20image%2020230402160120.png)