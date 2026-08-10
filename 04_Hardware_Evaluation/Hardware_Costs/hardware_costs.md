Explanation: This section showcases the costs of each hardware component of the LLM.

| Item | CPU | RAM | OS | NVMe | GPU | NIC | Other | Total |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| GPU Compute Node | $3498 | $1560 | $99 | $390 | $9000 | $390 | N/A | $14,937 |
| GPU Compute Node | $3498 | $1560 | $99 | $390 | $9000 | $79 | N/A | $14,626 |
| Spare Node | $1990 | $420 | $99 | N/A | N/A | $29 | N/A | $2,538 |
| Training and GPU Compute Node | $1980 | $3120 | $99 | $850 | $9000 | $79 | N/A | $15,128 |
| Chassis | N/A | N/A | N/A | N/A | N/A | N/A | Rails: 99 Cables: 6 | $105 |

| Node | CPU | RAM | Storage | NIC | Other | Total |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| Primary Storage Node | $238 | $300 | $470 | $0 | N/A | $1,008 |
| Replica Storage Node | $238 | $300 | $470 | $0 | N/A | $1,008 |
| Replica Storage Node | $238 | $300 | $470 | $0 | N/A | $1,008 |
| Replica Storage Node | $238 | $300 | $470 | $0 | N/A | $1,008 |
| Chassis \+ Rails | N/A | N/A | N/A | N/A | $750 | $750 |

| Node | CPU | RAM | Storage | NIC | Other | Total |
| ----- | :---- | :---- | :---- | :---- | :---- | :---- |
| Primary Observation Node | $34 | $300 | $99 | $0 | N/A | $433 |
| Replica Observation Node | $34 | $300 | $99 | $0 | N/A | $433 |
| Spare Node | $34 | $300 | $99 | $0 | N/A | $433 |
| Secrets Management Node | $34 | $300 | $180 | $0 | N/A | $514 |
| Chassis \+ Rails | N/A | N/A | N/A | N/A | $750 | $750 |

| Node | CPU | RAM | Storage | NIC | Other | Total |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| Request Processing Node A | $238 | $300 | $99 | $0 | N/A | $637 |
| Request Processing Node B | $238 | $300 | $99 | $0 | N/A | $637 |
| Orchestration Control Node | $238 | $300 | $99 | $0 | N/A | $637 |
| Secrets Management Node \+ Kubernetes | $238 | $300 | $99 | $0 | N/A | $637 |
| Chassis \+ Rails | N/A | N/A | N/A | N/A | $750 | $750 |

| Server | Total Cost |
| :---: | ----- |
| GPU Compute Server | $47,334 |
| Database Server | $4,782 |
| Observation Server | $2,563 |
| Request Processing Server | $3,298 |
| Grand Total (All Servers) | $57,977 |

