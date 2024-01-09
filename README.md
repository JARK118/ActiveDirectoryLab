# <h1>Active Directory Home Lab</h1>

 ### [YouTube Demonstration](https://www.youtube.com/watch?v=MHsI8hJmggI&list=PLqBeiU46hx1H--SNfTrohTOWeqkK-M2Y0&index=1&t=1s)

<h2>Description</h2>
In this project I am going to be creating an Active Directory home lab environment using virtual machines on Oracle's VirtualBox. This lab will provide practical skills in Active Directory administration, using Powershell to automate provisions, maintaining, and deprovisioning user accounts. I will also set up a Remote Access Servers (RAS) feature to support NAT/PAT and implement and maintain Windows DNS and DHCP services. 

<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Oracle VirtualBox</b>
- <b>Active Directory</b>
- <b>Windows 10 ISO</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>
- <b>Windows Server 19</b>

<h2>Steps:</h2>

<p align="center">
Architecture of Lab: <br/>
<img src="https://i.imgur.com/NgF8Khd.png" height="80%" width="80%" alt="Architecture of Lab"/>
<br />
<br />

## Download and install Oracle VirtualBox from the official website.
[Oracle Virtual Box](https://www.virtualbox.org/)

## Download the Windows 10 and Server 2019 ISO files.
[Windows 10 iso](https://www.microsoft.com/en-us/software-download/windows10ISO)

[Windows Server 2019](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019)

## Create a new virtual machine by clicking on "New" in VirtualBox, naming it "Domain Controller," and selecting the "Windows Server 2019" ISO file as the boot media.

<img src="https://i.imgur.com/6QSlzAi.png" height="80%" width="80%" alt="Architecture of Lab"/>

<img src="https://i.imgur.com/ONAk46n.png" height="80%" width="80%" alt="Architecture of Lab"/>

##  Configure the virtual machine by giving it two network adapters: one for connecting to the internet and the other for the private network.

<img src="https://i.imgur.com/5vmxtZa.png" height="80%" width="80%" alt="Architecture of Lab"/>

<img src="https://i.imgur.com/5qX3Bt1.png" height="80%" width="80%" alt="Architecture of Lab"/>

##  Install Server 2019 on the virtual machine and assign IP addressing for the internal network.

<img src="https://i.imgur.com/fs2yD6O.png" height="80%" width="80%" alt="Architecture of Lab"/>

<img src="https://i.imgur.com/rf9njlc.png" height="80%" width="80%" alt="Architecture of Lab"/>

##  Name the server and install Active Directory to create the domain.

<img src="https://i.imgur.com/Hp5iV1M.png" height="80%" width="80%" alt="Architecture of Lab"/>

<img src="https://i.imgur.com/LsDOAwG.png" height="80%" width="80%" alt="Architecture of Lab"/>

##  Configure routing so that clients on the private network can access the internet through the domain controller.

<img src="https://i.imgur.com/0rudPHD.png" height="80%" width="80%" alt="Architecture of Lab"/>

<img src="https://i.imgur.com/htnWNZF.png" height="80%" width="80%" alt="Architecture of Lab"/>

<img src="https://i.imgur.com/eRSrpgI.png" height="80%" width="80%" alt="Architecture of Lab"/>

##  Set up DHCP on the domain controller.

<img src="https://i.imgur.com/fwr1sY1.png" height="80%" width="80%" alt="Architecture of Lab"/>

<img src="https://i.imgur.com/kwLPFz9.png" height="80%" width="80%" alt="Architecture of Lab"/>

##  Run the PowerShell script to create 1000 users in Active Directory.

[Power Shell script for creating users](https://github.com/joshmadakor1/AD_PS)

##  Create a new virtual machine named "Client1" and install Windows 10 on it.

<img src="https://i.imgur.com/2k4moxN.png" height="80%" width="80%" alt="Architecture of Lab"/>

##  Connect the client machine to the private network and join it to the domain. Open Command Line Interface and use the ipconfig command.

<img src="https://i.imgur.com/iHsWSDu.png" height="80%" width="80%" alt="Architecture of Lab"/>

<img src="https://i.postimg.cc/GhKtZHvb/Active-Directory-Lab-step-15.png" height="80%" width="80%" alt="Architecture of Lab"/>

##  Log into the client 1 machine with a domain account.

<img src="https://i.postimg.cc/Gt9gdB96/Active-Directory-Lab-step-16.png" height="80%" width="80%" alt="Architecture of Lab"/>


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
