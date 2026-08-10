5.2.) Cabling Requirements

Explanation: This section outlines the network throughput requirements of the system based on workload demands and communication between components. It is used to determine the appropriate cabling types and infrastructure needed to maintain performance and reliability. The design takes into account expected system load, thermal considerations under heavy usage, and future scalability to ensure the network can support increased demand over time.

5.2.a.) Cabling Assessment
Explanation: This section provides an overview of the network interface requirements across system nodes to determine appropriate cable types and switching capacity. It also considers future expansion and port availability for scaling the infrastructure.

Category
Value
Explanation
GPU Nodes
3× 100GbE QSFP28
Each GPU node uses a 100GbE connection, this means a switch will require QSFP28 ports.
Request Handling Nodes
2× 1GbE RJ45
Uses Cat6a cabling; separated to preserve high-speed bandwidth ports for GPU nodes.
Database and Storage Nodes
4× 1GbE RJ45
Uses Cat6a cabling, standard bandwidth usage for DB nodes doesn’t go over the 1GbE threshold.
Observation Nodes
3× 1GbE RJ45
Low-bandwidth monitoring and logging traffic.
Total 1GbE Ports Needed
8 RJ45 ports
Allows for current usage with additional capacity for flexibility.
Total 100GbE Ports Needed
4 QSFP28 ports
3 GPU nodes + 1 spare port.
Cable Type: Cat6a
8 cables
For all 1GbE nodes
Cable Type: QSFP28 DAC
4 cables
For 100GbE GPU nodes
Server Rack Size
42U
Full‑height rack
Current Space Occupied
16U
Servers + switches + UPS
Leftover Space
26U (≈13 chassis)
The leftover space will be used for expansions.


5.2.b.) Cabling Overview + Cabling Cost
Explanation: This section details all of the necessary cables and receives for proper cabling as well as the costs for cables.

Cable Type
Quantity Needed
Estimated Cost Range
Purpose
Port Type
Cat6a RJ45
8 cables
On hand
Connects Observation, Request Handling, and Database Nodes
1GbE RJ45
QSFP28 DAC
4 cables
$40–$120 each
Connects GPU Nodes to 100GbE switch
100GbE QSFP28
Rack Power Cables
Included with chassis
Included with servers
Power delivery for server chassis
N/A
SFP+/SFP28 Uplink Cable
1–2 cables
$20–$80 each
Uplink from RJ45 access switch to core switch
SFP+/SFP28
Cable Management Accessories
As needed
$20–$50
Velcro straps and cable guides
N/A

