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
<br />
<img src="https://i.imgur.com/y0W7KBn.png" height="80%" width="80%" alt="Active Directory Steps"/>
<p align="center">
Assign two network adapters to this virtual machine: one for connecting to the internet and another for the private network within VirtualBox.<br />
<br />
<img src="https://i.imgur.com/tBcFTnf.png" height="80%" width="80%" alt="Active Directory Steps"/>
<img src="https://i.imgur.com/EHMGaxq.png" height="80%" width="80%" alt="Active Directory Steps"/>

<h3>Install Windows Server 2019</h3>
<p align="center">
Install Windows Server 2019 on the domain controller virtual machine.<br />
<br />
<img src="https://i.imgur.com/xpBriyk.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Configure IP addressing for the internal network.<br />
<br />
<img src="https://i.imgur.com/D1USxjC.png" height="80%" width="80%" alt="Active Directory Steps"/>

<h3>Setup and Configure Active Directory</h3>
<p align="center">
Install Active Directory.<br />
<br />
<img src="https://i.imgur.com/4vyc3lS.png" height="80%" width="80%" alt="Active Directory Steps"/>
<img src="https://i.imgur.com/auFbG1x.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Adding remote access <br />
<br />
<img src="https://i.imgur.com/kHXsA7o.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Configure routing so that clients on the private network can access the internet through the domain controller using NAT.<br />
<br />
<img src="https://i.imgur.com/odjpSEF.png" height="80%" width="80%" alt="Active Directory Steps"/>

<h3>Setup DHCP on the Domain Controller</h3>
<p align="center">
Adding DHCP<br />
<br />
<img src="https://i.imgur.com/8yJPLIK.png" height="80%" width="80%" alt="Active Directory Steps"/>  
<br />
<br />
Configure DHCP scope to enable automatic IP address assignment for the Windows 10 client machine.<br />
<br />
<img src="https://i.imgur.com/FkoG6Ea.png" height="80%" width="80%" alt="Active Directory Steps"/> 
<img src="https://i.imgur.com/x1KnGPQ.png" height="80%" width="80%" alt="Active Directory Steps"/> 
<img src="https://i.imgur.com/vAbauTT.png" height="80%" width="80%" alt="Active Directory Steps"/> 
  
<h3>Create Users with PowerShell</h3>
<p align="center">
Running a PowerShell script on the domain controller to automatically create 1,000 users in Active Directory.<br />
<br />
<img src="https://i.imgur.com/06V9p24.png" height="80%" width="80%" alt="Active Directory Steps"/>   
<img src="https://i.imgur.com/QiMYFVD.png" height="80%" width="80%" alt="Active Directory Steps"/>   

<h3>Create the Windows 10 Client Virtual Machine</h3>
<p align="center">
Create another virtual machine and assign the network adapter to internal.<br />
<br />
<img src="https://i.imgur.com/PgBHddn.png" height="80%" width="80%" alt="Active Directory Steps"/>
<img src="https://i.imgur.com/7869JA7.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Install windows 10<br />
<br />
<img src="https://i.imgur.com/Uw1Hewn.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Name the machine "client1" and join it to the domain.<br />
<br />
<img src="https://i.imgur.com/8bsXSnY.png" height="80%" width="80%" alt="Active Directory Steps"/>
<img src="https://i.imgur.com/CnY7Rlv.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
<br />
Log into the client machine using one of the domain accounts.<br />
<br />
<img src="https://i.imgur.com/alWgF89.png" height="80%" width="80%" alt="Active Directory Steps"/>
<img src="https://i.imgur.com/L4t0JBa.png" height="80%" width="80%" alt="Active Directory Steps"/>

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
