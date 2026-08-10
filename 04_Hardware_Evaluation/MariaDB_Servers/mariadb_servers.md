Explanation: This table outlines an example server architecture for what software would be running on each node of the server that the database systems are on.

Node
CPU
RAM
Storage/Nvme
NIC
OS
Role
Primary Storage Node
2× E5‑2699 v4 (44 cores)
2x32GB DDR4
1TB NVMe
1GbE
Ubuntu 24.04
Auth and Session
Primary Storage Node
2× E5‑2699 v4 (44 cores)
2x32GB DDR4
1TB NVMe
1GbE
Ubuntu 24.04
Sanitized Prompts
Replica Storage Node
2× E5‑2699 v4 (44 cores)
2x32GB DDR4
1TB NVMe
1GbE
Ubuntu 24.04
Auth and Session
Replica Storage Node
2× E5‑2699 v4 (44 cores)
2x32GB DDR4
1TB NVMe
1GbE
Ubuntu 24.04
Sanitized Prompts
Chassis
4× 1280W Platinum PSUs
N/A
12‑Bay NVMe
N/A
N/A
Physical Rails

