## Network Configuration Notes

All virtual machines are connected to a single internal VMware network (VMnet). This isolated network uses the 192.168.31.0/24 subnet, with the following static assignments:

| Hostname     | Role                  | IP Address     |
|---------------|----------------------|----------------|
| DC01          | AD DS, DNS Server     | 192.168.31.130 |
| DC02          | DHCP Server (Authorized) | 192.168.31.132 |
| LINUXCL01     | Samba File Server     | 192.168.31.134 |
| WINCL01       | Windows Client (Standard User) | 192.168.31.133 |
| WINCL02       | Windows Client (IT Support) | 192.168.31.132 |

### Key Setup Steps
- Created a custom VMware virtual network with no external internet connection.  
- Set static IPs on servers and configured DNS forwarding on DC01.  
- Authorized DC02 as the DHCP server within Active Directory.  
- Verified domain join and inter-VM connectivity through ping tests.  
- Enabled file sharing and permission management through AD security groups.  

This setup simulates a small enterprise domain environment for testing Windows and Linux interoperability.
