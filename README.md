<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine
- Internet Information Services (IIS)
- PHP Manager
- Rewrite Module
- VC Redist
- MySQL
- Heidi SQL
- osTicket v1.15.8
- Link to downloads: https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6

<h2>Installation Steps</h2>

<p>
1. Create a Virtual Machine and Resource group in Azure by going to portal.azure.com. The setup must include windows 10 and at least 2 vcpu's.
 </p>
 
 ![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/f29aa35b-24b6-4a58-b0b4-c6686a0e402e)

 ![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/8d9177ad-5bd4-41ce-a9d9-28e9a640f063)

 <p>
  Note: Make sure you remember your username and password as you'll need it to log into the Virtual Machine.
 </p>

 ![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/03678507-a2a8-400f-8a07-24a9b045c04f)

 <br />

<p>
2. Once your Resource Group and Virtual Machine is created we are going to connect to the Virtual Machine using Remote Desktop Connection. Copy the public IP address of your Virtual Machine and paste it into Remote Desktop Connection.
</p>

![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/87ca327d-b275-47e2-8fa5-2ec3831f0730)

![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/0ff0ebb5-5c14-4a81-be33-6c28aa6cad74)

<p>
 Next put the username and password you made into Remote Desktop Connection. (If another random username comes up navigate to more choices and it will give you the option to put another user name).
</p>

![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/ecd234b0-9cab-4f7c-a3ef-8ad6df0e3bf6)

<br />

<p>
3. Once you've officially logged into your new Virtual Machine the next step is to enable IIS. So firstly open your control panel and navigate to programs.
</p>

![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/26ab9408-c94f-4fdb-a86b-30f66702d40d)

<p>
Next click on Turn Windows features on or off
</p>

![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/99519c1e-27f5-4b70-874e-5d92ed8bb183)

<p>
 Now find Internet Information Services and check that
</p>

![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/e061b84c-f6b5-48f1-b618-9f8e04d3642c)

<p>
 Next navigate to World Wide Web Services -> Application Development Features ->
[X] CGI
[X] Common HTTP Features
</p>

<p>
 Next navigate to Internet Information Services -> Web Management Tools -> IIS Management Console
	[X] IIS Management Console
</p>

![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/702901e7-1b78-4a99-89f1-ae50376a6d48)

<p>
 To check if youve successfully enabled IIS in your Virtual Machine go to your browser and type in 127.0.0.1, and if this page comes up then you've successfully enabled IIS. 
</p>

![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/1e2078f4-33f3-47dc-a071-2087ca8b1e95)

<br />

<p>
4. For the next step we'll have to down load some files, first one is going to be PHP Manager for IIS. Navigate to your installation files on click download on PHP Manager for IIS.
</p>

![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/ed63e59c-2ff2-4ee9-8840-d83f10567d62)

<p>
After its downloaded go through the installation process and then navigate to the installation files and do the same thing and download the Rewrite Module.
</p>

![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/28f912fe-f0fc-4910-b1e1-0991ba3385f3)

<br />

<p>
5. The next step is to create a directory for a future download, navigate to your C drive and create a new folder called PHP.	
</p>

![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/df061eed-e36c-4b76-a16d-b2521e62fe4e)

<br />

<p>
6. Next we are going to navigate back to our installation files and download PHP 7.3.8.
</p>

![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/c4a8cf75-cc87-4d13-a8cc-2d5323d9c682)

<p>
One the file is downloaded go to it and right click it and extract it to your PHP folder we just made in your C drive.
</p>

![image](https://github.com/DevinWilliamsIT/osticket-prereqs/assets/155914712/236283a1-9d7d-48cd-97b9-acce7ffecc9b)



