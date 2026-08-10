**6.2.) Software Accessing**  
Explanation: This section details how the software will be accessed for management once inside of the host. It specifies if it should be directly accessed by authenticated users somewhere such as the web, or if it should only be accessed by a CLI by administrators.

Direct Access Table

| Software | Access Type | From Where |
| :---: | ----- | ----- |
| FastAPI | Direct | Web |
| Grafana | Direct | Web  |
| Prometheus \+ Loki | Direct | Web |
| Alertmanager | Direct | Web |
| HashiCorp Vault | Direct | Web  |

Indirect Access Table

| Software | Access Type | From Where |
| :---: | ----- | ----- |
| vLLM | Indirect | Command Line Interface or FastAPI |
| Axolotl | Indirect | Command Line Interface |
| Redis | Indirect | Command Line Interface |
| MariaDB | Indirect | Command Line Interface |
| Nginx | Indirect | Command Line Interface |
| Kubernetes | Indirect | Command Line Interface |

