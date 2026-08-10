Explanation: This section outlines an example server architecture for what software would be  running on each node of the server that metrics are being collected on. It also includes a secrets management instance within the system.

Node
CPU
RAM
Storage
NIC
OS
Role
Primary Observation Node
2× Intel Xeon E5‑2680 v4 (28 cores)
64GB DDR4 Registered
480GB SATA SSD
1GbE onboard
Ubuntu 24.04
Dashboards/Metrics/Logs
Replica Observation Node
2× Intel Xeon E5‑2680 v4 (28 cores)
64GB DDR4 Registered
480GB SATA SSD
1GbE onboard
Ubuntu 24.04
Dashboards/Metrics/Logs
Spare Node
2× Intel Xeon E5‑2680 v4 (28 cores)
64GB DDR4 Registered
480GB SATA SSD
1GbE onboard
Ubuntu 24.04
Spare Node
Secrets Management Node
2× Intel Xeon E5‑2680 v4 (28 cores)
64GB DDR4 Registered
960GB SATA SSD
1GbE onboard
Ubuntu 24.04
Secrets Management/Credential Storage
Chassis
4× 1280W 80Plus Platinum PSUs
N/A
12‑bay NVMe/SATA
N/A
N/A
4‑node chassis + rails

