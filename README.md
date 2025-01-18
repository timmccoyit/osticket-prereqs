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

- PHP Manager for IIS: Makes sure IIS can run PHP, which osTicket depends on.
- URL Rewrite Module for IIS: Ensures that osTicket's URLs are clean and easy to use.
- C:\PHP Folder: A folder where PHP will be stored and used by your server.
- PHP 7.3.8: The programming language required to run osTicket.
- VC Redist: The necessary Visual C++ libraries to ensure PHP works properly on Windows.
- MySQL: The database system used to store all of osTicket’s data, such as tickets and settings.

<h2>Installation Steps</h2>

![image](https://github.com/user-attachments/assets/7ff9b380-668e-47cb-a3e7-6497629b082b)
![image](https://github.com/user-attachments/assets/0d604329-6688-4b72-a04b-47778f8847f5)

<p>
First, we created our windows 10 virtual machine in microsoft azure then we remote desktop into and install Internet Information Services(IIS) with CGI. After this, we create a folder named PHP in our C directory to put the PHP files into for osTicket.
</p>
<br />

![image](https://github.com/user-attachments/assets/ba8f2f51-e842-410e-a42c-534987c80a31)
![image](https://github.com/user-attachments/assets/e048e821-1cdc-42bb-bc2c-3a241b7f38a0)

<p>
Then, we take our folder with all the dependencies in osTicket inside and start installing these dependencies one by one. After I install the last thing which is MySQL, then we open IIS as an Admin and register PHP from within IIS (PHP Manager --> direct to php-cgi.exe file.
</p>
<br />

![image](https://github.com/user-attachments/assets/69d6ee35-81bd-4603-a663-00897a97dd82)
![image](https://github.com/user-attachments/assets/447a59db-bacb-45fd-8487-ed9cda91b3e6)

<p>
Now we're installing osTicket itself and reloading IIS once more so we can go to site or landing page for osTicket. On this page, it states that some extensions are still not enabled so I go to the PHP manager and manually enable them then refresh osticket.
</p>
<br />

![image](https://github.com/user-attachments/assets/12d65354-8495-4a11-8c41-623e725601c4)
![image](https://github.com/user-attachments/assets/86c7c473-4b0c-4aab-afb3-c69caf0ed18c)

<p>
I then rename the config file for osticket then assign permissions to ost-config.php to give everyone permissions. Next, i install HeidiSQL to create the database for our ticketing system then continue setting up osticket in the browser.
</p>
<br />
