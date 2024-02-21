<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://youtu.be/aZq_ja7qrJg)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Setup Resources in Azure and Ensure Connectivity between Client-1 and DC-1 (Domain Controller)
- Install Active Directory, Create Admin, and Change Client-1 DNS Private IP Address
- Join Client-1 to Active Directory Domain and Setup Remote Desktop for Non-Administrative Users on Client-1
- Create a large group of additional users

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/eC1DU5b.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<img src="https://i.imgur.com/lyYJ68g.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<img src="https://i.imgur.com/poba1gD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


Creating the virtual machine DC-1 as the domain controller and creating virtual machine Client-1 as admin/employee work station allowed me to test network connectivity and communication.
</p>
<br />

<p>
<img src="https://i.imgur.com/DZP092O.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
</p>
<img src="https://i.imgur.com/gYFZG5L.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<img src="https://i.imgur.com/NJJ4Uij.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<p>
The purpose of Active Directory is to centralized, authentication, authorization, and management of network resources. This includes users, computers, groups, and devices within an organization's network. Jane Doe was created as Admin. Client-1 DNS private ip address is being pointed to DC-1 private id address.
  
</p>
<br />

<p>
<img src="https://i.imgur.com/o53xbHr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  
</p>
<img src="https://i.imgur.com/Uhpew83.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<img src="https://i.imgur.com/tjZmfaP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Joining Client-1 to DC-1 for the purpose of accessing and management. Giving employees remote access to DC-1. Creating 2000 employees with their own username and same passowrd.

</p>
<br />
