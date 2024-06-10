<h1>Active Directory Home Lab</h1>



<h2>Description</h2>
This project showcases the creation of a home lab environment using Active Directory, providing hands-on experience with this critical technology. Setting up a home lab offers a unique opportunity to gain practical skills and a deep understanding of Active Directory's setup and functionality. Mastering these foundational aspects is essential for those aiming to secure and manage Active Directory environments effectively.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Oracle Virtual Box</b> 

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>
** Create the Domain Controller Virtual Machine**  <br/>

- <b>Create the first virtual machine, which will act as the domain controller housing Active Directory.</b> 
- <b>Assign two network adapters to this virtual machine: one for connecting to the internet and another for the private network within VirtualBox.</b> 

Install Windows Server 2019  <br/>
Install Windows Server 2019 on the domain controller virtual machine.
Configure IP addressing for the internal network. The external network will automatically receive IP addresses from your home network/router.
Setup and Configure Active Directory
Name the server and install Active Directory.
Create a new domain and configure routing so that clients on the private network can access the internet through the domain controller.
Setup DHCP on the Domain Controller
Configure DHCP on the domain controller to enable automatic IP address assignment for the Windows 10 client machine.
Create Users with PowerShell
Run a PowerShell script on the domain controller to automatically create 1,000 users in Active Directory.
Explain the script to provide insight into PowerShell's capabilities and its potential uses.
Create the Windows 10 Client Virtual Machine
Create another virtual machine and install Windows 10 on it.
Connect this virtual machine to the private VirtualBox network.
Name the machine "client1" and join it to the domain.
Log into the client machine using one of the domain accounts.
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
