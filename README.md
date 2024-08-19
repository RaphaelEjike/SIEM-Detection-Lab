# SIEM-Detection-Lab

## Objective

The SIEM Detection Lab project aimed to establish a controlled environment for simulating and detecting cyber attacks. The primary focus was to ingest and analyze logs within a Security Information and Event Management (SIEM) system, generating test telemetry to mimic real-world attack scenarios.

## Tools Used

<ul>
  <li>Security Information and Event Management (SIEM) Azure sentinel system for log ingestion and analysis</li>
  </ul>

## Workflow

#### Deploy Infrastructure:
<ul>
<li>Azure Subscription, VMs, Resource Group, and Log Analytics.</li>
</ul>

#### Set Up and Configure SIEM:

<ul>
<li>Install, configure data sources, create detection rules, and set up dashboards.</li>
</ul>

## Steps for Setting Up the SIEM-Detection-Lab

### 1 Create Azure Subscription:
### Objective: 
<ul>
 <li>To establish a cloud environment where you can create and manage resources needed for the lab. </li>
</ul>

### Actions:
<ul> 
<li>Signed up or logged into the Azure portal. </li>
<li>Activated a subscription that allows you to create and manage Azure resources.</li>
</ul>

### 2 Create Virtual Machines (VMs):
### Objective:
<ul> 
<li> To simulate a network environment where cyber attacks can be generated and monitored.</li>
</ul>
  
### Actions:
<ul>
<li>Navigated to the Azure portal, and in the "Create a resource" section, selected "Virtual Machine."</li>
<li>Configured VM settings such as operating system, size, and region.</li>
<li>Deployed one or more VMs that will serve as hosts to simulate both attacker and victim roles.</li>
 </ul>

### 3 Create a Resource Group:
### Objective:
 <ul>
<li>To organise and manage your Azure resources in a logical container.</li>
</ul>

### Actions:
<ul>
<li>In the Azure portal, navigated to "Resource groups" and selected "Create." </li>
<li>Defined a name for the resource group and selected a region. </li>
<li>Added all related Azure resources (VMs, Log Analytics, etc.) into this resource group to keep them organised. </li>
</ul>

### 4 Create Log Analytics Workspace:

### Objective: 

<ul> 
<li>To collect, correlate, and analyse logs from the VMs in a centralised SIEM system.</li>
</ul>

### Actions:
<ul>
<li>From the Azure portal, selected "Log Analytics" under the Monitoring section and chose "Create."</li>
<li>Named the workspace and chose the appropriate subscription, resource group, and region.</li>
<li>Configured the workspace to be ready to ingest logs from the VMs.</li>
</ul>

### 5 Connect VMs to Log Analytics:

### Objective:
<ul> 
<li>To start collecting and analyzing logs from the VMs in the Log Analytics workspace.</li>
</ul>

### Actions:
<ul> 
<li> Installed the Microsoft Monitoring Agent (MMA) on the VMs, which allows them to send logs to the Log Analytics workspace.</li>
<li> Configured each VM to connect to the Log Analytics workspace by providing the workspace ID and key.</li>
<li> Verified the connection to ensure logs from the VMs were being ingested successfully into Log Analytics. </li>
</ul> 

### 6 Configure Data Sources:

### Objective:
<ul> 
<li>To ensure that logs from various sources are collected and sent to the SIEM system for analysis.</li>
</ul>

### Actions:
<ul> 
<li> Set up data connectors in the SIEM system to ingest logs from various sources (e.g., VMs, firewalls, application logs).</li>
<li> Ensured that the logs from your VMs were being forwarded to the SIEM system, using protocols like Syslog or by installing necessary agents.</li>
</ul> 

### 7 Create and Tune Detection Rules Configure Data Sources:

### Objective:
<ul> 
<li> To identify and accurately detect specific attack patterns and reduce the occurrence of false positives. </li>
</ul>

### Actions:
<ul> 
<li> Developed custom detection rules or used predefined rules to identify specific attack patterns.</li>
<li> Tuned these rules to minimise false positives and optimise detection accuracy.</li>
</ul> 

### 8 Create Dashboards and Alerts:

### Objective:
<ul> 
<li> To visualise incoming logs, monitor trends, and receive notifications for detected threats. </li>
</ul>

### Actions:
<ul> 
<li> Set up dashboards within the SIEM system to visualise incoming logs, trends, and detected threats.</li>
<li> Configured alerting mechanisms to notify you of suspicious activities in real-time.</li>
</ul> 


## Skills Learned Recap

<ul>
  <li>Advanced understanding of SIEM concepts and practical application</li>
  <li> Proficiency in Log Collection and Analysis</li>
  <li>Custom Rule Development and Tuning</li>
</ul>

