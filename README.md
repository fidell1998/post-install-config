<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket. This specific guide is designed for a broad audience, from non-technical users to IT professionals, making it accessible regardless of your technical background.
<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- **Windows 10** used for installing and configuring osTicket

A Windows 10 virtual machine was created using **Microsoft Azure**, with **macOS** as the host system.

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure Users
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<h3>Admin and Agent Panel</h3>

After logging into your **osTicket** installation as an administrator, you’ll notice two main interfaces: the **Agent Panel** and the **Admin Panel**.

If you're currently in the **Agent Panel**, you’ll see a button labeled **"Admin Panel"** in the top-right corner. This confirms your current view is the Agent Panel — the area where support tickets are created, viewed, and managed.

Click on **"Admin Panel"** to switch to the administrative interface. This is where we’ll perform backend configurations for our **Superhero Company**.
  
<img width="1916" height="1007" alt="1" src="https://github.com/user-attachments/assets/d1bec9d6-759c-47a9-8cab-c57e007d06af" />

Now we're in the **Admin Panel**. You can confirm this by checking the top-right corner — it will display a button labeled **"Agent Panel"**, indicating that you're currently in the admin interface.

Next, click on the **"Agent Panel"** button to switch back to the agent interface. Once you're there, navigate to the **"Agents"** tab in the top navigation bar, and then select **"Roles"** from the dropdown menu.

This is where we’ll manage user roles and permissions for agents within our **Superhero Company**.

<img width="1917" height="968" alt="2" src="https://github.com/user-attachments/assets/b75c2c13-f53e-49bf-8411-e4b06a83c7db" />

<br />

<h3>Configure Roles</h3>

In osTicket, a **Role** defines what an agent can and cannot access within the system. Each role comes with a specific set of permissions that control what actions agents are allowed to perform — such as viewing tickets, editing them, managing users, and accessing admin settings.

For example, a support agent might only have access to view and reply to tickets, while a manager might have broader permissions to assign tickets and view reports.

<img width="1917" height="462" alt="3" src="https://github.com/user-attachments/assets/c9417b4b-59e2-4aab-8c71-c4dac34b068a" />

Below is an example of a role with expanded access:

<img width="977" height="742" alt="4" src="https://github.com/user-attachments/assets/a5497f6d-2d08-4548-8b42-f442ccba1d49" />

You can also create custom roles by clicking **"Add New Role"**. This allows you to define a new access group tailored to specific responsibilities within your **Company**.

This is a powerful way to manage your team by giving each agent the right level of access based on their job.

<br>

<h3> Configure Departments </h3>


