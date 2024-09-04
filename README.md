<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<!---
# (<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com) -->

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Ensure osTicket runs in IIS
- Ensure MySQL database is created
- Ensure we can log in to the osTicket Admin panel
- Make any other osTicket configurations as appropriate

<h2>Configuration Steps</h2>


<p>1. Begin osTicket Configuration.  In Windows Explorer, browse to C:\inetpub\wwwroot\osTicket\include\ and look for ost-sampleconfig.php, and rename this file to ost-config.php:</p>
<img src="https://github.com/user-attachments/assets/c4909882-3676-4fc1-baad-51f3e9babfa8" alt="Browse to our ost-sampleconfig.php file" />
<img src="https://github.com/user-attachments/assets/eac577d5-61e6-4989-84da-b35bed03a802" alt="And rename it to ost-config.php" />
<br /><br />

<p>2. Temporarily reassign security permissions to "Everyone" with read and write access for ost-config.php:</p>
<img src="https://github.com/user-attachments/assets/1eb5c203-c11f-494a-a2e0-adadb3abf5de" alt="RW permissions to ost-config.php" />
<br /><br />

<p>3. Install HeidiSQL, which is our MySQL database client that allows sending SQL commands to MySQL</p>
<img src="https://github.com/user-attachments/assets/731e738c-ede6-4bc8-babd-5da016766f41" alt="Done HeidiSQL" />
<img src="https://github.com/user-attachments/assets/24e5ce7a-76ce-42ee-a2a2-74e1b54727fa" alt="Done HeidiSQL" />
<br /><br />

<p>4. Click New and connect to MySQL:</p>
<img src="https://github.com/user-attachments/assets/a86c6c76-a741-4349-b721-5e2b375691e6" alt="Connect to MySQL" />
<br /><br />

<p>5. Create a new MySQL database called "osTicket". All of our osTicket activities will be stored in this database:</p>
<img src="https://github.com/user-attachments/assets/f51257d1-31b6-4ff1-a728-e28db337c671" alt="Create a database called osTicket" />
<br /><br />

<p>6. Continue our osTicket installation and configuration. At the previous "Thank You" page at the bottom is a "Continue" button. Complete the fields as appropriate</p>
<img src="https://github.com/user-attachments/assets/a0b14417-6334-48ce-8933-f2fc054eca94" alt="Thank You page with Continue button" />
<img src="https://github.com/user-attachments/assets/43b340d3-1645-4607-8a5f-413a693bee8c" alt="osTicket Begin Installation page" />
<br /><br />

<p>7. Once done, we will have this Congratulations page. Note our links to the Admin and Agent portals:</p>
<img src="https://github.com/user-attachments/assets/63d9b66e-3a91-4427-aca3-ceb7d1fb1081" alt="Congratulations on installing osTicket" />
<br /><br />

<p>8. Go back to our ost-config.php in Windows Explorer, and change the permissions to Read only:</p>
<img src="https://github.com/user-attachments/assets/12c0ad5f-2a55-466b-91d9-8dc897006086" alt="Read only for ost-config.php" />
<br /><br />

<p>9. In a browser window, go to the link for our Admin portal:</p>
<img src="https://github.com/user-attachments/assets/a5eae3d9-f401-463c-8af8-6be92817faf3" alt="Going to our Admin portal" />
<img src="https://github.com/user-attachments/assets/42889592-cc3c-4579-97be-4aa173af4153" alt="Going to our Admin portal" />
<br /><br />

<p>10. We can then make any other configurations as appropriate.</p>
- Creating a "Super Admin" role:
<img src="https://github.com/user-attachments/assets/53dec451-25d6-4094-83d6-ae0865360a4d" alt="Super Admin Role" />
- Creating a "System Administrators" Department:
<img src="https://github.com/user-attachments/assets/005d0884-5df1-4f37-b8f7-7b9b6a162e17" alt="System Administrators Department" />
- Creating a "Level II Support" team:
<img src="https://github.com/user-attachments/assets/a0f299d2-445e-4d35-bf2f-ed6a9b20a5c2" alt="Level II Support Team" />
- Creating additional users in osTicket:
<img src="https://github.com/user-attachments/assets/82d360e2-98e2-4414-ba93-c92520db9892" alt="Creating Users" />
- Creating custom Service Level Agreement options:
<img src="https://github.com/user-attachments/assets/50baa259-e63b-47cc-a8f3-9bd2f7f4030d" alt="Creating SLAs" />
- Creating a new Help Topic:
<img src="https://github.com/user-attachments/assets/f565bd61-b863-4d9c-82ac-6ec249f17f68" alt="Adding Help Topic" />
