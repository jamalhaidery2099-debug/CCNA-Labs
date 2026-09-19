Accounts & Delivery Department Network

Project Overview

This project is a departmental network designed and simulated in Cisco Packet Tracer. It connects the Accounts and Delivery departments through VLANs and Router-on-a-Stick inter-VLAN routing.

Network Departments

- Accounts Department — VLAN 10
- Delivery Department — VLAN 20
- Server Network — VLAN 30

IP Addressing

Department| VLAN| Network| Gateway
Accounts| 10| 192.168.10.0/24| 192.168.10.1
Delivery| 20| 192.168.20.0/24| 192.168.20.1
Server| 30| 192.168.30.0/24| 192.168.30.1

Technologies Used

- Cisco Packet Tracer
- VLAN
- Router-on-a-Stick
- Inter-VLAN Routing
- DHCP
- DNS
- Cisco 2911 Router
- Cisco 2960 Switch

Network Features

- Separate VLANs for different departments
- Inter-VLAN communication
- Automatic IP address assignment using DHCP
- DNS name resolution
- Dedicated server network
- Router-on-a-Stick configuration
- Network connectivity testing using Ping

Testing

The following connectivity tests were performed successfully:

- Accounts PC → Accounts Gateway
- Accounts PC → Delivery Network
- Delivery PC → Accounts Network
- PCs → Server
- DNS name resolution using "company.local"

Project Files

- "Accounts-Delivery-Department-Network.pkt" — Cisco Packet Tracer project
- "Network-Diagram.png" — Network topology diagram

Learning Outcomes

This project demonstrates practical knowledge of VLAN configuration, trunking, Router-on-a-Stick, inter-VLAN routing, DHCP, DNS, IP addressing, and basic network troubleshooting.
