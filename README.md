![osTicketImage](https://github.com/user-attachments/assets/4288550c-e3df-4f74-b292-eb7aa85c8e28)

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 11</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure
- Virtual Machine
- osTicket and all other dependencies

<h3>Installation Steps</h3>

- Create Resource Group and Virtual Machine in Azure
- Install IIS in Windows with CGI on our Virtual Machine
- Install osTicket and all other dependencies on our Virtual Machine
  - Install PHP Manager for IIS
  - Install the Rewrite Module
  - Create the directory C:\PHP
  - Unzip PHP 7.3.8 into the “C:\PHP” folder
  - Install VC_redist.x86.exe
  - install MySQL 5.5.62
  - Register PHP from within IIS then reload it
  - Install osTicket
  - Reload IIS again then go to sites -> Default -> osTicket
  - In IIS click “Browse *:80” on the right
  - Enabled the proper extensions for osTicket in IIS
  - Assign Permissions for osTicket
- Setup osTicket in browser
  - Create profile
  - Install HeidiSQL and create osTicket database
  - Enter database info into the database setting and click "Install Now"
- Success!

____________________________________________________________________________________________________________________________
<p>
Create a resourse group and virtual machine in Azure and get IP address to open Remote Desktop. 
</p>
<br />


![GithubSnip1](https://github.com/user-attachments/assets/73eeba0a-2d82-4ec5-b1e9-e8117efe605f)


<p>
Inside the vitrual machine, search Windows for the IIS Manager and open it as an administrator. Activate Internet Information Services. Then open World Wide Web Services -> Application Development Features -> and activate CGI.
</p>
<br />


![GithubSnip3](https://github.com/user-attachments/assets/7ef93750-7ba7-4f69-b9d0-7be136c03f8d)





![GithubSnip4](https://github.com/user-attachments/assets/6b06f38a-6b9d-40cd-ad70-14a7f3895a89)



<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />





<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />





<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />





<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
