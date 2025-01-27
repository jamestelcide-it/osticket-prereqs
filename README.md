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

- Open OS Ticket Documentation for detailed information on prerequisites
- Download PHP Manager for IIS
- Download IIS URL Rewrite Module
- Download and Install HeidiSQL
- Download mySQL

<h2>Installation Steps</h2>

<p>
<img src="https://github.com/user-attachments/assets/6ca54f03-ef5b-4405-b9e1-80170b912c3d" height="80%" width="80%" alt="osTicket Steps"/>

<!-- ![image](https://github.com/user-attachments/assets/6ca54f03-ef5b-4405-b9e1-80170b912c3d) -->
</p>

<p>
Go within the control panel, then Programs, then Programs and Features, then click on the left hand side of the panel that says Turn Windows features on or off. Here we can check the box for Internet Information Services (IIS), we also need to check CGI here as well.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/25e1c0a2-7720-4a97-b8b7-254abd6ec6cc" height="80%" width="80%" alt="osTicket Steps"/>
 <!-- ![image](https://github.com/user-attachments/assets/25e1c0a2-7720-4a97-b8b7-254abd6ec6cc) -->
</p>
<p>
Next we install PHPManagerForIIS because osTicket runs on PHP and is required to make osTicket Work.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/147d79c7-23d5-4bd2-8680-37d9a3e6a353" height="80%" width="80%" alt="osTicket Steps"/>
<!-- ![image](https://github.com/user-attachments/assets/147d79c7-23d5-4bd2-8680-37d9a3e6a353) -->

</p>
<p>
Next we install another requirement for osTicket the rewrite module.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/a0226083-7991-4764-b43e-4e34449fa2d0" height="80%" width="80%" alt="osTicket Steps"/>
<!--  ![image](https://github.com/user-attachments/assets/a0226083-7991-4764-b43e-4e34449fa2d0) -->

</p>
<p>
Next we can create a new folder on the C:\ called PHP and we can install our php language files in here.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/637d3b78-d9d9-48e7-8c13-79164f36895f" height="80%" width="80%" alt="osTicket Steps"/>
<!-- ![image](https://github.com/user-attachments/assets/637d3b78-d9d9-48e7-8c13-79164f36895f) -->
</p>
<p>
Next we can install the VC_redistx86 file
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/396e6664-cc47-4b87-9618-e02c0b80ff61" height="80%" width="80%" alt="osTicket Steps"/>
<!-- ![image](https://github.com/user-attachments/assets/396e6664-cc47-4b87-9618-e02c0b80ff61) -->
</p>
<p>
Next we can install MySQL 5.5.62, this will give us a database that OS ticket will store all our data in
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/d0279c80-49ed-4d33-ba52-19b2e8b2b8d0" height="80%" width="80%" alt="osTicket Steps"/>
 <img src="https://github.com/user-attachments/assets/56c4d3e8-c29d-4129-92ee-dcbbd164fb51" height="80%" width="80%" alt="osTicket Steps"/>
<!-- ![image](https://github.com/user-attachments/assets/d0279c80-49ed-4d33-ba52-19b2e8b2b8d0) -->
<!-- ![image](https://github.com/user-attachments/assets/56c4d3e8-c29d-4129-92ee-dcbbd164fb51) -->

</p>
<p>
Next we can run IIS as an admin and here we can register PHP from within IIS
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/28e126a5-9793-428a-85a0-6390f3f04984" height="80%" width="80%" alt="osTicket Steps"/>
<!-- ![image](https://github.com/user-attachments/assets/28e126a5-9793-428a-85a0-6390f3f04984) -->

</p>
<p>
Next we can install osTicket into the IIS webroot folder.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/a278b41a-6153-4a4c-93b2-5905dc2ecb7c" height="80%" width="80%" alt="osTicket Steps"/>
<!-- ![image](https://github.com/user-attachments/assets/a278b41a-6153-4a4c-93b2-5905dc2ecb7c) -->
</p>
<p>
Now we should be able to browse to the osTicket setup webpage
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/0403557d-b8f2-4488-949e-57a8369be586" height="80%" width="80%" alt="osTicket Steps"/>
<!-- ![image](https://github.com/user-attachments/assets/0403557d-b8f2-4488-949e-57a8369be586) -->
</p>
<p>
We can then navigate to PHP Extensions in IIS Manager and enable php_imap.dll, php_inti.dll, and php_opache.dll in order to fulfil the previously crossed out recommendations for osTicket
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/4d4ae648-9e71-4e88-8eac-4d99dae00529" height="80%" width="80%" alt="osTicket Steps"/>
<!-- ![image](https://github.com/user-attachments/assets/4d4ae648-9e71-4e88-8eac-4d99dae00529) -->

</p>
<p>
Finally we can finish the basic installation of osTicket.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/68524144-4ce5-4e3e-b421-9851af7095cf" height="80%" width="80%" alt="osTicket Steps"/>
<!-- ![image](https://github.com/user-attachments/assets/68524144-4ce5-4e3e-b421-9851af7095cf) -->
