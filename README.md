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
Next we will be setting up ticket settings to allow anyone to create a ticket with out restrictions. To do this stay in the admin panel
and click the settings tab at the top and then click users. Once on the page simply check "require registration and login to create tickets" 
and then save changes.
</p>

___

<p>
<img src="https://i.imgur.com/8P2bUny.png" height="80%" width="80%" alt="Configure Agents"/>
</p>
<p>
Next we will be cconfiguring two new agents in osTicket. These agents can be added to different deparments and teams and they can also be assigned
tickets as well. To create new agents, stay in the admin panel and click the agents tab at the top and then click add new agent. You can give your 
new agent whatever new name and email address that you would like. Also you will need to give you agent a username and then click set password to assign
a password. On the password page uncheck "send the agent a password reset email" and also uncheck "require password change at next login". Enter in your password and then click set. Then click over to the access tab and you can assign your new agent to a department and give them a specific role. Then next in the teams tab you can assign them to one of the new teams that you created earlier. Once you are done hit create and then repeat the same process to create a second agent.
</p>

___

<p>
<img src="https://i.imgur.com/tsaje8m.png" height="80%" width="80%" alt="Adding Users"/>
</p>
<p>
Now that we have added some agents, it is time to add two users. Users will be the ones to send tickets to the agents that need to be 
resolved. We have spent most of our time in the admin panel for this tutorial but we will need to switch over to the agent panel in order
to create the users. One in the agent panel click the users tab at the top and then click add user. Once in the window add an the user email 
address and full name. You can also create a fake phone number and add internal notes it you would like and then click the add user button.
Repeat this process again to create the second user.
</p>

___

<p>
<img src="https://i.imgur.com/5x0yFb9.png" height="80%" width="80%" alt="Configuring SLA"/>
</p>
<p>
Now that the users have been created we will move to configuring three service level agreements in osTicket. To do this, switch over
to the admin panel and click the manage tab at the top. Then below the manage tab click SLA and then select "Add new SLA Plan". The first 
SLA Plan that we would want to add would be SEV-A, with a grace period of 1 hour and a schedule of 24/7. The grace period is how fast that the issue would need to be responded to (esstentially within one hour) and the schedule defines whether this would need to be addressed during business hours 
or on the weekend. Sev-A would be for severe incidents like an huge business outage. Click "add plan" once you are done. Next add SEV-B, with a grace period of 4 hours and a schdule of 24/7. This SLA  would be for medium level incidents like a department having issues with accessing microsoft powerpoint or microsoft word. Then lastly you would add a new plan called SEV-C, with a grace period of 8 hours and schedule of Monday through Friday business hours. This SLA would be for minor issues like your password needing to be reset. 
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

