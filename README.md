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
Install osTicket and all other dependencies on our Virtual Machine. I have them all in a file. They were all precollected for the purposes of this lab.
</p>


![GithubSnip2](https://github.com/user-attachments/assets/45174afd-3be4-44cf-ab3b-9ac54dc6ab3b)


<br />
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
Reload IIS again then go to sites -> Default Web Site -> osTicket
</p>
<br />


![GHSnip12a](https://github.com/user-attachments/assets/1fd5843f-ee65-403e-b33f-604c13c314cd)


<p>
In IIS click “Browse *:80” on the right
</p>
<br /


![GHSnip12b](https://github.com/user-attachments/assets/0d6b53ae-a568-43d1-af39-e09f83355dec)


<p>
Enable "php_imap.dll", "php_intl.dll", and "php_opcache.dll" for osTicket in IIS.
</p>
<br /


![GHSnip14](https://github.com/user-attachments/assets/f6ed3739-90b2-4f33-814a-c5697f89fea5)


<p>
Assign Permissions for osTicket by renaming ost-sampleconfig.php to ost-config.php in C:\inetpub\wwwroot\osTicket\include.
Right click ost-config.php and to Properties -> Security -> Advanced -> Disable Inheritence.
Now go to Add -> Select a principle then (for the purposes of this project) add everyone to give permissions.
</p>
<br /


![GHSnip15](https://github.com/user-attachments/assets/976d33de-8a0e-4850-b4d9-484c1424176a)

![GHSnip16](https://github.com/user-attachments/assets/c0176bd0-2ae9-43c4-8d93-0a33426fe8fb)

![GHSnip17](https://github.com/user-attachments/assets/8bd21572-9fb8-4097-b097-c85bf90561ef)


<p>
Setup osTicket in browser. Create a profile for the system. Your default email and your admin user email must be different.
</p>
<br /


![GHSnip18](https://github.com/user-attachments/assets/b8c805cf-5287-4229-b90f-6fc38e3be310)


<p>
Install HeidiSQL and create osTicket database.
</p>
<br /


![GHSnip19](https://github.com/user-attachments/assets/ff87250e-2ecc-48f9-abb4-f12eeacd5dcd)

![GHSnip20](https://github.com/user-attachments/assets/b5dc568b-49c1-4443-aab1-eb1e5dc19548)


<p>
Enter database info into the database setting and click "Install Now".
</p>
<br /


![GHSnip21](https://github.com/user-attachments/assets/af2c5524-be2d-474f-ba30-da708fe65138)


<p>
Success! Now you can log in as an admin. 
</p>
<br /


![GHSnip22](https://github.com/user-attachments/assets/9b0fbf0e-6c34-4562-abc8-8647b427be00)

![GHSnip22a](https://github.com/user-attachments/assets/a89d52a4-4dee-4afc-99c4-cefb88a2895d)
