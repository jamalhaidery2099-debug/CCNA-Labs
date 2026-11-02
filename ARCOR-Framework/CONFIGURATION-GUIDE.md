ARCOR Framework — Configuration Guide

1. OSPF Multi-Area Configuration

OSPF was implemented to provide dynamic routing between headquarters and branch networks.

R1-HQ

router ospf 1
router-id 1.1.1.1
network 192.168.10.0 0.0.0.255 area 0
network 10.0.12.0 0.0.0.3 area 0
network 10.0.31.0 0.0.0.3 area 0

R3-BRANCH

router ospf 1
router-id 3.3.3.3
network 10.0.23.0 0.0.0.3 area 0
network 10.0.31.0 0.0.0.3 area 0
network 192.168.30.0 0.0.0.255 area 1

2. EIGRP Configuration

EIGRP Autonomous System 100 was configured between R4-REDIST and R5-EDGE.

R4-REDIST

router eigrp 100
network 10.0.45.0 0.0.0.3
no auto-summary

R5-EDGE

router eigrp 100
network 10.0.45.0 0.0.0.3
no auto-summary

3. BGP Configuration

External BGP was configured between the enterprise edge and ISP.

R5-EDGE — AS 65001

router bgp 65001
neighbor 10.0.56.2 remote-as 65002
redistribute eigrp 100

R6-ISP — AS 65002

router bgp 65002
neighbor 10.0.56.1 remote-as 65001
network 203.0.113.0 mask 255.255.255.0

4. Route Redistribution

The routing domains exchange routes using redistribution.

R4-REDIST — OSPF into EIGRP

router eigrp 100
redistribute ospf 1 metric 10000 100 255 1 1500

R5-EDGE — BGP into EIGRP

router eigrp 100
redistribute bgp 65001 metric 10000 100 255 1 1500

R4-REDIST — EIGRP into OSPF

router ospf 1
redistribute eigrp 100 subnets

5. Verification Commands

Command| Purpose
"show ip route"| View routing table
"show ip ospf neighbor"| Verify OSPF neighbors
"show ip eigrp neighbors"| Verify EIGRP neighbors
"show ip bgp summary"| Verify BGP peering
"show ip eigrp topology"| View EIGRP topology
"show ip protocols"| Check routing protocols

6. Configuration Backup

Router configurations were saved using:

copy running-config startup-config

Note: These are the main protocol configurations used in the lab. Interface IP addressing and other device-specific settings are configured separately.
