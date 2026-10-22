2. Network Architecture

The topology contains:

- R1 — Enterprise Router: Connects departmental VLANs and applies routing, ACL, and NAT/PAT policies.
- R2 — ISP Router: Simulates the service-provider network and provides a path to the external web server.
- S1 — Core Switch: Connects departmental devices and enforces configured Layer 2 security.
- Departmental PCs: Represent HR, Finance, IT, and Admin users.
- Web Server: Represents an external server used for connectivity testing.

3. Security Layers

Layer 1 — Network Segmentation

Separate VLANs isolate HR, Finance, IT, and Admin departments into distinct IP networks.

Layer 2 — Inter-VLAN Routing

Router subinterfaces provide communication between VLANs according to the configured policies.

Layer 3 — Access Control Lists

ACLs restrict selected traffic between departments and control access to protected resources.

Layer 4 — Static Routing

Static routes define paths between the enterprise router and the simulated ISP router.

Layer 5 — NAT/PAT

NAT/PAT translates internal source addresses for traffic passing toward the simulated external network.

Layer 6 — Secure Remote Management

SSH provides encrypted remote management, while a VTY access-control list restricts management access to the authorized IT PC.

Layer 7 — Switch Port Security

Port security limits unauthorized device connections on configured access ports.

Layer 8 — Unused Port Protection

Unused switch ports are administratively disabled to reduce unnecessary access opportunities.

4. Zero-Trust Design Principles

The lab demonstrates selected Zero-Trust principles:

- Restrict access instead of allowing unrestricted communication.
- Separate departments using VLANs.
- Apply ACLs to control traffic.
- Limit router management access to an authorized source.
- Restrict access on configured switch ports.
- Verify security controls through testing.

Important: This is a learning demonstration of Zero-Trust principles, not a complete enterprise Zero-Trust deployment.

5. Verification

Use the following commands to inspect the network and security configuration:

show ip interface brief
show ip route
show access-lists
show ip nat translations
show ip nat statistics
show ip ssh
show port-security

6. Conclusion

The SEAC Framework combines routing, segmentation, ACLs, NAT/PAT, SSH access restrictions, and switch port security in one enterprise network lab.

The project demonstrates practical CCNA networking and security skills using Cisco Packet Tracer.

Environment: Educational simulation
Platform: Cisco Packet Tracer
