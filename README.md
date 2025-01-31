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

<h3><b>Step 3: Identifying Components for Migration</b></h3>


| Component        | Current State                      | Cloud Service Model (PaaS/IaaS/SaaS)                       |
| ---------------- | ---------------------------------- | ---------------------------------------------------------- |
| Web Application  | Monolithic app on physical server	| IaaS (VMs) or PaaS (App Services)                          |
| Backend Database | SQL Server on local host           | PaaS (Managed SQL) or IaaS (Self-hosted DB)                |
| File Storage	   | Local file system	                | PaaS (Cloud Storage) or IaaS (File Server on VM)           |
| Networking	     | On-prem firewalls & routers        | IaaS (Virtual Networks & Firewalls)                        |
| Email Services   | SMTP server                        | SaaS (Managed Email Services like Office 365, Gmail, etc.) |

<h3><b>Step 4: Description of Components & Dependencies.</b></h3>
<p>A . Web Application (Monolithic Architecture)</p>
<li>Current State: Hosted on a physical server.</li>
<li>Dependency: SQL Server for data storage.</li>
<li>Cloud Migration Approach:</li>
      <li> IaaS: Move to a VM-based infrastructure for easier migration.</li>
      <li> PaaS: Refactor into a container-based microservices architecture using Kubernetes or cloud app services.</li>


<p>B . Backend Database (SQL Server)</p>
<li>Current State: Running on-prem SQL Server.</li>
<li>Dependency: The web application queries this database for transactional data.</li>
<li>Cloud Migration Approach: </li>
      <li>IaaS: Deploy on a Cloud VM with SQL installed.</li>
      <li>PaaS: Use managed database services (e.g., Azure SQL Database, AWS RDS, Google Cloud SQL).</li>

      
<p>C . File Storage (Local File System)</p>
<li>Current State: Files are stored on a local file server.</li>
<li>Dependency: Web application retrieves and updates files.</li>
<li>Cloud Migration Approach:</li>
      <li>PaaS: Using cloud storage solution (e.g Azure Blob Storage).</li>
      <li>IaaS: Deploying a file server in the cloud.</li>


<p>D . Networking (Routers & Firewalls)</p>
<li>Current State: Managed with on-prem routers and firewalls.</li>
<li>Dependency: Secure access control between services and user devices.</li>
<li>Cloud Migration Approach:</li>
      <li>IaaS: Using virtual networking solution (e.g. Azure Virtual Network).</li>
      <li>PaaS: Managing security solutions like firewall-as-a-service.</li>


<p>E . Email Services (SMTP Server)</p>
<li>Current State: SMTP server handles email notifications.</li>
<li>Dependency: Used for client notifications.</li>
      <li>Cloud Migration Approach:</li>
      <li>SaaS: Use managed email services like Microsoft 365.</li>

<h1>Section 2: Migration Strategies</h1>
<h3><b>Step 1: Determining Cloud Service Models</b></h3>

| Component       | Cloud Service Model | Cloud Service         | Migration Approach                                                  |
| --------------- | ------------------- | --------------------- | ------------------------------------------------------------------- |
| Web Application | PaaS or IaaS        | Azure App Service     | Replatforming (Shifting to Paas if applicable else Iaas             |
| Database        | PaaS or IaaS        | Azure SQL Database    | Rehost (Lift and Shift to IaaS in beginning, then refactor to PaaS) |
| File Storage    | PaaS or IaaS        | Azure Blob Storage    | Refactor (Migrating to cloud-native storage services)               |
| Networking      | Cloud-Native        | Azure Virtual Network | Rearchitect (Moving towards cloud-based networking)                 |
| Email Service   | Saas                | Office 365            | Replace (Accepting SaaS-based email services)                       |
