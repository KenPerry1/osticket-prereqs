<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### https://www.youtube.com/watch?v=MNgaYilYu2A

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Web Server: A web server, like IIS, Apache, or LiteSpeed, is needed to host the osTicket application.
- PHP: osTicket requires a specific version of PHP, typically 8.1 or 8.2. Older versions may not be supported.
- MySQL/MariaDB Database: A server like MySQL or MariaDB must store osTicket's data. 
- osTicket Database: A dedicated database within your MySQL/MariaDB server to store specifically osTicket data.
- MySQL User with Privileges: A MySQL user with full privileges on the database created for osTicket.

<h2>Installation Steps</h2>

<p>
<img src"<img width="1022" alt="image" src="https://github.com/user-attachments/assets/14796cd6-3242-40c8-92c9-927c1230eb7f" />

</p>
<p>
It is necessary to use Azure to create a virtual machine. Once a virtual machine is created, use Remote Desktop Connection to access the virtual machine. Moving forward, gathering and downloading the installation files is paramount.
</p>
<br />

<p>
<img src<img width="1027" alt="image" src="https://github.com/user-attachments/assets/e98b04f1-8671-489f-a183-95882e0ead25" />

</p>
<p>
Installing PHP and MySQL is the next step.
</p>
<br />

<p>
<img src<img width="1023" alt="image" src="https://github.com/user-attachments/assets/58f3147a-aa36-4c67-8c30-17e30e892783" />


</p>
<p>
Next, open IIS as an admin and register PHP. Once registered, install the osTicket file in C:\inetpub\wwwroot. After completing, restart IIS, and the web browser will display the osTicket installation page. PHP now requires extension configuration for an improved help desk experience.
</p>
<br />

<p>
<img src<img width="1022" alt="image" src="https://github.com/user-attachments/assets/ef0e0e97-133f-4120-ba8b-9897c31875bd" />

</p>
<p>
Install HeidiSQL, create a new session, and a database. Name the new database osTicket.
</p>
<br />

<p>
<img src<img width="1022" alt="image" src="https://github.com/user-attachments/assets/788d8254-864b-4ad5-9964-5dc0aa955ee5" />

</p>
<p>
Finish the browser installation for osTicket.
</p>
<br />

<p>
<img src<img width="1016" alt="image" src="https://github.com/user-attachments/assets/232e9961-7cc9-40cb-8060-71926115862a" />

</p>
<p>
Now that the installation is complete, the osTicket login page can be reached.
</p>
<br />
