**5.4) Switching Requirements**  
Explanation: This section details the Layer 3 Switches that will be selected in order to meet all of the requirements set forth in the subnetting section. It will also detail the cost. These tables below will be used to find a switch that meets all of our requirements.

**This table details the requirements for our Core Switch and our Access Switch in order to ensure full connectivity in our server rack.**

| Requirements | Nodes | Ports | Explanation |
| :---: | ----- | ----- | ----- |
| 100GbE GPU Nodes Usage (Max) | 3 nodes | 4 Ports (Total Port Count)  x 3 Nodes \= 12 Ports | GPU Compute nodes |
| 100GbE Future GPU Nodes Usage (Max) | 6 nodes | 4 Ports x 6 Nodes \= 24 Ports | Planned expansion (6×2U servers) |
| Total 100GbE Ports Required | 9 Nodes | 4 Ports x 9 Nodes \= 36 Ports | 12 \+ 24 future \= 36 Ports |
| 1GbE Nodes Usage (Max) | 3 Nodes | 4 Ports (Total Port Count) x 3 Nodes \= 12 Ports | Non-GPU Compute nodes |
| 1GbE Future Nodes Usage (Max) | 7 Nodes | 4 Ports x 7 Nodes \= 28 Ports | Planned expansion (7x2U servers) |
| Total 100GbE Ports Required | 9 Nodes | 36 Ports | This is the amount of ports our Core Switch will require. |
| Total 1GbE Ports Required | 10 Nodes | 40 Ports | This is the amount of ports our Access Switch will require. |

**5.4.a) Switching Selection \+ Cost**  
Explanation: This section details what switches will be used based on the future expansion requirements and compatibility requirements.

| Switch | Role | Ports | Why It Fits (Expansion \+ Compatibility Requirements) | Estimated Cost |
| :---: | ----- | ----- | ----- | ----- |
| Cisco Nexus 9332C | Core 100GbE Switch | 32×100GbE QSFP28 | Provides dense 100GbE for high‑bandwidth nodes. While it falls short of the theoretical 36‑port requirement, moving to a 48‑port chassis would drastically increase cost. | $12,000–$18,000 |
| Cisco Catalyst C9300‑48T | Access 1GbE Switch | 48×1GbE RJ45 \+ 4×10GbE SFP+ | Supports 48×1GbE ports. This more than meets the 40 1GbE ports that will be used. It also provides VLAN segmentation and remains in the same ecosystem for easier patching and service. | $3,000–$6,000 |

