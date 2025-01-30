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

- Configure Roles and Departments 
- Configure Teams and allow anyone to create a ticket
- Configure Agents (workers) and Users (customers)
- Settting Up Service Level Agreements and Creating Help Topics

<h2>Configuration Steps</h2>

<p align="center">
First login into the osTicket. 
</p>
<p>
<img width="1512" alt="Login SC" src="https://github.com/user-attachments/assets/6ca6af23-2020-4d9c-80fb-da20c4d32a97" />
</p>
<br />

<p align="center">
STEP 1 : 
In osTicket, I created a "Super Admin" role by navigating to Admin Panel > Agents > Roles and adding a new role. This Super Admin role was configured with full access permissions to all parts of the ticketing system, allowing comprehensive control and management capabilities. The primary purpose of creating this role was to group high-level permissions together, enabling efficient administration and oversight of the entire osTicket platform.
</p>
<p>
<img width="1512" alt="Roles SC" src="https://github.com/user-attachments/assets/b166b6c6-eca3-40a0-87f7-2549f478b210" />
<img width="1512" alt="Adding a Role SC" src="https://github.com/user-attachments/assets/65053979-1ef3-429e-8a7b-a12df7e72fb5" />
</p>
<br />

<p align="center">
In the osTicket system, I created a dedicated SysAdmin department to efficiently categorize and route technical support tickets related to system administration tasks. By configuring the department in the Admin Panel under Agents > Departments, I established a strategic method to control ticket access and visibility, ensuring that only authorized personnel can view and manage specific system-related issues. This approach improves workflow efficiency, enhances security, and provides a clear organizational structure for handling complex IT support requests.
</p>
<p>
<img width="1512" alt="Creating new department " src="https://github.com/user-attachments/assets/9aa9e4a8-10d3-43bd-9583-c393f27f51a6" />

<img width="1512" alt="Dept Name " src="https://github.com/user-attachments/assets/e45b78f8-1f30-4cae-9bb4-6c310b250825" />
</p>
<br />

<p align="center">
STEP 2 : In osTicket, I created a new team in the Admin Panel under Agents > Teams, which enables cross-departmental collaboration by allowing agents from different departments to work together on specific tickets. Teams provide a flexible mechanism for grouping agents who may not be in the same department but need to collaborate on resolving complex support issues or specialized tasks. By configuring teams, organizations can enhance ticket management efficiency, ensure comprehensive problem-solving, and create a more adaptable support workflow that transcends traditional departmental boundaries. The team I created was online banking. 
</p>
<p>
<img width="1512" alt="Screenshot 2025-01-16 at 2 12 00 PM" src="https://github.com/user-attachments/assets/d42e5647-7b84-454b-9eae-7c1103d6b1e6" />
  <img width="1512" alt="Screenshot 2025-01-16 at 2 13 26 PM" src="https://github.com/user-attachments/assets/ff3aafcf-6513-4d2c-9bc9-3bc1ef0157e3" />

</p>
<br />

<p align="center">
In osTicket, we enhanced accessibility by configuring user settings to allow ticket creation without mandatory registration. By navigating to User Settings and unchecking "Registration Required: Require registration and login to create tickets," we enabled a more user-friendly experience for customers seeking support. This open ticketing approach is considered best practice as it reduces barriers to entry, potentially increasing user engagement and satisfaction, while still maintaining the option for registered users to track their tickets more efficiently.
</p>
<p>
<img width="1512" alt="Screenshot 2025-01-16 at 2 22 50 PM" src="https://github.com/user-attachments/assets/96b15557-e678-4f03-957b-1730bf3add0a" />
</p>
<br />




<p align="center">
STEP 3 :  In osTicket, we configured agents by creating new user accounts and strategically assigning them to specific departments. We navigated to the Admin Panel > Agents > Add New Agent, where we set up two distinct agents: one assigned to the SysAdmins department and another to the Support department. This departmental assignment is crucial for efficient ticket routing and management, ensuring that each agent has access to relevant tickets and can provide specialized support within their area of expertise.
</p>
<p>

<img width="1512" alt="Screenshot 2025-01-16 at 2 28 18 PM" src="https://github.com/user-attachments/assets/1d198590-080d-424f-a289-afa8226d1ef1" />

<img width="1512" alt="Screenshot 2025-01-16 at 2 51 30 PM" src="https://github.com/user-attachments/assets/15ec5a6d-f6cd-424c-a437-600c0d48ba57" />


</p>
<br />





<p align="center">
  In osTicket, configuring users (customers) is a critical step in establishing an effective support system. To add new customers, we navigate to the Agent Panel, select the Users tab, and click on "Add New User," where we input essential customer information. This process is vital for maintaining an organized database of support requesters, enabling personalized ticket tracking, and facilitating efficient communication between support staff and customers throughout the ticket lifecycle.
</p>
<p>
<img width="1512" alt="Screenshot 2025-01-16 at 4 49 05 PM" src="https://github.com/user-attachments/assets/0941f822-63ee-49c8-9284-16da7c0f6421" />
</p>
<br />





<p align="center">
STEP 4 : Setting up Service Level Agreements (SLAs) in osTicket is a crucial step in defining and managing support priorities. SLAs are typically associated with severity levels, which are determined by the organization based on business impact, ensuring that critical issues receive appropriate attention and resources. By configuring SLAs, support teams can effectively prioritize tickets, meet response time commitments, and align their efforts with the organization's operational needs, ultimately enhancing customer satisfaction and maintaining service quality standards. 
</p>
<p>
 <img width="1512" alt="Screenshot 2025-01-16 at 5 09 28 PM" src="https://github.com/user-attachments/assets/b7be8e8a-bc04-4f25-b5c1-7f09ebec38b0" />
  <img width="1512" alt="Screenshot 2025-01-16 at 5 15 40 PM" src="https://github.com/user-attachments/assets/eed77f80-0915-4928-896b-fad4aeea9e4a" />

</p>
<br />


<p align="center">
Creating Help Topics in osTicket streamlines the ticket submission process by providing users with pre-defined categories for their issues or requests. This feature directs tickets to the appropriate department automatically, reducing manual sorting and improving response times. By implementing Help Topics, organizations can efficiently manage ticket flow, ensure proper assignment to specialized teams, and gather valuable data on common issues, ultimately enhancing the overall support experience and operational efficiency.
</p>
<p>
   <img width="1512" alt="Screenshot 2025-01-16 at 5 29 25 PM" src="https://github.com/user-attachments/assets/d9a3a81a-1307-461f-ab27-d6c4fee47a0d" />
</p>
<br />
















