# vmware-virtual-lab
# Windows and Linux Virtual Lab Environment – VMware Workstation Pro

This project demonstrates a mini enterprise hybrid Windows and Linux network environment configured within a /24 virtual subnet using VMware. It was designed to simulate an enterprise style Active Directory and file sharing for systems administration and integration practice.

---

## Overview

Network Segment: 192.168.31.0/24

| Hostname     | Role / Services     | IP Address     | Operating System |
|---------------|---------------------|----------------|------------------|
| DC01          | AD DS, DNS          | 192.168.31.130 | Windows Server   |
| DC02          | DHCP Authorized     | 192.168.31.132 | Windows Server   |
| LINUXCL01     | Samba File Server   | 192.168.31.134 | Ubuntu Server    |
| WINCL01       | Standard User       | 192.168.31.132 | Windows 10       |
| WINCL02       | IT Support          | 192.168.31.132 | Windows 10       |

---

## Topology Diagram

![Network Topology Diagram](images/topology-diagram.png)

---

## Configuration Notes

- Virtualization Platform: VMware Workstation Pro  
- Domain Controller: Active Directory DS and DNS configured on DC01  
- DHCP: Authorized on DC02  
- File Sharing: Samba configured on LINUXCL01 for cross-platform access  
- Clients: Two Windows workstations joined to the domain  

---

## Skills Demonstrated

- Windows Server Administration  
- Linux File Services (Samba)  
- Active Directory, DNS, and DHCP Configuration  
- Network Topology Documentation  
- Systems Integration in a Virtualized Environment  

---

## Author

Carlos Mercedes  
TS/SCI Clearance  
[LinkedIn](https://linkedin.com/in/carlosmercedes98)  
[GitHub](https://github.com/CarlosAMercedes)
