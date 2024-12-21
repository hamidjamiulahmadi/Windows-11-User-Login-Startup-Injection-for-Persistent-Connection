<h1>Windows11 User Login Startup Injection for Persistent Connection</h1>

<h2>Description</h2>
<br />In this lab, I will exploit a misconfigured startup folder to gain privileged access and to mantain a persistence connection with the target machine. First things first, I will create an exploit.exe file then share it to stablish a connection with the the victim machine then I will run the Metasploit for the further configuration, after that i will bypass the UAC of the Windows 11 to gain access as the root user, then i will create a payload and upload it into the C drive Startup folder, it means whenever the Windows start itself again, i have a connection on it and at the end testing the lab.<br />

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
 Step Nr.2 : Victim machine got the file and the connection will be stablish.
<p align="center">
Victim machine got the file: <br/>
<img src="https://i.imgur.com/oGqYrNa.png" height="80%" width="80%" alt="Lab Step Nr.2"/>
<br />
 Step Nr.3 : after stablishing connection, i have the normal user priviledge access, next step i will bypass the UAC of the windows 11 machine to become the root user.
<p align="center">
Bypassing UAC, gain root user: <br/>
<img src="https://i.imgur.com/IzGTADR.png" height="80%" width="80%" alt="Lab Step Nr.3"/>
<img src="https://i.imgur.com/ObSnuCe.png" height="80%" width="80%" alt="Lab Step Nr.3"/>
<br />
Step Nr.4 : As you see i bypassed the UAC and now i am the root user, now i will create a payload and then upload it into the startup folder of the windwos11 machine C drive that whenever the user loged in agian to the machine, the startup folder run automaticlly with Windows and i have a connection with the target machine.
<p align="center">
Creating payload, upload to C drive: <br/>
<img src="https://i.imgur.com/uf9axAq.png" height="80%" width="80%" alt="Lab Step Nr.4"/>
<img src="https://i.imgur.com/93C5toe.png" height="80%" width="80%" alt="Lab Step Nr.4"/>
<br />
Step Nr.5 : We see that the payload is successfully uploaded to the C drive start up, it means whenever the windows start itself again I have a connection on it, then I will open another terminal and run the Metasploit on the following port that I assign it before to see the lab accomplishment and you see down here that i have a connection on the Windows 11 machine and the lab successfully completed.
<p align="center">
Windows 11 rebooted, Connection stablished agian: <br/>
<img src="https://i.imgur.com/hvHxK2t.png" height="80%" width="80%" alt="Lab Step Nr.5"/>
<img src="https://i.imgur.com/xOVFdV0.png" height="80%" width="80%" alt="Lab Step Nr.5"/>
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
