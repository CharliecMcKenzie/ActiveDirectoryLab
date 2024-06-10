<h1>Active Directory Home Lab</h1>
<p align="center">
<img src="https://i.imgur.com/rm8a6tf.png" height="80%" width="80%" alt="Active Directory Steps"/>

<h2>Description</h2>
This project showcases the creation of a home lab environment using Active Directory, providing hands-on experience with this critical technology. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Oracle Virtual Box</b> 

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<h3>Create the Domain Controller Virtual Machine</h3>  
<p align="center">
Create the first virtual machine, which will act as the domain controller housing Active Directory.<br />
<p align="center">
Assign two network adapters to this virtual machine: one for connecting to the internet and another for the private network within VirtualBox.<br />

<h3>Install Windows Server 2019</h3>
<p align="center">
Install Windows Server 2019 on the domain controller virtual machine.<br />
Configure IP addressing for the internal network.<br />
<br />
<img src="https://i.imgur.com/hUl3t0U.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />

<h3>Setup and Configure Active Directory</h3>
<p align="center">
Name the server and install Active Directory.<br />
<p align="center">
Create a new domain and configure routing so that clients on the private network can access the internet through the domain controller.<br />

<h3>Setup DHCP on the Domain Controller</h3>
<p align="center">
Configure DHCP on the domain controller to enable automatic IP address assignment for the Windows 10 client machine.<br />
    
<h3>Create Users with PowerShell</h3>
<p align="center">
Run a PowerShell script on the domain controller to automatically create 1,000 users in Active Directory.<br />
<br />
<img src="https://i.imgur.com/9S11OKc.png" height="80%" width="80%" alt="Active Directory Steps"/>   
<br />

<h3>Create the Windows 10 Client Virtual Machine</h3>
<p align="center">
Create another virtual machine and install Windows 10 on it.<br />
<p align="center">
Connect this virtual machine to the private VirtualBox network.<br />
<p align="center">
Name the machine "client1" and join it to the domain.<br />
<p align="center">
Log into the client machine using one of the domain accounts.<br />
<br />
<img src="https://i.imgur.com/alWgF89.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
This concludes the tutorial, demonstrating the process of setting up a home lab with Active Directory, creating a domain controller, and adding a client machine to the domain.



<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
