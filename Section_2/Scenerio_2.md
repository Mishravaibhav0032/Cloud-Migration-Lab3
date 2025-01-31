<h1>Section 2: Migration Strategies - Migration Plan</h1>
<h3><b>Step 1: Determining Cloud Service Models</b></h3>

| Component       | Cloud Service Model | Cloud Service         | Migration Approach                                                  |
| --------------- | ------------------- | --------------------- | ------------------------------------------------------------------- |
| Web Application | PaaS or IaaS        | Azure App Service     | Replatforming (Shifting to Paas if applicable else Iaas             |
| Database        | PaaS or IaaS        | Azure SQL Database    | Rehost (Lift and Shift to IaaS in beginning, then refactor to PaaS) |
| File Storage    | PaaS or IaaS        | Azure Blob Storage    | Refactor (Migrating to cloud-native storage services)               |
| Networking      | Cloud-Native        | Azure Virtual Network | Rearchitect (Moving towards cloud-based networking)                 |
| Email Service   | Saas                | Office 365            | Replace (Accepting SaaS-based email services)                       |


<h3><b>Step 2: Hybrid Migration Approach</b></h3>

<p>This plan follows a phased migration strategy:</p>
<p> Phase 1: Lift and Shift (IaaS-Based Migration)</p>
<li>Move web applications and databases to IaaS with minimal modifications.</li>
<li>Establish hybrid connectivity and test cloud performance.</li>
<p></p>
<ul>1. Web Application : Deploy to Azure Virtual Machines (IaaS).</ul>
<ul>2. Database : Migrate to Azure SQL Virtual Machines (IaaS).</ul>
<ul>3. File Storage : Move to Azure Files or Azure Blob Storage.</ul>
<ul>4. Networking : Set up Azure Virtual Network (VNet) and establish hybrid connectivity.</ul>
<ul>5. Email Service : Continue using on-premises service until SaaS transition.</ul>
<p></p>
<p> Phase 2: Replatforming & Optimization</p>
<li>Transition web applications and databases from IaaS to PaaS.</li>
<li>Move file storage and networking components to cloud-native solutions.</li>
<p></p>
<ul>1. Web Application : Transition from IaaS VMs to Azure App Service (PaaS).</ul>
<ul>2. Database : Migrate from SQL Server on IaaS to Azure SQL Database (PaaS).</ul>
<ul>3. File Storage : Optimize and utilize Azure Blob Storage for scalability.</ul>
<ul>4. Networking : Implement Azure Firewall and Azure Load Balancer for security and high availability.</ul>
<ul>5. Email Service : Begin transition to Office 365 (SaaS).</ul>
<p></p>
<p> Phase 3: Full Cloud Adoption & Automation</p>
<li>Migrate email services to SaaS.</li>
<li>Optimize security, cost, and performance.</li>
<li>Implement cloud automation and monitoring tools.</li>
<p></p>
<p> Final Considerations </p>
<li>1. Security & Compliance : Implement IAM policies, encryption, and compliance standards.</li>
<li>2. Backup & Disaster Recovery : Utilize cloud backup solutions and multi-region replication.</li>
<li>3. Monitor Performance : Using cloud-native monitoring tools (e.g. Azure Monitor).</li>
<li>4. Optimization of Cost : Purchasing reserved instances and autoscaling features to improve costs.</li>
