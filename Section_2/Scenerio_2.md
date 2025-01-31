<h1>Section 2: Migration Strategies</h1>
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
<p> Phase 2: Replatforming & Optimization</p>
<li>Transition web applications and databases from IaaS to PaaS.</li>
<li>Move file storage and networking components to cloud-native solutions.</li>
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
