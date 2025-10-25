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

## Verification Screenshots

Each server and client includes a small set of screenshots demonstrating key configuration steps.  
The complete image collection is organized by system under the [/screenshots](screenshots) directory.

### Domain Controller (DC01)
Active Directory and DNS setup.
![AD Installation](screenshots/dc01_active_directory/ad_installation.png)

### DHCP Server (DC02)
DHCP authorization and scope configuration.
![DHCP Scope](screenshots/dc02_dhcp/dhcp_scope.png)

### Linux File Server (LINUXCL01)
Samba file share configuration and Windows access.
![Samba Share](screenshots/linuxcl01_samba/share_access_windows.png)

### Windows Clients
Domain join and login verification.
![Domain Join](screenshots/wincl01_client/domain_join.png)


## Author

Carlos Mercedes  
TS/SCI Clearance  
[LinkedIn](https://linkedin.com/in/carlosmercedes98)  
[GitHub](https://github.com/CarlosAMercedes)
