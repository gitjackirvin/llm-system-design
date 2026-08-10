# Large Language Model System Network Design

# About Me: Hello, my name is Jack I am a third-year student studying Cybersecurity and am a aspiring network engineer! I created this project because I am passionate about learning new technologies and wanted to create a lower cost way for medium sized enterprises to host their own LLM models and control their data.

The Large Language Model System Network Design is a complete infrastructure design for deploying and operating an internal Large Language Model environment. The system is designed around security, performance, reliability, scalability, and controlled access, allowing an organization to run AI workloads while maintaining control over its data and infrastructure.
This project was designed to enable organizations to run AI workloads while maintaining control over their data and infrastructure. It was designed with security, performance, scalability, high-availability, and controlled access in mind.

This system supports **LLM inference, model training, APIs, databases, resource monitoring, and automated workflows**. GPU compute, dedicated service servers, and gateway systems are isolated using **VLANs and network segmentation**, while **filtering, rate limiting, encryption, validation, logging, authentication, and continuous patching** protect the environment and control communication between systems.

The design also considers the physical requirements of operating the system, including rack space, switching, cabling, power consumption, UPS protection, hardware requirements, and future expansion. Backup and recovery planning is included to maintain high-availability and protect important system data.

The result is an infrastructure architecture designed to provide an internal AI platform that can support a variety of workloads while remaining secure, observable, maintainable, and scalable. Below is a sample of what the physical rack architecture would look like.

![LLM System Network Design](11_Diagrams/Rack_Diagram/Rack%20Diagram.drawio.png)

---

# 📁 Repository Navigation

The repository is organized into sections. **Click any section below to expand it.**

<details>
<summary><strong>1. Introduction</strong></summary>

### Introduction

A brief introduction to the project and the reasoning behind the system design.

* [Introduction](01_Introduction/introduction.md)

</details>

<details>
<summary><strong>2. Design Requirements</strong></summary>

### Design Requirements

This section establishes the requirements and design goals for the LLM infrastructure, including security, latency, availability, scalability, backups, and network isolation.

* [Capabilities](02_Design_Requirements/Capabilities/capabilities.md)
* [Goals](02_Design_Requirements/Goals/goals.md)
* [Security Goals](02_Design_Requirements/Security_Goals/security_goals.md)
* [Physical Infrastructure Goals](02_Design_Requirements/Physical_Infrastructure_Goals/physical_infrastructure_goals.md)
* [Latency SLO](02_Design_Requirements/Latency_SLO/latency_slo.md)
* [Scalability Goals](02_Design_Requirements/Scalability_Goals/scalability_goals.md)
* [Backup Goals](02_Design_Requirements/Backup_Goals/backup_goals.md)
* [Subnetting Goals](02_Design_Requirements/Subnetting_Goals/subnetting_goals.md)

</details>

<details>
<summary><strong>3. Technical Evaluation</strong></summary>

### Technical Evaluation

Evaluation of the software and technologies required to operate the LLM system.

Topics include LLM model selection, training, APIs, orchestration, databases, caching, metrics, logging, alerting, and credential security.

* [Alerting](03_Technical_Evaluation/Alerting/alerting.md)
* [Backend API](03_Technical_Evaluation/Backend_API/backend_api.md)
* [Caching](03_Technical_Evaluation/Caching/caching.md)
* [Credential Security](03_Technical_Evaluation/Credential_Security/credential_security.md)
* [Database](03_Technical_Evaluation/Database/database.md)
* [Frontend API](03_Technical_Evaluation/Frontend_API/frontend_api.md)
* [Gateway API](03_Technical_Evaluation/Gateway_API/gateway_api.md)
* [LLM Model](03_Technical_Evaluation/LLM_Model/llm_model.md)
* [Log Tracking](03_Technical_Evaluation/Log_Tracking/log_tracking.md)
* [Metrics Dashboard](03_Technical_Evaluation/Metrics_Dashboard/metrics_dashboard.md)
* [Metrics Tool](03_Technical_Evaluation/Metrics_Tool/metrics_tool.md)
* [Model Training](03_Technical_Evaluation/Model_Training/model_training.md)
* [Orchestration](03_Technical_Evaluation/Orchestration/orchestration.md)
* [Reverse Proxy](03_Technical_Evaluation/Reverse_Proxy/reverse_proxy.md)

</details>

<details>
<summary><strong>4. Hardware Evaluation</strong></summary>

### Hardware Evaluation

Evaluation and selection of the physical hardware required to operate the system.

This includes GPU compute nodes, database servers, observability servers, gateway servers, power requirements, UPS systems, hardware costs, and software-to-hardware mapping.

* [Gateway Servers](04_Hardware_Evaluation/Gateway_Servers/gateway_servers.md)
* [Hardware Costs](04_Hardware_Evaluation/hardware_costs.md)
* [Hardware Specs](04_Hardware_Evaluation/Hardware_Specs/Hardware%20Specs.md)
* [Latency SLO](04_Hardware_Evaluation/latency_slo.md)
* [MariaDB](04_Hardware_Evaluation/Maria_DB/mariadb_.md)
* [Observability Servers](04_Hardware_Evaluation/Observability_Servers/observability_servers.md)
* [Power Usage](04_Hardware_Evaluation/Power_Usage/power_usage.md)
* [Software to Hardware Mapping](04_Hardware_Evaluation/Software_to_Hardware_Mapping/Software%20to%20Hardware%20Mapping.md)
* [Hardware Token Estimation](04_Hardware_Evaluation/Token_Estimation/Hardware%20Token%20Estimation.md)
* [UPS Selection](04_Hardware_Evaluation/UPS_Selection/ups_selection.md)
* [vLLM / Axolotl Server](04_Hardware_Evaluation/vLLM_Axolotl_Server/Vllm_axolotl_server.md)

</details>

<details>
<summary><strong>5. Physical Infrastructure</strong></summary>

### Physical Infrastructure

Planning for the physical environment in which the LLM system will operate.

This section covers rack requirements, switching, cabling, subnetting requirements, and overall physical infrastructure costs.

* [Cabling Requirements](05_Physical_Infrastructure/Cabling_Requirements/cabling_requirements.md)
* [Rack Requirements](05_Physical_Infrastructure/Rack_Requirements/rack_requirements.md)
* [Subnetting Requirements](05_Physical_Infrastructure/Subnetting_Requirements/subnetting_requirements.md)
* [Switching Requirements](05_Physical_Infrastructure/Switching_Requirements/switching_requirements.md)
* [Total Physical Cost](05_Physical_Infrastructure/Total_Physical_Cost/total_physical_cost.md)

</details>

<details>
<summary><strong>6. Data Access</strong></summary>

### Data Access

Documentation covering system access, Proxmox access, software access, metrics access, and security considerations.

* [Proxmox Access](06_Data_Access/Proxmox_Access/proxmox_access.md)
* [Security Considerations](06_Data_Access/Security_Considerations/security_considerations.md)
* [Software Access](06_Data_Access/Software_Access/software_access.md)

</details>

<details>
<summary><strong>7. Subnetting</strong></summary>

### Subnetting

Network segmentation and VLAN architecture used to isolate different components of the infrastructure.

* [Data Segmentation](07_Subnetting/Data_Segmentation/data_segmentation.md)
* [VLANs](07_Subnetting/VLANs/vlans.md)

</details>

<details>
<summary><strong>8. Scalability</strong></summary>

### Scalability

Planning for future growth of the physical infrastructure, servers, compute resources, and database systems.

* [Database Scalability](08_Scalability/Database_Scalability/database_scalability.md)
* [Physical Scalability](08_Scalability/Physical_Scalability/physical_scalability.md)
* [Server Scalability](08_Scalability/Server_Scalability/server_scalability.md)

</details>

<details>
<summary><strong>9. Backups</strong></summary>

### Backups

Backup architecture covering backup locations, scheduling, and retention policies.

* [Backup Locations](09_Backups/Backup_Locations/backup_locations.md)
* [Backup Retention](09_Backups/Backup_Retention/backup_retention.md)
* [Backup Schedule](09_Backups/Backup_Schedule/backup_schedule.md)

</details>

<details>
<summary><strong>10. Security</strong></summary>

### Security

Security controls designed to protect the LLM infrastructure and its users.

Topics include logging, filtering, rate limiting, input validation, network segmentation, patching, and encryption.

* [Continuous Patching](10_Security/Continuous_Patching/continuous_patching.md)
* [Encryption in Transit](10_Security/Encryption_in_Transit/encryption_in_transit.md)
* [Filtering](10_Security/Filtering/filtering.md)
* [Logging](10_Security/Logging/logging.md)
* [Rate Limiting](10_Security/Rate_Limiting/rate_limiting.md)
* [Separate Subnetting](10_Security/Separate_Subnetting/separate_subnetting.md)
* [Validation & Sanitizing](10_Security/Validation_Sanitizing/validation_sanitizing.md)

</details>

<details>
<summary><strong>11. Diagrams</strong></summary>

### Diagrams

Architecture diagrams documenting the logical, physical, hardware, and rack designs.

#### Hardware Diagram

* [Hardware Diagram Explanation](11_Diagrams/Hardware_Diagram/hardware_diagram.md)

[![Hardware Diagram](11_Diagrams/Hardware_Diagram/Physical%20Diagram.drawio.png)](11_Diagrams/Hardware_Diagram/Physical%20Diagram.drawio.png)

#### Logical Diagram

* [Logical Diagram Explanation](11_Diagrams/Logical_Diagram/logical_diagram.md)

[![Logical Diagram](11_Diagrams/Logical_Diagram/Rack%20Diagram-Page-3.drawio.png)](11_Diagrams/Logical_Diagram/Rack%20Diagram-Page-3.drawio.png)

#### Rack Diagram

* [Rack Diagram Explanation](11_Diagrams/Rack_Diagram/rack_diagram.md)

[![Rack Diagram](11_Diagrams/Rack_Diagram/Rack%20Diagram.drawio.png)](11_Diagrams/Rack_Diagram/Rack%20Diagram.drawio.png)

</details>

<details>
<summary><strong>12. Cost Analysis</strong></summary>

### Cost Analysis

Analysis of the estimated costs associated with the hardware, physical infrastructure, and complete system.

* [Hardware Cost](12_Cost_Analysis/Hardware_Cost/hardware_cost.md)
* [Physical Cost](12_Cost_Analysis/Physical_Cost/physical_cost.md)
* [Total Cost](12_Cost_Analysis/Total_Cost/total_cost.md)

</details>

<details>
<summary><strong>13. Uses</strong></summary>

### Uses

Potential applications and use cases for the internal LLM system.

* [Academic & Research](13_Uses/Academic%20%26%20Research.md)
* [Accessibility](13_Uses/Accessibility.md)
* [Automation & Workflow](13_Uses/Automation%20%26%20Workflow.md)
* [Email Automation](13_Uses/Email%20Automation.md)
* [File Conversion & Data Processing](13_Uses/File%20Conversion%20%26%20Data%20Processing.md)
* [Knowledge Management](13_Uses/Knowledge%20Management.md)
* [Meetings & Scheduling](13_Uses/Meetings%20%26%20Scheduling.md)
* [Networking & Infrastructure](13_Uses/Networking%20%26%20Infrastructure.md)
* [Security & Compliance](13_Uses/Security%20%26%20Compliance.md)

</details>

<details>
<summary><strong>14. Scripts</strong></summary>

### Scripts

Configuration files, network automation, access-control rules, and supporting project documentation.

* [Access Switch Config](14_Scripts/access_switch_config)
* [ACL Rules](14_Scripts/acl_rules)
* [Core Switch Config](14_Scripts/core_switch_config)
* [LLM Network Design Report](14_Scripts/LLM%20Network%20Design%20Report.md)

</details>

