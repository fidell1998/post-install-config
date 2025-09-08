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

Click on **"Admin Panel"** to switch to the administrative interface. This is where we’ll perform backend configurations for our **Company**.
  
<img width="1916" height="1007" alt="1" src="https://github.com/user-attachments/assets/d1bec9d6-759c-47a9-8cab-c57e007d06af" />

Now we're in the **Admin Panel**. You can confirm this by checking the top-right corner — it will display a button labeled **"Agent Panel"**, indicating that you're currently in the admin interface.

Next, click on the **"Agent Panel"** button to switch back to the agent interface. Once you're there, navigate to the **"Agents"** tab in the top navigation bar, and then select **"Roles"** from the dropdown menu.

This is where we’ll manage user roles and permissions for agents within our **Company**.

<img width="1917" height="968" alt="2" src="https://github.com/user-attachments/assets/b75c2c13-f53e-49bf-8411-e4b06a83c7db" />

<br />

<h3>Configure Roles</h3>

In osTicket, a **Role** defines what an agent can and cannot access within the system. Each role comes with a specific set of permissions that control what actions agents are allowed to perform — such as viewing tickets, editing them, managing users, and accessing admin settings.

For example, a support agent might only have access to view and reply to tickets, while a manager might have broader permissions to assign tickets and view reports.

<img width="1917" height="462" alt="3 10 29 02 AM" src="https://github.com/user-attachments/assets/f84b800e-ddd0-402b-8dd9-1dbd0d35ceb3" />

Below is an example of a role with expanded access:

<img width="977" height="742" alt="4" src="https://github.com/user-attachments/assets/a5497f6d-2d08-4548-8b42-f442ccba1d49" />

You can also create custom roles by clicking **"Add New Role"**. This allows you to define a new access group tailored to specific responsibilities within your **Company**.

This is a powerful way to manage your team by giving each agent the right level of access based on their job.

<br>

<h3> Configure Departments </h3>

Next, navigate to the **Departments** tab in the **Admin Panel**.

In osTicket, **Departments** are used to organize your support structure. Each department can represent a specific area of your company, such as **Technical Support**, **Billing**, **Customer Service**, or even teams like **Superhero Operations**.

Creating departments allows you to:

- Route tickets to the appropriate team.
- Assign department-specific agents.
- Set up custom auto-responses and SLA plans for each department.

To add a new department, click **“Add New Department”**

<img width="1004" height="385" alt="5" src="https://github.com/user-attachments/assets/81fb0778-e2c0-4014-a368-2b72b2e232a3" />

I will make a department called SysAdmins:

<img width="1001" height="925" alt="6" src="https://github.com/user-attachments/assets/e8090d16-7b1f-4871-9de0-33596cc41f34" />

<br>

<h3>Configure Teams</h3>

Now, let's navigate to the **Teams** section in the **Admin Panel**.

In osTicket, a **Team** is a group of agents within a department. Teams allow you to further organize your support staff by grouping agents who work on more specific tasks or areas.

For example, within a **Support Department**, you might have teams like **Online Banking**, **Technical Issues**, or **Account Recovery**.

To create a new team, click **“Add New Team”**.

<img width="1117" height="363" alt="7" src="https://github.com/user-attachments/assets/9bfc42a3-5570-41b4-b847-2837ea1b99b8" />

For this guide, we’ll create a team called **Online Banking**:

<img width="1067" height="743" alt="8" src="https://github.com/user-attachments/assets/8c024120-dfa6-4b27-bfa3-9e4d6e64d7a3" />

<br>

<h3>Configure Agents</h3>

Now let’s go to the **Agents** section in the **Admin Panel**.

This is where you create login accounts for your team members so they can access the system and work on tickets.

Click **“Add New Agent”** to begin setting up an account. In the **Account** tab, you can fill out basic information about the agent, such as name, email, username, and contact details.

<img width="1030" height="409" alt="9" src="https://github.com/user-attachments/assets/f47635f4-efa5-4879-8f05-abb10f21754f" />

When assigning a password, make sure to review the options carefully. Double-check what checkboxes are selected or not, this helps avoid any login or accessibility issues for the agent.

<img width="788" height="499" alt="11" src="https://github.com/user-attachments/assets/45a5e8dd-c2f9-4e3a-89ae-82715f5296fe" />

Next, assign the agent to a department. In this example, we're assigning the agent to the **SysAdmins** department.

<img width="1026" height="587" alt="12" src="https://github.com/user-attachments/assets/6568a0b9-5852-4335-aa15-8570f066ae5f" />

You can also assign the agent to a specific team. Here, we’re adding them to the **Online Banking** team.

<img width="1120" height="493" alt="13" src="https://github.com/user-attachments/assets/7a7d2a3c-537e-431c-873c-e43621a49fa8" />

For this guide, we created two agents: **Spider-Man** and **Wonder Woman**. Both are now active agents within the company, alongside the admin account.

<img width="1025" height="486" alt="14" src="https://github.com/user-attachments/assets/c47338bc-d7fd-470d-b085-c6f0309a54d5" />

<br>

<h3>Configure Users</h3>
