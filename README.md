<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Create different role for agents ( ex: Supreme Admin, Admin)
- Create different departments in osTicket ( ex: Accounting, System Administrators)
- Setup different support level teams ( ex: Level 2 Support, Level 3 Support)
- Configure permissions for ticket creation by customers
- Configure different agents/workers 
- Configure different users/customers
- Setup SLA ( Service Level Agreements)
- Configure Help Topics ( ex: Business Critical Outage, Password Reset, etc)

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/thvxoMH.png" height="80%" width="80%" alt="Setting Up Roles"/>
</p>
<p>
If you followed my previous tutorial for installing osTicket, you should now have fully installed osTicket with all of the necessary
prerequistes and with a username and password to access your admin and agent panel. In this tutorial we will be configuring different 
aspects of osTicket so that we can simulate the typical ticket lifecycle found in IT in my next tutorial.  To starts things off we will
be configuring different roles in osTicket and to do this click your Admin Panel button at the top and then select the Agents tab in the 
upper second row and then select roles. Click Add New Role and create a new role name. I decided to create a role called Supreme Admin that
esstentially has all permissions granted but you can call your new role whatever you would like to. Once you name your new role, go over to 
the permissions tab and select what permisions you would like this particular role to have and then once you are done click add role at the
bottom to complete your new role. You can create as many new roles that as needed.
</p>

___

<p>
<img src="https://i.imgur.com/09LKDYq.png" height="80%" width="80%" alt="Adding New Departments"/>
</p>
<p>
Next we will be configuring different departments. Departments are pretty useful because you can assign specific agents to different departments and even assign specific SLA ( service level agreements) to certain departments.  To get to the departments page, stay in the admin panel and agents tab and simply click departments which should be next to the roles button. Then click add new department. Once on this page, add a department name ( example: System Administrators, DevOps, Cloud). Right now we don't have our SLAs set up yet so we can leave the SLA and Schedule lines on default. Once we configure that you can always come back and update the department information. You can also assign a manager and since there is only one agent created so far (yourself) you can assign it to your username. Once you are done, simply click the create department button at the bottom.
</p>

___

<p>
<img src="https://i.imgur.com/08AnFrn.png" height="80%" width="80%" alt="Configure Teams"/>
</p>
<p>
Next we will be creating different teams in osTicket. Teams can be used to seperate agents by support level or by tasks.
For example you can create a level 1 support team for lower priority tickets and a escalations team that handles higher priority tickets.
To configure a new team simply head to the Teams tab that is next to the roles tab. Once on the teams page click add new team and give the 
new team a name. Then click members and assign yourself as a member of the newly created team and then press create team at the bottom.
</p>

___


<p>
<img src="https://i.imgur.com/wLrxl1c.png" height="80%" width="80%" alt="Setting up user permissions"/>
</p>
<p>
Ticket Permissions
</p>

___

<p>
<img src="https://i.imgur.com/8P2bUny.png" height="80%" width="80%" alt="Configure Agents"/>
</p>
<p>
Setup Agent Profiles
</p>

___

<p>
<img src="https://i.imgur.com/tsaje8m.png" height="80%" width="80%" alt="Adding Users"/>
</p>
<p>
Add Users
</p>

___

<p>
<img src="https://i.imgur.com/5x0yFb9.png" height="80%" width="80%" alt="Configuring SLA"/>
</p>
<p>
Configure SLA
</p>

___

<p>
<img src="https://i.imgur.com/KUcA4Nz.png" height="80%" width="80%" alt="Configure Help Topics"/>
</p>
<p>
Configure Help Topics 
</p>

___

<p>
<img src="https://i.imgur.com/ZMRmYeB.png" height="80%" width="80%" alt="Tutorial Complete"/>
</p>
<p>
Tutorial Complete
</p>

