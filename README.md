<h1>Windows11 User Login Startup Injection for Persistent Connection</h1>

<h2>Description</h2>
<br />In this lab, I will exploit a misconfigured startup folder to gain privileged access and persistence on the target machine. First things first, I will create an exploit.exe file then share it to stablish a connection with the the victim machine then I will run the Metasploit for the further configuration, after that i will bypass the UAC of the Windows 11 to gain access as the root user, then i will create a payload and upload it into the C drive Startup folder, it means whenever the Windows start itself again, i have a connection on it and at the end testing the lab.<br />

<br />The Startup folder of the Windows contains a list of application shortcuts that are executed, when the Windows machine is booted. Injecting a program into the Startup folder causes the program to run when a user logins and help you to maintain presistence or escalate privileges using the misconfigured startup. 
<br />


<h2>Environments Used </h2>

- <b>Parrot Operating System</b> 
- <b>Windows 11</b>

<h2>Lab walk-through:</h2>
Step Nr.1 : Creating exploit.exe, assigning IP and Local host of my computer to exploit, share it through the path with the victim machine and running Metasploit to stablish the connection. 
<p align="center">
Creaing,Share,Assign,Stablish: <br/>
<img src="https://i.imgur.com/bzMOtoZ.png" height="80%" width="80%" alt="Lab Step Nr.1"/>
<img src="https://i.imgur.com/A9qLzsn.png" height="80%" width="80%" alt="Lab Step Nr.1"/>
<br />




</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
