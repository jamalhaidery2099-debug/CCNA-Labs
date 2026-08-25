🔐 Network Security & Device Hardening

📌 Project Overview

This project demonstrates the implementation of basic network security and device hardening techniques using Cisco Packet Tracer.

The network consists of a router, switch, and PC. Security configurations were applied to protect network devices from unauthorized access and to control access to switch ports.

🎯 Objectives

- Secure Cisco router and switch access
- Configure privileged EXEC password protection
- Configure console password protection
- Configure SSH for secure remote management
- Configure local user authentication
- Enable switch port security
- Secure unused switch ports
- Verify network connectivity and security configurations

🖥️ Network Topology

PC0 → SW1 → R1

- PC0: "192.168.1.10/24"
- SW1 Management IP: "192.168.1.2/24"
- R1: "192.168.1.1/24"

🔐 Security Features Implemented

1. Device Password Security

Router and switch were protected using:

- Enable Secret
- Console Password
- Password Encryption
- MOTD Banner

2. SSH Configuration

SSH was configured for secure remote management.

Configuration included:

- Local username authentication
- Domain name
- RSA key generation
- SSH Version 2
- VTY line authentication
- SSH-only remote access

3. Switch Port Security

Port Security was configured on "FastEthernet0/1".

Configuration:

- Maximum MAC addresses: "1"
- Sticky MAC address learning
- Violation mode: "shutdown"

This helps prevent unauthorized devices from accessing the protected switch port.

4. Unused Port Shutdown

Unused switch ports from "FastEthernet0/2" to "FastEthernet0/23" were administratively shut down.

This reduces the possibility of unauthorized physical network access.

🧪 Testing & Verification

The following commands were used to verify the configuration:

show ip ssh
show running-config
show port-security interface fastEthernet 0/1
show ip interface brief
ping 192.168.1.1

The network connectivity and security configurations were successfully verified.

🛠️ Tools Used

- Cisco Packet Tracer
- Cisco IOS CLI
- Router
- Layer 2 Switch
- PC

📸 Project Screenshots

Network Topology

"Network Topology" (01-Topology.png)

Router Security

"Router Security" (02-Router-Security.png)

SSH Configuration

"SSH Configuration" (03-SSH-Configuration.png)

Switch Security

"Switch Security" (04-Switch-Security.png)

Port Security

"Port Security" (05-Port-Security.png)

Unused Ports

"Unused Ports" (06-Unused-Ports.png)

Final Verification

"Final Verification" (07-Final-Verification.png)

📁 Project Files

- "Network-Security-and-Device-Hardening.pkt" — Cisco Packet Tracer project
- "README.md" — Project documentation
- PNG files — Configuration and verification screenshots

✅ Conclusion

This project demonstrates practical network security and device hardening using Cisco Packet Tracer.

The router and switch were secured using authentication, SSH, port security, and unused-port shutdown techniques. The project also demonstrates basic verification and troubleshooting commands used in Cisco networking environments.
