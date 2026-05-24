# Sakura Corp Network Design
## CPE314 - Data Communication & Computer Networks

**Student Name:** SANA AMANAT
**Reg No:** FA23-BCE-108
**Instructor:** Modassir Ishfaq
**University:** COMSATS University Islamabad, Lahore Campus

---

## Project Overview
Enterprise network design for Sakura Corp with:
- Headquarters (HQ) with centralized services
- Branch A and Branch B with VLAN segmentation
- Centralized DHCP, DNS, and Web Server at HQ

---

## Network Topology
- HQ Router connects to Branch A, Branch B, and ISP
- Router-on-a-Stick (ROAS) at each branch
- OSPF routing across all routers
- DHCP Relay (ip helper-address) at branches

---

## IP Addressing Scheme

| Purpose | Network | Gateway |
|---|---|---|
| Server Farm VLAN100 | 192.168.1.0/24 | 192.168.1.1 |
| Branch A Staff VLAN10 | 192.168.10.0/24 | 192.168.10.1 |
| Branch A Guest VLAN20 | 192.168.20.0/24 | 192.168.20.1 |
| Branch B Staff VLAN10 | 192.168.30.0/24 | 192.168.30.1 |
| Branch B Guest VLAN20 | 192.168.40.0/24 | 192.168.40.1 |

---

## Technologies Used
- OSPF (Single Area 0)
- DHCP Relay Agent
- Router on a Stick (ROAS)
- VLANs (10, 20, 100)
- ACLs (Extended)
- Port Security
- VTP Version 2
- DNS Resolution
- HTTP Web Server