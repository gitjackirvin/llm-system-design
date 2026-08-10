**\#Public VLAN Blocked from Database Access**  
**ip access-list PUBLIC-FILTER**

**10 deny ip 10.10.60.0/24 10.10.40.0/24**

**20 permit ip any any**

**interface vlan60**  
**ip access-group PUBLIC-FILTER in**

**\#Management VLAN Allowed Everywhere**  
**ip access-list MANAGEMENT-FULL**

**10 permit ip 10.10.10.0/24 any**

**interface vlan10**  
**ip access-group MANAGEMENT-FULL in**

**\#GPU VLAN can only access Request Nodes**  
