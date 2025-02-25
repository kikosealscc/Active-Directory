# Active-Directory
<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://youtu.be/LR8009GgGAQ?si=syY1sraHCO-mtzEc)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows 11 Pro (23H2)
- Windows Server 2022

<h2>High-Level Deployment and Configuration Steps</h2>

- Create Virtual Machines 
- Configure Network Settings
- Allow Firewall Permissions
- Install Active Directory

<h2>Deployment and Configuration Steps</h2>

<p>


  
![image](https://github.com/user-attachments/assets/aa2cca08-2159-4366-896f-a10f35ba5bd8)

</p>
<p>

  
Provision Azure Virtual Machines: Create two virtual machines in Azure. One will serve as the Domain Controller (DC) running Windows Server, and the other will be a client machine running Windows 11. 
</p>
<br />

<p>

  ![image](https://github.com/user-attachments/assets/db87d851-8ebf-47d7-a89c-ffa38d1daefa)

</p>
<p>
Configure Networking: Ensure connectivity between the two virtual machines by configuring the virtual network and subnet settings. Enable Remote Desktop access on both machines. 
</p>
<br />

<p>

  ![image](https://github.com/user-attachments/assets/fc3a815d-bff8-45bb-bbea-05d7fd56153e)

</p>
<p>
  
Install Active Directory Domain Services: On the Windows Server VM, use the Server Manager to install the "Active Directory Domain Services" role. Promote the server to a Domain Controller and create a new domain
</p>
<br />


![image](https://github.com/user-attachments/assets/3d1b0502-70cb-41e8-8f2e-a92b9fe4df57)

Join Client to Domain: On the Windows 10 VM, adjust the network settings to use the Domain Controller's IP address as the primary DNS server. Join the client machine to the newly created domain and validate connectivity.

