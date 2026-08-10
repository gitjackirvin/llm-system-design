**5.5.) Total Physical Infrastructure Cost**  
Explanation: This section details all of the physical infrastructure needed for the LLM. It takes into account the servers that are being used, what's running on them, the software being run, and the parts included. The brand is also listed and a total cost is listed at the bottom.

| Hardware Type | Cost | What’s Running On It | Parts Included / Brand |
| :---: | ----- | ----- | ----- |
| 2U Twin Node Server (GPU Compute) | $47,334 | Compute and training services. | 3× NVIDIA L40 GPUs, Intel Xeon Gold 6348/6338N, 128–256GB DDR4 RAM, 2–4TB Samsung/Intel NVMe, 100GbE Mellanox/NVIDIA ConnectX NICs, 2× 2200W PSUs, Supermicro chassis \+ rails |
| 2U Twin Node Server (Database and Storage) | $4,782 | Database and Storage services. | 4× Intel Xeon E5‑2699 v4, 4× 1TB NVMe SSDs, 4× 32GB DDR4 RAM, 1GbE Intel NICs, 12‑bay Supermicro chassis |
| 2U Twin Node Server (Observation) | $2,563 | Metric, logging, and visibility tools. | Intel Xeon E5‑2680 v4, 480GB SATA SSD, 64GB DDR4 RAM, 1GbE Intel NICs, Supermicro chassis |
| 2U Twin Node Server (Request Handling) | $3,298 | Gateway, request handing services. | Intel Xeon E5‑2699 v4, 480GB SATA SSD, 64GB DDR4 RAM, 1GbE Intel NICs, Supermicro chassis |
| UPS System | $2,000–$4,000 | N/A | Eaton 9PX / 93PS 15kVA, battery modules, power conditioning |
| Rack (APC NetShelter SX 42U) | $2,000–$4,000 | N/A | APC NetShelter SX, rails, wheels, airflow baffles, noise‑dampening |
| Switching Hardware | $15,000–$24,000 | N/A | Cisco Nexus 9332C (32×100GbE), Cisco Catalyst C9300‑48T (48×1GbE \+ 4×10GbE) |
| Cabling | $160–$520 | N/A | QSFP28 DAC cables, Cat6a RJ45, SFP+/SFP28 uplinks, cable management accessories |
| TOTAL COST | $76,137 – $90,497 | All hardware combined | Servers \+ Rack \+ UPS \+ Switching \+ Cabling |

