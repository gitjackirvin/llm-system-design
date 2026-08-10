Explanation: This section outlines an example server architecture for what software would be running on each node of the server where user requests are initially processed along with the associated hardware specifications.

Node
CPU
RAM
Storage
NIC
OS
Role
Request Processing Node A
2× Intel Xeon E5‑2699 v4 (44 cores)
64GB DDR4
480GB SATA SSD
1GbE
Ubuntu 24.04
API Gateway / Request Processing / Caching + Kubernetes Worker
Request Processing Node B
2× Intel Xeon E5‑2699 v4 (44 cores)
64GB DDR4
480GB SATA SSD
1GbE
Ubuntu 24.04
API Gateway / Request Processing / Caching + Kubernetes Worker
Orchestration Control Node 
2× Intel Xeon E5‑2699 v4 (44 cores)
64GB DDR4
480GB SATA SSD
1GbE
Ubuntu 24.04
Kubernetes Control Plane
Secrets Management Node + Kubernetes
2× Intel Xeon E5‑2699 v4 (44 cores)
64GB DDR4
480GB SATA SSD
1GbE
Ubuntu 24.04
Secrets Management + Cluster Orchestration Services


Chassis
4× 1280W PSUs
N/A
12‑Bay NVMe/SATA
N/A
N/A
Rails Included 

