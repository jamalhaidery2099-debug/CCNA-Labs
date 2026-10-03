# Accounts & Delivery Department Network

## Project Overview

This project presents the design and simulation of a departmental network for **Accounts and Delivery departments** using Cisco Packet Tracer.

The network uses **VLANs** to separate departments and **Router-on-a-Stick** for inter-VLAN communication. A dedicated server VLAN is also configured to provide network services such as **DHCP and DNS**.

## Network Departments

| Department / Network |    VLAN |
| -------------------- | ------: |
| Accounts Department  | VLAN 10 |
| Delivery Department  | VLAN 20 |
| Server Network       | VLAN 30 |

## IP Addressing

| Network  | VLAN | Network Address | Default Gateway |
| -------- | ---: | --------------- | --------------- |
| Accounts |   10 | 192.168.10.0/24 | 192.168.10.1    |
| Delivery |   20 | 192.168.20.0/24 | 192.168.20.1    |
| Server   |   30 | 192.168.30.0/24 | 192.168.30.1    |

## Network Topology

The network consists of:

* Cisco 2911 Router
* Cisco 2960 Switch
* Accounts PCs
* Delivery PCs
* Server
* VLANs for network segmentation

## Technologies Used

* Cisco Packet Tracer
* VLAN
* Trunking
* Router-on-a-Stick
* Inter-VLAN Routing
* DHCP
* DNS
* IP Addressing
* Ping Testing

## Network Features

* Separate VLANs for Accounts and Delivery departments
* Dedicated Server VLAN
* Router-on-a-Stick inter-VLAN routing
* Automatic IP address assignment using DHCP
* DNS name resolution
* Trunk connection between switch and router
* Connectivity testing using Ping

## VLAN Configuration

### VLAN 10 – Accounts

**Network:** `192.168.10.0/24`
**Gateway:** `192.168.10.1`

### VLAN 20 – Delivery

**Network:** `192.168.20.0/24`
**Gateway:** `192.168.20.1`

### VLAN 30 – Server

**Network:** `192.168.30.0/24`
**Gateway:** `192.168.30.1`

## Testing

The following tests were performed to verify network connectivity:

* Accounts PC → Accounts Gateway
* Delivery PC → Delivery Gateway
* Accounts PC → Delivery Network
* Delivery PC → Accounts Network
* Accounts PC → Server
* Delivery PC → Server
* DNS name resolution using `company.local`

Successful ping responses confirm connectivity between the configured networks.

## Network Services

### DHCP

DHCP is used to automatically assign IP addresses and network information to client PCs.

### DNS

DNS is configured to provide name resolution for the network.

Example:

`company.local`

## Project Files

* `Accounts-Delivery-Department-Network.pkt` — Cisco Packet Tracer project
* `Network-Diagram.png` — Network topology diagram

## Learning Outcomes

This project demonstrates practical knowledge of:

* VLAN configuration
* VLAN segmentation
* Access and trunk ports
* Router-on-a-Stick
* Inter-VLAN routing
* DHCP configuration
* DNS configuration
* IP addressing
* Network connectivity testing
* Basic network troubleshooting
* Cisco Packet Tracer simulation

## Conclusion

This project demonstrates how VLANs, Router-on-a-Stick, DHCP, and DNS can be combined to build a structured departmental network. The configuration was tested using connectivity and DNS resolution tests in Cisco Packet Tracer.
