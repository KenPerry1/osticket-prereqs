<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### https://www.youtube.com/watch?v=MNgaYilYu2A

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Web Server: A web server, like IIS, Apache, or LiteSpeed, is needed to host the osTicket application.
- PHP: osTicket requires a specific version of PHP, typically 8.1 or 8.2. Older versions may not be supported.
- MySQL Database: Version 5.0 or higher.
- Web Platform Installer: This is helpful for installing the necessary components.
- MySQL User with Privileges: A MySQL user with full privileges on the database created for osTicket.

<h2>Installation Steps</h2>


<p>
<img src<img width="823" alt="image" src="https://github.com/user-attachments/assets/694eddbc-2f3d-4c78-99d7-a0e3812e85ba" />
</p>
<p>
Log in to your Azure account and create a virtual machine. Ensure that the virtual machine has 4 vCPUs and is running Windows.
</p>
<br />

<p>
<img src<img width="791" alt="image" src="https://github.com/user-attachments/assets/7e136629-1767-4e2a-a5b3-77d314b91e19" />
</p>
<p>
Once your virual machine is created, identify the public ip address in order to remotely access it via the Remote Desktop Connection.
</p>
<br />

<p>
<img src<img width="836" alt="image" src="https://github.com/user-attachments/assets/cfbd21fe-7c1a-4cdf-b845-9915800b22e1" />
</p>
<p>
Log into the virtual machine. Gather and download the installation files for osTicket
</p>
<br />

<p>
<img src<img width="827" alt="image" src="https://github.com/user-attachments/assets/bc7bf202-d9c0-4539-908e-64a093054e57" />
</p>
<p>
Unzip the installation files onto the deskop. The new folder should be called osTicket-Installation-Files. OsTicket will be installed from the files in this folder as well as some of the dependencies needed to run it.
</p>
<br />

<p>
<img src<img width="826" alt="image" src="https://github.com/user-attachments/assets/decf647a-da38-47b8-a581-92183cab3e33" />
</p>
<p>
Install/Enable IIS with CGI. This can be achieved by accessing the Control Panel and selecting uninstall a program underneath Programs. On the left there will be an option to Turn Windows features on or off, select that. Then navigate to Internet Information Services and expand it. From there expand World Wide Web Services, expand Application Development Features and select CGI and press ok.
</p>
<br />

<p>
<img src<img width="827" alt="image" src="https://github.com/user-attachments/assets/ffe40a27-4390-4e66-97c8-f19378387584" />
</p>
<p>
From the osTicket-Installation-Files folder, install the PHP manager for IIS. A PHP Manager is a tool that simplifies the installation, configuration, and management of PHP versions and settings on servers, especially those running Windows with IIS.
</p>
<br />

<p>
<img src<img width="824" alt="image" src="https://github.com/user-attachments/assets/f54789f5-ce25-4dd9-aaa4-ac7d6e6cf6ac" />
</p>
<p>
From the osTicket-Installation-Files folder, install the Rewrtie Module. The URL Rewrite Module rewrites request URLs to simple, user-friendly, and search-engine friendly addresses that are displayed to users or in Web applications.
</p>
<br />

<p>
<img src<img width="825" alt="image" src="https://github.com/user-attachments/assets/679eaec8-9613-4558-b84c-426183807edf" />
</p>
<p>
From the C: drive create a folder and name it PHP. 
</p>
<br />

<p>
<img src<img width="826" alt="image" src="https://github.com/user-attachments/assets/93026b8d-f1bd-4643-b31a-76c7d465c032" />
</p>
<p>
Open the osTicket-Installation-Files folder and unzip the php-7.3.8-nts-Win32-VC15-x86.zip into the PHP folder from the C: drive.
</p>
<br />

<p>
<img src<img width="826" alt="image" src="https://github.com/user-attachments/assets/2f8dc127-5168-4d2f-82a7-d75b41d6a1e2" />
</p>
<p>
Go to the osTicket-Installation-Files folder, and install the VC_redist.x86.exe. Redistributable software, like Microsoft Visual C++ Redistributable packages, are runtime libraries that are required by applications to function correctly.
</p>
<br />

<p>
<img src<img width="824" alt="image" src="https://github.com/user-attachments/assets/58f4dad4-4a40-4eef-be8f-5cb789d28187" />
</p>
<p>
Open the osTicket-Installation-files folder, and install mysql-5.5.62-win32.msi. When installing be sure to select typical setup and to launch configuration wizard after the install. Once the configuration wizard is launched select standard configuration. Be sure to remember the username and password as this user will have full privileges. MySQL is an open-source Relational Database Management System (RDBMS) that stores, manages, and retrieves structured data. It uses Structured Query Language (SQL) to interact with databases and is widely used in various applications, from small projects to large websites.
</p>
<br />

<p>
<img src<img width="826" alt="image" src="https://github.com/user-attachments/assets/6b84a657-5af1-42dd-bb7a-7e81702fbe37" />
</p>
<p>
Open IIS as an administrator 
</p>
<br />

<p>
<img src<img width="827" alt="image" src="https://github.com/user-attachments/assets/a6686999-ddaf-4308-b214-43e34fef9d23" />
</p>
<p>
From within IIS, select PHP Manager, register PHP, and then reload IIS by stopping and starting it on the right of the screen.
</p>
<br />

<p>
<img src<img width="824" alt="image" src="https://github.com/user-attachments/assets/d6b49853-17a2-4f4c-b8c2-cc5c144bb458" />
</p>
<p>
Open the osTicket-Installation-Files folder and unziip the osTicket-v1.15.8.zip folder.
</p>
<br />

<p>
<img src<img width="824" alt="image" src="https://github.com/user-attachments/assets/27a22240-eaab-4337-9695-0a007ad12b59" />
</p>
<p>
Within the osTicket-v1.15.8 folder there will be another folder named upload. The upload folder needs to be copied into the C:\inetpud\wwwroot. A good way to do this is to open another file explorer and navigate to C:\inetpub\wwwroot. From within the osTicket-v1.15.8 folder, drag the upload folder into to wwwroot folder. Make sure the upload folder also gets renamed as osTicket.
</p>
<br />

<p>
<img src<img width="827" alt="image" src="https://github.com/user-attachments/assets/16754c40-7157-4ac9-8f6a-c2e58c824e38" />
</p>
<p>
Relaod IIS by stopping it and starting it on the right side. Go to Sites on the left side, select Default Web Site, and then select osTicket. On the right of the screen select Browse*:80. The osTicket installer will populate and you will see that there are some extentions that still need to be enabled.
</p>
<br />

<p>
<img src<img width="827" alt="image" src="https://github.com/user-attachments/assets/f1a9c305-d1ac-43be-a64c-ec8bacbe1f44" />
</p>
<p>
Open IIS and go to Sites on the left side of the screen. Select Default Web Site and then osTicket. From there double click PHP Manager and select enable or disable an extentention at the bottom of the page.
</p>
<br />

<p>
<img src<img width="827" alt="image" src="https://github.com/user-attachments/assets/173fd9c7-eae0-4576-8ebf-ab974a22439d" />
</p>
<p>
Enable these three extentions: php_imap.dll, php_intl.dll, and php_opcache.dll. The php_imap.dll extention is a Dynamic Link Library (DLL) for the PHP programming language that provides functionality to interact with Internet Message Access Protocol (IMAP) servers. This extension allows PHP scripts to connect to mailboxes, read emails, and manage messages stored on an IMAP servers. the php_intl.dll extention is designed to handle different locales and languages correctly, ensuring proper text formatting, sorting, and other locale-dependent operations. The php_opcache.dll is a PHP extension that acts as a cache for PHP scripts, significantly improving performance.
</p>
<br />

<p>
<img src<img width="827" alt="image" src="https://github.com/user-attachments/assets/46e6e76a-28f5-439e-86b3-3214b9521793" />
</p>
<p>
Navigate to C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php. Rename ost-sampleconfig.php to ost-config.php. 
</p>
<br />

<p>
<img src<img width="825" alt="image" src="https://github.com/user-attachments/assets/35f6db6a-cfbd-48da-b8d5-165bb505c272" />
</p>
<p>
Right click on ost-config.php to disable inheritance and assign new permissions. Select properties after you right click on ost-config.php. At the top select Security and then select advanced. There will be a button the says disable inheritance select it and disable the inheritance for everyone. 
</p>
<br />

<p>
<img src<img width="824" alt="image" src="https://github.com/user-attachments/assets/11a578c4-6145-42aa-a2a0-9bf058b42528" />
</p>
<p>
Add a new Permission that will allow everyone full access. Select Add and the at the top click select a principal. Type everyone where it says enter the objects name. Give everyone full access and select ok at the bottom. Select apply and then ok. This step for the permissions is only for demonstrative purposes as in a real world setting it is a security risk to allow everyone full access. 
</p>
<br />

<p>
<img src<img width="826" alt="image" src="https://github.com/user-attachments/assets/3730928a-69ad-45dc-b2ee-ee11a2e004c0" />
</p>
<p>
Open File Explorer and go to the osTicket-Installation-Files folder. From there install HeidiSQL.
</p>
<br />

<p>
<img src<img width="826" alt="image" src="https://github.com/user-attachments/assets/c14bfd56-3dce-4e61-a8fd-3906b8e3a7d1" />
</p>
<p>
Create a new session within HeidiSQL. Create a new database named osTicket. 
</p>
<br />

<p>
<img src<img width="827" alt="image" src="https://github.com/user-attachments/assets/14650d26-ae82-442f-91f1-a890bdd7c6a5" />

</p>
<p>
Continue the Installation of osTicket.
</p>
<br />

<p>
<img src<img width="827" alt="image" src="https://github.com/user-attachments/assets/c8308de8-34ff-45e7-834d-6fb69012a635" />
</p>
<p>
Upon completion of the osTicket installation, the congradualtion page will apear with all the necessary links for osTicket. 
</p>
<br />
