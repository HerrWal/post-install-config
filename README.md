<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration 🚀</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Protocol (RDP)
- Internet Information Services (IIS)
- osTicket Web Interface

<h2>Operating Systems Used</h2>

- Windows 10 (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Understand the difference between Agent and Admin panels
- Create and assign Roles, Departments, and Teams
- Configure Agent and User accounts
- Enforce user registration policies
- Define SLAs and Help Topics for ticket routing

<h2>Configuration Steps</h2>

<h3>1. Access Admin and End-User Portals</h3>
<p>
<img src="https://i.imgur.com/yU3LALU.png" height="80%" width="80%" alt="Admin Login Page"/>
<img src="https://i.imgur.com/cOF8oW4.png" height="80%" width="80%" alt="User Login Page"/>
</p>
<p>
Login to the osTicket Admin Panel:<br/>
👉 <code>http://localhost/osTicket/scp/login.php</code><br/>
End-User Portal for submitting tickets:<br/>
👉 <code>http://localhost/osTicket</code><br/>
Understand the difference between the <b>Agent Panel</b> (for support staff) and the <b>Admin Panel</b> (for configuring the system).
</p>
<br />

<h3>2. Configure Roles</h3>
<p>
<img src="https://i.imgur.com/wwiMA9A.png" height="80%" width="80%" alt="Configuring Roles"/>
</p>
<p>
Navigate to: <code>Admin Panel → Agents → Roles</code><br/>
Create a new role: <b>Supreme Admin</b><br/>
Roles are used to group permission sets that define what actions agents can perform.
In this instance, let's grant all permissions and select all boxes on all the tabs.
</p>
<br />

<h3>3. Configure Departments</h3>
<p>
<img src="https://i.imgur.com/ofafXh9.png" height="80%" width="80%" alt="Departments"/>
</p>
<p>
Navigate to: <code>Admin Panel → Agents → Departments</code><br/>
Departments determine ticket visibility and workflow. Create example departments like:
<ul>
  <li><b>SysAdmins</b></li>
  <li><b>Support</b></li>
  <li><b>Networking</b></li>
</ul>
</p>
<br />

<h3>4. Create Teams</h3>
<p>
<img src="https://i.imgur.com/Dgl6A97.png" height="80%" width="80%" alt="Teams"/>
</p>
<p>
Navigate to: <code>Admin Panel → Agents → Teams</code><br/>
Teams allow you to group agents from different departments. Example team: <b>Online Banking</b>
</p>
<br />

<h3>5. Adjust User Registration Settings</h3>
<p>
<img src="https://i.imgur.com/WPAoT95.png" height="80%" width="80%" alt="User Registration Settings"/>
</p>
<p>
Navigate to: <code>Admin Panel → Settings → User Settings</code><br/>
Make sure is unchecked: <b>"Require registration and login to create tickets"</b><br/>
Enable: <b>"Registration Required"</b><br/>
This restricts ticket creation to registered users only.
</p>
<br />

<h3>6. Add Agents</h3>
<p>
<img src="https://i.imgur.com/iCVrWgR.png" height="80%" width="80%" alt="Add Agent"/>
</p>
<p>
Navigate to: <code>Admin Panel → Agents → Add New</code><br/>
Create support agents such as:
<ul>
  <li><b>Jane</b> (Department: SysAdmins)</li>
  <li><b>John</b> (Department: Support)</li>
</ul>
</p>
<br />

<h3>7. Add End Users</h3>
<p>
<img src="https://i.imgur.com/48QRWXb.png" height="80%" width="80%" alt="Add User"/>
</p>
<p>
Navigate to: <code>Agent Panel → Users → Add New</code><br/>
Add sample users (customers):
<ul>
  <li><b>Karen</b></li>
  <li><b>Ken</b></li>
</ul>
</p>
<br />

<h3>8. Configure SLA Plans</h3>
<p>
<img src="https://i.imgur.com/0wrDMZ0.png" height="80%" width="80%" alt="SLA Plans"/>
</p>
<p>
Navigate to: <code>Admin Panel → Manage → SLA</code><br/>
Define Service Level Agreements:
<ul>
  <li><b>Sev-A</b>: 1 hour (24/7)</li>
  <li><b>Sev-B</b>: 4 hours (24/7)</li>
  <li><b>Sev-C</b>: 8 hours (Business Hours)</li>
</ul>
SLA plans determine response deadlines based on ticket severity.
</p>
<br />

<h3>9. Create Help Topics</h3>
<p>
<img src="https://i.imgur.com/RSikZMT.png" height="80%" width="80%" alt="Help Topics"/>
</p>
<p>
Navigate to: <code>Admin Panel → Manage → Help Topics</code><br/>
Create topics that users select when submitting tickets. Examples:
<ul>
  <li>Business Critical Outage</li>
  <li>Personal Computer Issues</li>
  <li>Equipment Request</li>
  <li>Password Reset</li>
  <li>Other</li>
</ul>
These help route tickets to the correct department or team.
</p>
<br />

<h2>Conclusion</h2>

<p>
With the post-install configuration complete, your osTicket system is now tailored for your organization's support workflow. Agents are assigned, users are registered, and tickets can be prioritized using SLA plans and help topics. These foundational steps not only make the help desk functional, but also scalable and efficient.
</p>

<p>
From here, you can further enhance your setup by configuring email integration, setting up automated responses, and exploring analytics tools to track performance. Your help desk is live and ready to serve! 🚀
</p>
