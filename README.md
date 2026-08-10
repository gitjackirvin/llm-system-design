# Large Language Model System Network Design

This repository contains a complete, structured, and GitHub-optimized version of the **LLM System Network Design Report** authored by **Jack Irvin**.
The original document has been reorganized into modular Markdown files for readability, maintainability, and version control.

## 📘 Purpose

This repository provides a full technical breakdown of designing, deploying, and maintaining an internal Large Language Model (LLM) system, including:

* System capabilities
* Security and infrastructure goals
* Technical stack evaluation
* Hardware architecture
* Physical infrastructure planning
* Backup and scalability strategies
* Cost analysis
* Diagrams and usage scenarios

All content is derived from the provided document.

## 📁 Repository Navigation

![Rack Diagram](https://raw.githubusercontent.com/gitjackirvin/llm-system-design/11_Diagrams/Physical Diagram.drawio.png)

### 1. Introduction

Brief introduction to my project and why I designed it.

* [Introduction](01_Introduction/introduction.md)
  
### 2. Design Requirements

Includes secure infrastructure, low latency, high availability, subnetting isolation, and backup availability as goals.

* [Capabilities](02_Design_Requirements/Capabilities/capabilities.md)
* [Goals](02_Design_Requirements/Goals/goals.md)
* [Security Goals](02_Design_Requirements/Security_Goals/security_goals.md)
* [Physical Infrastructure Goals](02_Design_Requirements/Physical_Infrastructure_Goals/physical_infrastructure_goals.md)
* [Latency SLO](02_Design_Requirements/Latency_SLO/latency_slo.md)
* [Scalability Goals](02_Design_Requirements/Scalability_Goals/scalability_goals.md)
* [Backup Goals](02_Design_Requirements/Backup_Goals/backup_goals.md)
* [Subnetting Goals](02_Design_Requirements/Subnetting_Goals/subnetting_goals.md)

### 3. Technical Evaluation

Includes LLM model selection, training, API frameworks, orchestration, database, caching, metrics, logging, alerting, and credential security.

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

### 4. Hardware Evaluation

Full hardware specifications, GPU compute nodes, database nodes, observability nodes, gateway nodes, UPS selection, and cost tables.

* [Gateway Servers](04_Hardware_Evaluation/Gateway_Servers/gateway_servers.md)
* [UPS Selection](04_Hardware_Evaluation/ups_selection.md)
* [Hardware Costs](04_Hardware_Evaluation/hardware_costs.md)
* [Hardware Specs](04_Hardware_Evaluation/Hardware_Specs/Hardware%20Specs.md)
* [Latency SLO](04_Hardware_Evaluation/latency_slo.md)
* [MariaDB](04_Hardware_Evaluation/Maria_DB/mariadb_.md)
* [Observability Servers](04_Hardware_Evaluation/Observability_Servers/observability_servers.md)
* [Power Usage](04_Hardware_Evaluation/Power_Usage/power_usage.md)
* [Software to Hardware Mapping](04_Hardware_Evaluation/Software_to_Hardware_Mapping/Software%20to%20Hardware%20Mapping.md)
* [Token Estimation / Hardware Token Estimation](04_Hardware_Evaluation/Token_Estimation/Hardware%20Token%20Estimation.md)
* [UPS Selection](04_Hardware_Evaluation/UPS_Selection/ups_selection.md)
* [vLLM / Axolotl Server](04_Hardware_Evaluation/vLLM_Axolotl_Server/Vllm_axolotl_server.md)

### 5. Physical Infrastructure

Rack design, switching, cabling, and total physical cost.

* [Cabling Requirements](05_Physical_Infrastructure/Cabling_Requirements/cabling_requirements.md)
* [Rack Requirements](05_Physical_Infrastructure/Rack_Requirements/rack_requirements.md)
* [Subnetting Requirements](05_Physical_Infrastructure/Subnetting_Requirements/subnetting_requirements.md)
* [Switching Requirements](05_Physical_Infrastructure/Switching_Requirements/switching_requirements.md)
* [Total Physical Cost](05_Physical_Infrastructure/Total_Physical_Cost/total_physical_cost.md)

### 6. Data Access

Proxmox access, metrics access, and security considerations.

* [Proxmox Access](06_Data_Access/Proxmox_Access/proxmox_access.md)
* [Security Considerations](06_Data_Access/Security_Considerations/security_considerations.md)
* [Software Access](06_Data_Access/Software_Access/software_access.md)

### 7. Subnetting

Data segmentation and VLAN design.

* [Data Segmentation](07_Subnetting/Data_Segmentation/data_segmentation.md)
* [VLANs](07_Subnetting/VLANs/vlans.md)

### 8. Scalability

Physical, server, and database scalability planning.

* [Database Scalability](08_Scalability/Database_Scalability/database_scalability.md)
* [Physical Scalability](08_Scalability/Physical_Scalability/physical_scalability.md)
* [Server Scalability](08_Scalability/Server_Scalability/server_scalability.md)

### 9. Backups

Backup locations, schedules, and retention policies.

* [Backup Locations](09_Backups/Backup_Locations/backup_locations.md)
* [Backup Retention](09_Backups/Backup_Retention/backup_retention.md)
* [Backup Schedule](09_Backups/Backup_Schedule/backup_schedule.md)

### 10. Security

Logging, filtering, rate limiting, validation, subnetting, patching, and encryption.

* [Continuous Patching](10_Security/Continuous_Patching/continuous_patching.md)
* [Encryption in Transit](10_Security/Encryption_in_Transit/encryption_in_transit.md)
* [Filtering](10_Security/Filtering/filtering.md)
* [Logging](10_Security/Logging/logging.md)
* [Rate Limiting](10_Security/Rate_Limiting/rate_limiting.md)
* [Separate Subnetting](10_Security/Separate_Subnetting/separate_subnetting.md)
* [Validation & Sanitizing](10_Security/Validation_Sanitizing/validation_sanitizing.md)

### 11. Diagrams

Logical, hardware, and conceptual diagrams.

* [Hardware Diagram Explained](11_Diagrams/Hardware_Diagram/hardware_diagram.md)
* [Hardware Diagram](11_Diagrams/Hardware_Diagram/Physical%20Diagram.drawio.png)
* [Logical Diagram Explained](11_Diagrams/Logical_Diagram/logical_diagram.md)
* [Logical Diagram](11_Diagrams/Logical_Diagram/Rack%20Diagram-Page-3.drawio.png)
* [Rack Diagram Explained](11_Diagrams/Rack_Diagram/rack_diagram.md)
* [Rack Diagram](11_Diagrams/Rack_Diagram/Rack%20Diagram.drawio.png)

### 12. Cost Analysis

Hardware, physical infrastructure, and total cost.

* [Hardware Cost](12_Cost_Analysis/Hardware_Cost/hardware_cost.md)
* [Physical Cost](12_Cost_Analysis/Physical_Cost/physical_cost.md)
* [Total Cost](12_Cost_Analysis/Total_Cost/total_cost.md)

### 13. Uses

Use-case table for the LLM system.

* [Academic & Research](13_Uses/Academic%20%26%20Research.md)
* [Accessibility](13_Uses/Accessibility.md)
* [Automation & Workflow](13_Uses/Automation%20%26%20Workflow.md)
* [Email Automation](13_Uses/Email%20Automation.md)
* [File Conversion & Data Processing](13_Uses/File%20Conversion%20%26%20Data%20Processing.md)
* [Knowledge Management](13_Uses/Knowledge%20Management.md)
* [Meetings & Scheduling](13_Uses/Meetings%20%26%20Scheduling.md)
* [Networking & Infrastructure](13_Uses/Networking%20%26%20Infrastructure.md)
* [Security & Compliance](13_Uses/Security%20%26%20Compliance.md)

### 14. Scripts

* [Access Switch Config](14_Scripts/access_switch_config)
* [ACL Rules](14_Scripts/acl_rules)
* [Core Switch Config](14_Scripts/core_switch_config)
* [LLM Network Design Report](14_Scripts/LLM%20Network%20Design%20Report.md)

---

## 📜 License

This repository contains content provided by the author and is intended for internal or educational use.

## 📬 Contact

For questions or improvements, reach out to the repository maintainer.
