<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<!--<h2>Video Demonstration</h2>-->

<!-- - ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)-->

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create a virtual machine running Windows 10.
- Login to the virtual machine and enable Internet Information Services with CGI enabled. 
- Item 3
- Item 4
- Item 5

<h2>Installation Steps</h2>

<p>
<img src="https://github.com/user-attachments/assets/7950d93a-a843-4a2e-ac79-d3e728807aa8" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Create a virtual machine running Windows 10. The virtual machine should be have at least 2 CPUs and 16 GiB of memory. 
</p>
<p><img width="1710" alt="Screenshot 2024-11-04 at 11 37 46 AM" src="https://github.com/user-attachments/assets/82a2239f-f989-4c48-b72c-eef9b149a2b0"></p>
<p>Log into the virtual machine. </p>

<p><img width="1710" alt="Screenshot 2024-11-04 at 1 37 27 PM" src="https://github.com/user-attachments/assets/05d636eb-06bc-4b16-afbb-e168f25279ee"></p>
<p>Open the control panel and enable internet information services. Also enable CGI. To get to this click World Wide Web Services folder then click Application Development Features. Check the CGI folder. Then press ok. </p>

<p><img width="1710" alt="Screenshot 2024-11-04 at 11 33 15 AM" src="https://github.com/user-attachments/assets/4e6c7b7d-c7b5-47fc-bde9-a8c77f61aa1a">
</p>
<p>
Install PHP Manager for IIS. </p>
<p><img width="1710" alt="Screenshot 2024-11-04 at 2 58 52 PM" src="https://github.com/user-attachments/assets/7b06832c-e39e-4227-9434-6389bc90e499"></p>
<p>Install Rewrite Module</p>
<p><img width="1710" alt="Screenshot 2024-11-04 at 3 11 24 PM" src="https://github.com/user-attachments/assets/9de55450-7d1f-4e6b-8864-6f0fae44bc5d">
</p>
<p>Create a folder on the C drive called PHP</p>
<p><img width="1710" alt="Screenshot 2024-11-04 at 3 58 06 PM" src="https://github.com/user-attachments/assets/8e292f8d-cebc-46c9-9aab-e9655aadd426"></p>
<p>Install Microsoft Visual C++ Redistrubutable.</p>
<p><img width="1710" alt="Screenshot 2024-11-04 at 4 01 47 PM" src="https://github.com/user-attachments/assets/005f6fee-939a-4435-b961-d26a7aeb8fb3">
</p>
<p>Install MySQL. Use the typical install option. Make sure to launch the MySQL Instance Configuration Wizard at the end.</p>
<p><img width="1710" alt="Screenshot 2024-11-05 at 12 14 46 PM" src="https://github.com/user-attachments/assets/ba6ed502-4c32-46de-a9e1-f253352e6760"></p>
<p>When setting up your server create a Standard Configuration.</p>
<p><img width="1710" alt="Screenshot 2024-11-05 at 12 34 33 PM" src="https://github.com/user-attachments/assets/42dc5619-70f0-4f26-b7d5-c7bc9d198d60"></p>
<p>Run IIS as an administrator. </p>
<p><img width="1710" alt="Screenshot 2024-11-05 at 12 55 31 PM" src="https://github.com/user-attachments/assets/c188c212-9a76-4fb6-9a8c-6eacfce5772e"></p>
<p>Next we will register PHP from IIS Manager. After you click register you will navigate to where you saved PHP on your harddrive. Make sure to reload IIS when done. </p>
<p>
  <img width="1710" alt="Screenshot 2024-11-05 at 4 10 21 PM" src="https://github.com/user-attachments/assets/42d94c7e-43e7-4768-83f8-9b60ed15322c">
</p>
<p>Extract the osTicket installation folder and copy the upload folder into "c:\inet\wwwroot" folder.</p>
<p><img width="1710" alt="Screenshot 2024-11-05 at 4 01 55 PM" src="https://github.com/user-attachments/assets/90d81fbd-3862-4dd9-95f9-6edb4f782c19"></p>
<p>Restart the IIS server when extraction is complete.</p>
<p>
<img width="1710" alt="Screenshot 2024-11-05 at 4 12 37 PM" src="https://github.com/user-attachments/assets/db08d556-74d1-407a-9c52-6c7f226aef53">  
</p>
<p>Rename upload folder osTicket after it is moved.</p>



<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>

<br />
