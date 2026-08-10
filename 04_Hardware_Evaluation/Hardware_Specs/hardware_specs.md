Explanation: This section outlines the estimated hardware specifications required for each software component in the system. It takes into account CPU usage, memory requirements, GPU utilization, storage capacity, and operating system compatibility. These specifications are intended to act as baseline guidelines for deployment. Actual requirements may vary depending on system load, scaling needs, and future expansion.

Software Running
CPU Cores Needed
RAM Needed
GPU Needed
Storage Needed
OS Needed
vLLM
8–16 cores
64–128 GB
1× L40
200–500 GB NVMe
Ubuntu 24.04
Axolotl
8–16 cores
64–128 GB
1× L40 (2× ideal)
1–2 TB NVMe
Ubuntu 24.04
FastAPI
2–4 cores
2–4 GB
N/A
<10 GB
Ubuntu 24.04
Nginx
1–2 cores
512 MB–1 GB
N/A
<5 GB
Ubuntu 24.04
Redis
1–2 cores
4–8 GB
N/A
<5 GB
Ubuntu 24.04
Prometheus + Alertmanager
4 cores
16 GB
N/A
200 GB SSD
Ubuntu 24.04
Loki
4–6 cores
8–16 GB
N/A
200–500 GB SSD
Ubuntu 24.04
Grafana
1–2 cores
2–4 GB
N/A
<10 GB
Ubuntu 24.04
MariaDB
4–8 cores
16–32 GB
N/A
500 GB–1 TB NVMe
Ubuntu 24.04
HashiCorp Vault
2–4 cores
4–8 GB
N/A
<20 GB
Ubuntu 24.04

