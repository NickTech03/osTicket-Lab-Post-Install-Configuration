<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket Lab: Post-Install-Configuration</h1>

<h2>Introdution</h2>
osTicket is an open-source help desk platform designed to centralize and streamline customer support requests by converting emails, phone calls, and web form submissions into organized, trackable tickets.

</p>

Ticketing systems help IT teams organize and manage support requests in one central place. Instead of tracking problems through emails, phone calls, or messages, every issue is recorded as a ticket that can be assigned, updated, and monitored.
This makes sure no requests are missed, allows urgent problems to be fixed first, and helps IT staff work more efficiently. Ticketing systems also keep a history of all support activity, which improves accountability, security, and overall service quality.

</p>

This is the **SECOND** part of a four-part osTicket lab. In this section, we go step by step through the post-installation and start configuring osTicket to simulate a real-world IT help desk environment after completing the first part (osTicket: Prerequisites, Installation, and Validation). This project includes creating roles, departments, and teams to organize support staff and manage ticket access. It also involves adding agents and users, setting up SLA plans to track response times, and creating help topics to categorize incoming requests. These configurations help build a structured and efficient support system that reflects how many organizations manage IT support operations.

</p>

- [osTicket: Prerequisites, Installation, and Validation](https://github.com/NickTech03/osTicket-Lab-Prerequisites-Installation-and-Validation)
- **osTicket: Post-Install Configuration**
- [osTicket: Ticket Lifecycle Workflow (Examples)](https://github.com/NickTech03/osTicket-Lab-Ticket-Lifecycle-Workflow-Examples)
- [osTicket: Using ChatGPT to Simulate Support Tickets](https://github.com/NickTech03/osTicket-Lab-Using-ChatGPT-to-Simulate-Support-Tickets) 

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines / Compute)
- Remote Desktop Protocol (RDP)
- Admin / Staff Control Panel (SCP): http://localhost/osTicket/scp/login.php (**From Part 1**)
- End User Portal: http://localhost/osTicket/ (**From Part 1**)

**Admin / Staff Control Panel (SCP):** This is the Staff Portal, where support agents log in to view, manage, assign, and resolve support tickets. It serves as the main workspace for IT staff to handle user requests and track ticket progress.

**End User Portal:** This is the public help desk portal where users can submit support tickets, view updates, and check the status of their existing requests.

<h2>Operating Systems Used </h2>

- Windows 11 Pro, version 25H2 - x64 Gen2

# Post-Install Configuration Steps/Walkthrough

---

## Step 1 - Acknowledge Admin Panel vs Agent Panel

First, we'll start by logging into the the osTicket web portal for admin / staff control panel using the link below.

 - http://localhost/osTicket/scp/login.php

You can login with the username and password that was made in the previous lab.

- Username: `adminuser`
- Password: `Password1`

<img src=https://github.com/NickTech03/osTicket-Lab-Post-Install-Configuration/blob/24a61cab15b4f74c3fa8fe3626db6dac3f34e19f/1.png>

Once logged into the portal the dashboard will look like this for the **Agent Panel**. This is were you configure settings on the back-end for osTicket.

<img src=https://github.com/NickTech03/osTicket-Lab-Post-Install-Configuration/blob/f2e60141b672ab3c1b5e322888f88132fac7f5f3/2.png>

Now, when you look at the top of the page. You can see the **Admin Panel** highlighted, click that.

<img src=https://github.com/NickTech03/osTicket-Lab-Post-Install-Configuration/blob/4d47e3b8f4ec1d3aec2e7c658561cde60260a40d/3.png>

This is the Admin Panel portal were it's used by Help Desk Agents and Support Specialists to view, manage, and resolve support tickets submitted by users.

<img src=https://github.com/NickTech03/osTicket-Lab-Post-Install-Configuration/blob/595a49393d443c0894953f211aeece6c0be33eb3/4.png>

**We will going through these panels frequently during this lab and in Part 3 as well**

## Step 2 - Configure Roles











