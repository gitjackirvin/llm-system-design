Explanation: This section outlines the subnetting requirements for the traffic on the server rack. All traffic will need to be segmented onto their own VLAN’s to separate broadcast domains as well as limit access to data to only authorized users.

Item
Requirement
Explanation
VLAN Segmentation
Multiple VLANs required
Separates all the different servers into separate broadcast domains.
Inter-VLAN Communication
Inter-VLAN Routing must be configured
Needed so all the servers can communicate securely across VLANs to complete requests.
Layer 3 Switch
Mandatory for routing + segmentation
Provides communication between VLANs and segmentation.
Security Isolation
Rack must be isolated from general LAN
Prevents unauthorized external devices from accessing nodes directly. This reduces attack surface and prevents bandwidth being exhausted by incorrect traffic reaching the server rack.
Latency Optimization
Ensure quick speeds and no bottlenecks in the server rack
Ensures all requests fall within the Latency Service-Level Objective times.

