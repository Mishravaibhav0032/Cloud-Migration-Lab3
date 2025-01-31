# Cloud-Migration-Lab3
<h1>Section 1: On-Premises Solution Design</h1>

<h3><b>Step 1: Identifying the Current Architecture</b></h3>
<p>A mid-sized retail company currently operates an on-premises infrastructure with:</p>

<p><b>1. Web Application: Monolithic architecture hosted on physical servers.</b></p>
<p><b>2. Database: SQL Server.</b></p>
<p><b>3. File Storage: Local file system.</b></p>
<p><b>4. Networking: Operated through company's routers and firewalls.</b></p>
<p><b>5. Email Service: Used to handle client's notifications.</b></p>

<h3><b>Step 2: Creating an On-Premises Architecture Diagram</b></h3>

![Image](https://github.com/user-attachments/assets/465e78e3-c3fc-45fa-a458-98692d1ea21a)

<h1>Section 2: Migration Strategies</h1>
<h3><b>Step 1: Determining Cloud Service Models</b></h3>
| Component       | Cloud Service Model | Cloud Service         | Migration Approach                                                  |
| --------------- | ------------------- | --------------------- | ------------------------------------------------------------------- |
| Web Application | PaaS or IaaS        | Azure App Service     | Replatforming (Shifting to Paas if applicable else Iaas             |
| Database        | PaaS or IaaS        | Azure SQL Database    | Rehost (Lift and Shift to IaaS in beginning, then refactor to PaaS) |
| File Storage    | PaaS or IaaS        | Azure Blob Storage    | Refactor (Migrating to cloud-native storage services)               |
| Networking      | Cloud-Native        | Azure Virtual Network | Rearchitect (Moving towards cloud-based networking)                 |
| Email Service   | Saas                | Office 365            | Replace (Accepting SaaS-based email services)                       |
