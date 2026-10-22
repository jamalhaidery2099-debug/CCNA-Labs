*SEAC Framework*

Secure Enterprise Access Control

An Enterprise Network Security Project Built with Cisco Packet Tracer

SEAC is a hands-on enterprise networking project focused on secure network design, traffic control, routing, and access management. It demonstrates how multiple networking and security technologies work together in a simulated enterprise environment.

1. Project Overview

The SEAC (Secure Enterprise Access Control) Framework combines VLAN segmentation, inter-VLAN routing, Access Control Lists (ACLs), NAT/PAT, SSH management restrictions, and switch port security in one Cisco Packet Tracer project.

Project Goals

- Design a structured enterprise network.
- Control traffic between departmental networks.
- Restrict unauthorized network and device access.
- Configure routing and NAT/PAT.
- Test connectivity and verify security policies.

2. Network Topology

![SEAC Enterprise Network Topology](https://github.com/jamalhaidery2099-debug/CCNA-Labs/blob/main/SEAC-Enterprise-Network-Security/seac-topology.png?raw=true)

Network Components

Device| Role
R1-ENTERPRISE| Enterprise routing, ACLs, and NAT/PAT
R2-ISP| Simulated ISP router
S1-CORE| Core switch for departmental connectivity
HR VLAN| Human Resources network
Finance VLAN| Finance department network
IT VLAN| IT department network and authorized management source
Admin VLAN| Administration network
Web Server| External-server simulation for connectivity testing

3. Technologies and Features

- VLANs: Departmental network segmentation
- Inter-VLAN Routing: Communication between VLANs according to configured policies
- Static Routing: Routes between the enterprise and simulated ISP networks
- ACLs: Traffic filtering and access restrictions
- NAT/PAT Overload: Internal address translation
- SSH: Encrypted remote router management
- Switch Port Security: Restrictions on connected devices
- Unused Port Shutdown: Disabling unused switch ports
- Troubleshooting: Connectivity tests and Cisco IOS verification commands

4. Security Policies

- Restrict selected HR-to-Finance traffic using an extended ACL.
- Translate selected internal network traffic using NAT/PAT.
- Restrict SSH management access to the authorized IT PC.
- Apply port security to configured switch access ports.
- Administratively disable unused switch ports.

These controls demonstrate selected network-security and Zero-Trust principles in an educational lab.

5. Configuration Verification

The following Cisco IOS commands can be used to inspect the network configuration and security controls:

show ip interface brief
show ip route
show access-lists
show ip nat translations
show ip nat statistics
show ip ssh
show port-security

6. Project Files and Documentation

- ![SEAC Project Folder](https://github.com/jamalhaidery2099-debug/CCNA-Labs/tree/main/SEAC-Enterprise-Network-Security)
- ![Network Topology Image](https://github.com/jamalhaidery2099-debug/CCNA-Labs/blob/main/SEAC-Enterprise-Network-Security/seac-topology.png)
- ![Router and Switch Configurations](https://github.com/jamalhaidery2099-debug/CCNA-Labs/tree/main/SEAC-Enterprise-Network-Security/configs)
- ![Security Architecture](https://github.com/jamalhaidery2099-debug/CCNA-Labs/blob/main/SEAC-Enterprise-Network-Security/documentation/security-architecture.md)
- ![Testing Results](https://github.com/jamalhaidery2099-debug/CCNA-Labs/blob/main/SEAC-Enterprise-Network-Security/documentation/testing-results.md)

7. Verification Evidence

7.1 Network Topology

![SEAC Network Topology Evidence](https://github.com/jamalhaidery2099-debug/CCNA-Labs/blob/main/SEAC-Enterprise-Network-Security/seac-topology.png?raw=true)

7.2 NAT/PAT Verification

![NAT/PAT Verification](https://github.com/jamalhaidery2099-debug/CCNA-Labs/blob/main/SEAC-Enterprise-Network-Security/nat-pat-verification.png?raw=true)

7.3 ACL Security Verification

![ACL Security Verification](https://github.com/jamalhaidery2099-debug/CCNA-Labs/blob/main/SEAC-Enterprise-Network-Security/acl-security-verification.png?raw=true)

8. Tools and Technologies

- Cisco Packet Tracer
- Cisco IOS Command-Line Interface (CLI)
- GitHub for project documentation and version control

9. Learning Outcomes

This project supports practical learning in:

- Enterprise routing and switching
- VLAN design and segmentation
- ACL-based traffic control
- NAT/PAT configuration and verification
- Secure remote management using SSH
- Layer 2 switch security
- Network troubleshooting and documentation

10. Disclaimer

This project is an educational network simulation built for CCNA practice and portfolio development. It is not presented as a production-ready enterprise security solution.

---

Project: SEAC — Secure Enterprise Access Control
Platform: Cisco Packet Tracer
Focus: Enterprise Networking and Network Security
