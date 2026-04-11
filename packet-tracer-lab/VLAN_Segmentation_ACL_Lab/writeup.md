# VLAN Segmentation & ACL Lab

**Tools:** Cisco Packet Tracer, IOS CLI  
**Date:** April 2026

## Objective
Build a segmented office network with VLANs, inter-VLAN routing, DHCP, DNS, and ACLs enforcing least privilege between departments.

## Topology
*(screenshot)*

## IP Plan
| Segment | VLAN | Network | Gateway |
|---------|------|---------|---------|
| IT | 10 | 192.168.10.0/24 | 192.168.10.1 |
| HR | 20 | 192.168.20.0/24 | 192.168.20.1 |
| Guest | 30 | 192.168.30.0/24 | 192.168.30.1 |

## What I Configured
- VLANs 10, 20, 30 on all switches with trunk links
- Inter-VLAN routing via SVIs on Multilayer Switch
- DHCP pools per VLAN with automatic IP assignment
- DNS server with intranet.local A record
- Extended ACL blocking Guest from IT and HR subnets

## Test Results
- PC0 (IT) → ping 192.168.20.1 ✅ success
- PC2 (Guest) → ping 192.168.10.1 ❌ blocked by ACL
- PC1 (HR) → ping intranet.local ✅ resolved to 192.168.20.100

## Security Concepts Demonstrated
- Network segmentation
- Least privilege access control
- Defense in depth
- DNS and DHCP infrastructure services

## Screenshots
*(add screenshots here)*
