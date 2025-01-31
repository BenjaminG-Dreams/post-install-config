<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites</h1>
This tutorial is a continuation of the installation of osTicket which is linked below if you have not completed it yet.</p>

- [osTicket: Prerequisites and Installation](https://github.com/bvongpradith/osticket-prereqs)

<h2>Environments and Technologies Used in Tutorial</h2>

- Microsoft Azure
- Remote Desktop
- Internet Information Services (IIS)
- osTicket
- HeidiSQL

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Steps</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Download and install the Rewrite Module
- Allow anyone to create tickets
- Configure Agents (employees)
- Configure Users (customers)
- Configure SLAs
- Configure Help Topics

<h2>Detailed Steps</h2>

![Screenshot 2025-01-30 212659](https://github.com/user-attachments/assets/a1929ba1-2ebd-4078-b88f-3afc57ab6d8c)

<p>
We'll first go to the login (http://localhost/osTicket/scp/login.php) to login with the admin credentials from the previous tutorial.
</p>
<br />

![Screenshot 2025-01-30 212835](https://github.com/user-attachments/assets/6f14f8aa-075a-46ae-9b57-4e308977871f)

![Screenshot 2025-01-30 213656](https://github.com/user-attachments/assets/5c4f4ccc-78d4-491f-b000-13b2aff87d2e)

<p>
Next, click "Admin Panel" at the top right of the screen. The button will change to "Agent Panel" when you navigate inside the admin panel.Then go to Agents > Roles > Add New Role
</p>
<br />

![Screenshot 2025-01-30 213738](https://github.com/user-attachments/assets/b7de9fe1-c2f4-4d71-ba32-e6e5b0714d47)

![Screenshot 2025-01-30 213812](https://github.com/user-attachments/assets/89ecab9b-2795-49a5-9b46-96cb7df60b0f)


<p>
Now, name the role to "TopAdmin" and then allow all permissions in the next tab. Click "Add Role".
</p>
<br />

![Screenshot 2025-01-30 214117](https://github.com/user-attachments/assets/8ef81096-d4cb-4ed9-b5b5-e425edbf6e5f)



<p>
Navigate to "Departments" and then click "Add New Department".
</p>
<br />

![Screenshot 2025-01-30 214305](https://github.com/user-attachments/assets/8e3acc6d-86d6-4301-b277-19bf309622fd)

<p>
Name the department to "SysAdmins" and then press "Create Dept".
</p>
<br />

![Screenshot 2025-01-30 214416](https://github.com/user-attachments/assets/2b2baa95-a84d-41f7-9b84-391a9d2da44e)

![Screenshot 2025-01-30 214522](https://github.com/user-attachments/assets/c3971361-6c6f-4390-86df-a231b252530b)

<p>
Head to the "Teams" panel and click "Create New Team". Name the new team "Level II Support" and press create.
</p>
<br />

![Screenshot 2025-01-30 214839](https://github.com/user-attachments/assets/8d0dbb02-649f-4669-9511-fd3630434e4b)

<p>
Afterwards, go to "Settings" > Users > Make sure the box for registration requirement is not checked > make the method public > Save Changes.
</p>
<br />

![Screenshot 2025-01-30 214937](https://github.com/user-attachments/assets/3fa55c01-2e0a-4f81-ab67-6bd5841ee9a8)

<p>
Now go into the agents panel and add new agent.
</p>
<br />

![Screenshot 2025-01-30 215527](https://github.com/user-attachments/assets/d284188e-24d2-4c0e-a684-8a1287c1e5c9)

![Screenshot 2025-01-30 215810](https://github.com/user-attachments/assets/296a5f3a-9d36-4379-b4b9-4bd0485a3027)

![Screenshot 2025-01-30 215841](https://github.com/user-attachments/assets/e454e07c-c1f8-4d55-b58c-d443bbba2041)


<p>
Create these accounts:

- Name:	Jane Doe
- Email Address: jane.doe@osticket.com
- Username: jane.doe
- Set the password to "Password1"
- Go to Access and set the department to SysAdmins and select Supreme Admin for the role.
- Go to the teams section and select Level II Support, then create.

  ![Screenshot 2025-01-30 220210](https://github.com/user-attachments/assets/b319cd7c-fdae-417b-9725-0209d6d6bc87)

After, create a second account for " John Doe"
</p>
<br />

![Screenshot 2025-01-30 221237](https://github.com/user-attachments/assets/1df5cbb8-0a0d-4a5e-a9a8-4c56212931db)

<p>
Then go to Agent panel > Users > Add User
</p>
<br />

![Screenshot 2025-01-30 221429](https://github.com/user-attachments/assets/ae725d4f-c0c3-42bc-99ee-20c6a3e868cc)

<p>
 Add the following users:
- Email Address: Karen.k@gmail.com
- Full Name: Karen K
</p>
<br />

![Screenshot 2025-01-30 221634](https://github.com/user-attachments/assets/c47eb7b9-d792-40f5-92ca-cde0b38c20b2)

<p>
Head to Admin Panel > Manage > SLA > Add New SLA Plan.
</p>
<br />

![Screenshot 2025-01-30 221741](https://github.com/user-attachments/assets/d6985140-3927-4e76-bb20-41a21acc26da)

![Screenshot 2025-01-30 221827](https://github.com/user-attachments/assets/77ad1e5e-dcc4-40b3-9554-d86954f18a3b)

![Screenshot 2025-01-30 221936](https://github.com/user-attachments/assets/7d936eb5-ab2e-46c6-b1b5-3048433b8eeb)


<p>
Next, add the following SLAs
  
- SEV-A with a grace period of 1 hour, and a 24/7 schedule
- SEV-B with a grace period of 4 hours, and a 24/7 schedule
- SEV-C with a grace period of 8 hours, and a Mon-Fri business hours schedule
</p>
<br />

![Screenshot 2025-01-30 222023](https://github.com/user-attachments/assets/de3e82fe-c106-405a-ae67-7f3411df5890)
![Screenshot 2025-01-30 222132](https://github.com/user-attachments/assets/7ba96f59-2b89-43bc-8eac-000487935a97)

<p>
Now, navigate to "Help Topics" and add the following help topics:
  
- Business Critical Outage/ Report Problem
- Personal Computer Issues/ Report Problem
- Equipment Request/ General Inquiry
- Password Reset/ Report Problem
















