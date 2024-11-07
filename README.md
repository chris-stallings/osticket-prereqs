<p align="center">
<img width="699" alt="Screenshot 2024-11-07 at 11 36 30 AM" src="https://github.com/user-attachments/assets/8192c223-200b-4535-a9db-9d94974ee30f">

</p>


<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<!--<h2>Video Demonstration</h2>-->

<!-- - ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)-->

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- HeidiSQL

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create a virtual machine running Windows 10.
- Setup Internet Information Services.
- Install PHP on virtual machine.
- Install Rewrite Module.
- Install Microsoft Visual
- Install MySQL

<h2>Installation Steps</h2>

<p>
<img src="https://github.com/user-attachments/assets/7950d93a-a843-4a2e-ac79-d3e728807aa8" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Create a virtual machine running Windows 10. The virtual machine should be have at least 2 CPUs and 16 GiB of memory. 
</p>
<br />
<p><img width="1710" alt="Screenshot 2024-11-04 at 11 37 46 AM" src="https://github.com/user-attachments/assets/82a2239f-f989-4c48-b72c-eef9b149a2b0"></p>
<p>Log into the virtual machine. </p>
<br />
<p><img width="1710" alt="Screenshot 2024-11-04 at 1 37 27 PM" src="https://github.com/user-attachments/assets/05d636eb-06bc-4b16-afbb-e168f25279ee"></p>
<p>Open the control panel and enable internet information services. Also enable CGI. To get to this click World Wide Web Services folder then click Application Development Features. Check the CGI folder. Then press ok. </p>
<br />
<p><img width="1710" alt="Screenshot 2024-11-04 at 11 33 15 AM" src="https://github.com/user-attachments/assets/4e6c7b7d-c7b5-47fc-bde9-a8c77f61aa1a">
</p>
<p>
Install PHP Manager for IIS. </p>
<br />
<p><img width="1710" alt="Screenshot 2024-11-04 at 2 58 52 PM" src="https://github.com/user-attachments/assets/7b06832c-e39e-4227-9434-6389bc90e499"></p>
<p>Install Rewrite Module</p>
<br />
<p><img width="1710" alt="Screenshot 2024-11-04 at 3 11 24 PM" src="https://github.com/user-attachments/assets/9de55450-7d1f-4e6b-8864-6f0fae44bc5d">
</p>
<p>Create a folder on the C drive called PHP</p>
<br />
<p><img width="1710" alt="Screenshot 2024-11-04 at 3 58 06 PM" src="https://github.com/user-attachments/assets/8e292f8d-cebc-46c9-9aab-e9655aadd426"></p>
<p>Install Microsoft Visual C++ Redistrubutable.</p>
<br />
<p><img width="1710" alt="Screenshot 2024-11-04 at 4 01 47 PM" src="https://github.com/user-attachments/assets/005f6fee-939a-4435-b961-d26a7aeb8fb3">
</p>
<p>Install MySQL. Use the typical install option. Make sure to launch the MySQL Instance Configuration Wizard at the end.</p>
<br />
<p><img width="1710" alt="Screenshot 2024-11-05 at 12 14 46 PM" src="https://github.com/user-attachments/assets/ba6ed502-4c32-46de-a9e1-f253352e6760"></p>
<p>When setting up your server create a Standard Configuration.</p>
<br />
<p><img width="1710" alt="Screenshot 2024-11-05 at 12 34 33 PM" src="https://github.com/user-attachments/assets/42dc5619-70f0-4f26-b7d5-c7bc9d198d60"></p>
<p>Run IIS as an administrator. </p>
<br />
<p><img width="1710" alt="Screenshot 2024-11-05 at 12 55 31 PM" src="https://github.com/user-attachments/assets/c188c212-9a76-4fb6-9a8c-6eacfce5772e"></p>
<p>Next we will register PHP from IIS Manager. After you click register you will navigate to where you saved PHP on your harddrive. Make sure to reload IIS when done. </p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 4 10 21 PM" src="https://github.com/user-attachments/assets/42d94c7e-43e7-4768-83f8-9b60ed15322c">
</p>
<p>Extract the osTicket installation folder and copy the upload folder into "c:\inet\wwwroot" folder.</p>
<br />
<p><img width="1710" alt="Screenshot 2024-11-05 at 4 01 55 PM" src="https://github.com/user-attachments/assets/90d81fbd-3862-4dd9-95f9-6edb4f782c19"></p>
<p>Restart the IIS server when extraction is complete.</p>
<br />
<p>
<img width="1710" alt="Screenshot 2024-11-05 at 4 12 37 PM" src="https://github.com/user-attachments/assets/db08d556-74d1-407a-9c52-6c7f226aef53">  
</p>
<p>Rename upload folder osTicket after it is moved.</p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 4 14 45 PM" src="https://github.com/user-attachments/assets/9b8d4d4f-1fa3-4f66-a0f2-3c2208acd325">
</p>
<p>Navigate to the osTicket folder within IIS. Once there click browse *.80(http) on the right hand side.</p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 4 17 32 PM" src="https://github.com/user-attachments/assets/5aebeed2-5077-420a-9dbe-be0bf2030d17">
</p>
<p>This will load the osTicket installation page in your default web browser. Before we install we need to fix some of the features. </p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 4 24 37 PM" src="https://github.com/user-attachments/assets/ad2fa499-df18-4836-b2dc-e02a7eb2420d">
</p>
<p>Go back to IIS. Double click the PHP Manager icon within the osTicket folder. Then click the enable or disable an extension. </p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 4 35 27 PM" src="https://github.com/user-attachments/assets/9a017eda-b955-43a6-b118-871190917a2b">
</p>
<p>Enable the following extensions php_imap.dll, php_intl.dll, php_opache.dll . After enabling these restart your server. </p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 4 40 38 PM" src="https://github.com/user-attachments/assets/52e231cf-6c5b-4b5c-b861-5d868135b17b">
</p>
<p>Refresh the browser that had the osTicket installation page. Make sure you have all green check marks except for the last two. Those aren't necessary for this installation. </p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 4 48 34 PM" src="https://github.com/user-attachments/assets/dd987c37-f08b-4047-a2f1-df1c0a89529a">
</p>
<p>Open the osTicket folder on your computer. Navigate to the include folder. Locate the file ost-sampleconfig.php. Rename this file ost-config.php</p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 5 01 33 PM" src="https://github.com/user-attachments/assets/71806d11-3971-4a8f-972b-ad437cb041a3">
</p>
<p>
  Edit the permissions of this file. Right click then go to properties. Click the security tab then advanced button. Disable inheritance first. Then remove all permissions. 
</p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 5 33 44 PM" src="https://github.com/user-attachments/assets/5d15f86f-ee52-444d-845d-94b6d0da70f7">
</p>
<p>
  Add permission to Everyone as the principal. 
</p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 5 38 07 PM" src="https://github.com/user-attachments/assets/af475566-eeb7-42d4-915c-b3acc5f83aaa">
</p>
<p>
  Give full control to everyone. Click ok. Click Apply then ok.
</p>
<br />
<p>
<img width="1710" alt="Screenshot 2024-11-05 at 5 48 28 PM" src="https://github.com/user-attachments/assets/0c36eb57-b5b8-4277-828b-37fed1174dae">
</p>
<p>
  Return to the installation screen in your web browser. Fill in the first half of the setup page. Make sure the admin e-mail and the default email are two different e-mail addresses. 
</p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 5 55 33 PM" src="https://github.com/user-attachments/assets/d5ccc3a6-906e-4211-940f-ebfd797b0e7e">
</p>
<p>Next we will install HeidiSQL. Install with all the default settings. Make sure to launch HeidiSQL when the install is finished. </p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 6 01 11 PM" src="https://github.com/user-attachments/assets/d0af935f-8639-4870-9790-04ece8cd0590">
</p>
<p>Connect to the SQL server we created in a previous step. </p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 6 03 08 PM" src="https://github.com/user-attachments/assets/4eddee7b-a8b1-47a2-9829-90ed02d3011e">
</p>
<p>
  Create a new database called osTicket. 
</p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 6 08 36 PM" src="https://github.com/user-attachments/assets/100ae81a-c376-4a86-9d90-cb54efeff8ba">
</p>
<p>Fill in the information from the osTicket database that you just created on the installation page. Press Install Now.</p>
<br />
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 6 11 52 PM" src="https://github.com/user-attachments/assets/751b4438-b89d-4c87-8ee7-dcba88e8bbed">
</p>
<p>The installation should be complete and succesful now. </p>
<br />
<p>Admin/Analyst Login Page:</p>
<p><a href="http://localhost/osTicket/scp/login.php">http://localhost/osTicket/scp/login.php</a> </p>
<br />
<p>End Users osTicket URL:</p>
<p><a href="http://localhost/osTicket">http://localhost/osTicket</a> </p>
