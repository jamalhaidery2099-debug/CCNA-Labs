
SEAC Framework — Secure Enterprise Access Control

Project Overview

SEAC is a Cisco Packet Tracer enterprise networking lab designed to practise network connectivity, traffic control, and basic security.

Network Topology

The lab includes:

- R1-ENTERPRISE router
- R2-ISP router
- S1-CORE switch
- HR, Finance, IT, and Admin VLANs
- Web server

See "seac-topology.png" for the network diagram.

Technologies and Features

- VLANs and Inter-VLAN Routing
- Static Routing
- Extended Access Control Lists (ACLs)
- NAT/PAT Overload
- SSH Remote Management
- Switch Port Security
- Network Troubleshooting

Security Policies

- HR-to-Finance traffic is restricted by an extended ACL.
- NAT/PAT translates selected internal network traffic.
- SSH is configured for remote router management with access restrictions.
- Switch port security limits connected device MAC addresses on access ports.

Verification

The lab was tested using connectivity checks and Cisco IOS show commands, including:

- "show ip interface brief"
- "show ip route"
- "show access-lists"
- "show ip nat statistics"
- "show port-security"

Project Files

- "SEAC-Enterprise-Network.pkt" — Packet Tracer lab file
- "seac-topology.png" — Network topology screenshot
- "configs/" — Router and switch configuration files

Learning Objectives

To develop practical skills in Cisco networking, routing, VLANs, access control, NAT/PAT, SSH, and Layer 2 security.
Project Documentation

- "Security Architecture" (./documentation/security-architecture.md)
- "Testing Results" (./documentation/testing-results.md)

Project Highlights

- Department-based VLAN segmentation
- Extended ACL traffic restrictions
- Static routing between enterprise and ISP routers
- NAT/PAT overload
- SSH management access restricted to the IT PC
- Switch port security and unused-port shutdown
- Connectivity and security verification in Cisco Packet Tracer

Tools Used

- Cisco Packet Tracer
- Cisco IOS CLI
- GitHub for project documentation and version control

Disclaimer

This is an educational lab built for practice. It has not been presented as a production-ready enterprise security solution.
