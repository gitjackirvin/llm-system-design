Explanation: This table outlines an example hardware configuration for the GPU compute system used to support model inference, training, and Kubernetes orchestration workloads. The configuration below utilizes a multi-node setup designed for performance, scalability, and fault tolerance.

| Item | CPU | RAM | Storage | NVMe | GPU | NIC | Role |
| :---: | ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| GPU Compute Node | 2× Gold 6348 | 128GB 3200 | 480GB SATA | 2TB NVMe | L40 | 100GbE OCP | Model Inference \+ Kubernetes |
| GPU Compute Node | 2× Gold 6348 | 128GB 3200 | 480GB SATA | 2TB NVMe | L40 | 100GbE PCIe | Model Inference \+ Kubernetes |
| Spare Node | 2× Silver 4310 | 64GB 2666 | 480GB SATA | N/A | N/A | 1GbE | Future Expansion |
| Training and GPU Compute Node | 2× Gold 6338N | 256GB 3200 | 480GB SATA | 3.84TB NVMe | L40 | 100GbE PCIe | Model Inference \+ Training \+ Kubernetes |
| Chassis | 2× 2200W PSU | N/A | N/A | N/A | N/A | N/A | Rails \+ 2× C13→C14 Cables |

