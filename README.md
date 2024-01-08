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
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
