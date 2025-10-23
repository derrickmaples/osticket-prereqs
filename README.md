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
  - Install MySQL 5.5.62
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


<p>
Install PHP Managerf for IIS
</p>
<br />


![GithubSnip4](https://github.com/user-attachments/assets/6b06f38a-6b9d-40cd-ad70-14a7f3895a89)


<p>
Install the Rewrite Module
</p>
<br />


![GithubSnip5](https://github.com/user-attachments/assets/0ff29075-2c57-4dea-b146-2ac89914202d)


<p>
Create the directory C:\PHP
</p>
<br />


![GHSnip6](https://github.com/user-attachments/assets/879ec589-dc6e-4c35-93e0-cf3b9453130f)



<p>
Unzip PHP 7.3.8 into the “C:\PHP” folder
</p>
<br />

![GHSnip7](https://github.com/user-attachments/assets/8be1fcb5-8126-4f6c-86b3-0d66601f420b)


<p>
Install VC_redist.x86.exe
</p>
<br />

![GHSnip8](https://github.com/user-attachments/assets/1f7c5d78-30d1-46e5-94ec-a9d2d76e37c9)


<p>
Install MySQL 5.5.62
</p>
<br />


![GHSnip9](https://github.com/user-attachments/assets/bc408ca8-cf5b-478a-8c3f-868846353c29)


<p>
Register PHP from within IIS then reload it
</p>
<br />


![GHSnip10](https://github.com/user-attachments/assets/ddc2cb48-1249-4975-b32a-cd7da9d5a3b0)
![GHSnip11a](https://github.com/user-attachments/assets/f9b6b927-f658-476c-b53f-da1b19f8fc7f)
![GHSnip11b](https://github.com/user-attachments/assets/8941c1bc-a5ce-4f2d-90ab-eb46c134e2c6)


<p>
Install osTicket
</p>
<br />


![GHSnip12](https://github.com/user-attachments/assets/a7dc5693-33e4-4326-87d7-c8d8532b560c)


<p>
Reload IIS again then go to sites -> Default -> osTicket
</p>
<br />


![GHSnip12a](https://github.com/user-attachments/assets/1fd5843f-ee65-403e-b33f-604c13c314cd)


<p>
In IIS click “Browse *:80” on the right
</p>
<br /


![GHSnip12b](https://github.com/user-attachments/assets/0d6b53ae-a568-43d1-af39-e09f83355dec)























