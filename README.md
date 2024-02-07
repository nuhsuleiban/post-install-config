<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)


<h2>Tutorial Steps


Step 1: Configure Roles


First, we are going to create a "Supreme Admin" role, and give this role full access. To do this from the Admin Panel we are going to "Agents", then "Roles", and "Add New Role". Enter the name "Supreme Admin". In Permissions, you are given different areas that you can assign permissions to this role. For this role we are going to check every permission, making this a role that can essentially do everything.

<img width="1312" alt="image" src="https://github.com/nuhsuleiban/post-install-config/assets/153963865/36673611-3146-4ca5-b460-59d32c95449e">
 
Step 2: Configure Departments


Next, we will create a department in the Admin Panel. Navigate to "Agents", "Departments", and select "Add New Department". Name this department "System Administrators", and for this project we are going to leave all the default settings and simply click "Create Department".

<img width="1312" alt="image" src="https://github.com/nuhsuleiban/post-install-config/assets/153963865/180743cc-8704-4f5b-9fce-927cb5f517c4">

Step 3: Configure Teams

Creating teams allows for multiple agents from different departments to collaborate together on a team. To make a team from the Admin Panel, navigate to "Agents", "Teams", and select "Add New Team". Call this team "Level II Support", and under the "Members" tab add yourself to the team.

<img width="1312" alt="image" src="https://github.com/nuhsuleiban/post-install-config/assets/153963865/bb90d52d-ec64-436c-8b70-4f49ecd3983c">

Step 4: Allow Anyone To Create Tickets

To do this in the Admin Panel, navigate to "Settings", "Users", "Settings", and uncheck "Require registration and login to create tickets".

<img width="1312" alt="image" src="https://github.com/nuhsuleiban/post-install-config/assets/153963865/1493f452-6266-4193-8170-8ab27e4ccbea">

Step 5: Configure Agents

Now we will create some agents, which are the help desk professionals who check and resolve tickets. In the Admin Panel, under "Agents", click "Add New Agent". The first agent will be named "Jane Doe" with an email of "jane.doe@osticket.com" and username "jane.doe". Make sure to note Jane's username for later. Click "Set Password", uncheck "Send the agent a password reset email", and enter a password for Jane. Once again, make note of this password for later. Uncheck "Require password change at next login", and click "Set". On the other tabs, this is where we can set Jane's permissions, add her to a team, and her department. Under "Access" We will put Jane in the "System Administrators" department as a "Supreme Admin". In "Teams" we will add her to "Level II Support", and then click "Create". Follow Step 5 to create a second agent with the name "John Doe". Set his department as "Support" and "View only". Now you should be able to see Jane and John under "Agents" with their departments listed.

<img width="1312" alt="image" src="https://github.com/nuhsuleiban/post-install-config/assets/153963865/0fd1d7de-f2af-4c7d-92ec-f92d17497c0a">

Step 6: Configure Users


Next, we will configure the users, who simply put, are the people opening tickets. To add users, switch to the "Agent Panel". Under "Users", click "Create New User". Name the first user "Karen Karen" with an email of "Karen@osticket.com", and "Add User". We will now add one more user. Following the same steps with the name Ken.

<img width="1312" alt="image" src="https://github.com/nuhsuleiban/post-install-config/assets/153963865/6b48e654-de87-4658-a237-f021e63d7270">

Step 7: Configure SLAs

The purpose for the Service Level Agreement is to prioritize requests and also provide a length of time in which the help desk administrator expects the tickets to be resolved. So we will do this next. Go back to the "Admin Panel" and navigate to "Manage", and "SLA" where we will create 3 SLA plans. Click "Add New SLA Plan", naming it "SEV A", a grace period of "1" (hours), and schedule of "24/7". This means that at any time a ticket comes in, it has to be resolved in 1 hour. Next make two more SLAs, one called "SEV B", a grace period of "4" (hours), schedule of "24/7", and finally "SEV C", grace period of "8" (hours), schedule "Monday-Friday".

<img width="1312" alt="image" src="https://github.com/nuhsuleiban/post-install-config/assets/153963865/3372913c-55d6-4eff-8caf-bc819de4a514">

Step 8: Configure Help Topics

Help topics help streamline tickets assignments for users, so we will configure a few now. In the Admin Panel, navigate to "Manage", "Help Topics", and click "Add New Help Topic". We will create the following 4 help topics: "Business Critical Outage", "Personal Computer Issues", "Equipment Request", and "Password Reset".

<img width="1312" alt="image" src="https://github.com/nuhsuleiban/post-install-config/assets/153963865/4e8d0587-c347-49ff-9472-b8b2446d781e">


That completes the set up and configuration of osTicket!

