SEAC Framework — Secure Enterprise Access Control

A Cisco Packet Tracer enterprise networking project demonstrating network segmentation, traffic control, routing, and multiple security controls.

Project Overview

The SEAC (Secure Enterprise Access Control) Framework is an enterprise network security lab designed to practise Cisco networking, access control, and troubleshooting. It combines routing, VLANs, ACLs, NAT/PAT, SSH access restrictions, and Layer 2 security in one simulated network.

Network Topology

![SEAC Enterprise Network Topology](https://github.com/jamalhaidery2099-debug/CCNA-Labs/blob/main/SEAC-Enterprise-Network-Security/seac-topology.png?raw=true)

The topology includes:

- R1-ENTERPRISE: Enterprise router for VLAN routing, ACLs, and NAT/PAT.
- R2-ISP: ISP simulation router.
- S1-CORE: Core switch connecting departmental devices.
- HR, Finance, IT, and Admin: Separate departmental VLANs.
- Web Server: External-server simulation for connectivity testing.

Technologies and Features

- VLANs and inter-VLAN routing
- Static routing
- Standard and extended Access Control Lists (ACLs)
- NAT/PAT overload
- SSH remote management
- Switch port security
- Unused switch-port shutdown
- Network troubleshooting and verification

Security Policies

- Restrict selected HR-to-Finance traffic using an extended ACL.
- Translate selected internal network traffic using NAT/PAT.
- Restrict SSH management access to the authorized IT PC.
- Limit device access on configured switch ports using port security.
- Administratively disable unused switch ports.

Verification

The following Cisco IOS commands can be used to inspect the configuration and verify the lab:

show ip interface brief
show ip route
show access-lists
show ip nat translations
show ip nat statistics
show ip ssh
show port-security

Project Files

- ""SEAC-Enterprise-Network.pkt"" (./SEAC-Enterprise-Network.pkt) — Packet Tracer lab file.
- ""seac-topology.png"" (./seac-topology.png) — Network topology image.
- ""configs/"" (./configs/) — Router and switch configuration files.
- ""documentation/security-architecture.md"" (./documentation/security-architecture.md) — Security architecture.
- ""documentation/testing-results.md"" (./documentation/testing-results.md) — Testing documentation.

Verification Evidence

Network Topology

"SEAC Network Topology" (https://github.com/jamalhaidery2099-debug/CCNA-Labs/blob/main/SEAC-Enterprise-Network-Security/seac-topology.png?raw=true)

NAT/PAT Verification

"NAT/PAT Verification" (https://github.com/jamalhaidery2099-debug/CCNA-Labs/blob/main/SEAC-Enterprise-Network-Security/nat-pat-verification.png?raw=true)

ACL Security Verification

"ACL Security Verification" (https://github.com/jamalhaidery2099-debug/CCNA-Labs/blob/main/SEAC-Enterprise-Network-Security/acl-security-verification.png?raw=true)

Tools Used

- Cisco Packet Tracer
- Cisco IOS CLI
- GitHub for project documentation and version control

Learning Objectives

- Practise enterprise routing and switching.
- Understand VLAN-based network segmentation.
- Apply ACLs to control network traffic.
- Configure and verify NAT/PAT.
- Secure remote management using SSH.
- Implement switch port security.
- Document and troubleshoot a multi-device network.

Disclaimer

This project is an educational simulation built for networking practice. It is not presented as a production-ready enterprise security solution.
