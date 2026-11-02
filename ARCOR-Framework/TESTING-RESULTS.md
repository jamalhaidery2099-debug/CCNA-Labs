ARCOR Framework — Testing Results

1. Network Connectivity Testing

Test| Expected Result| Status
R1 to R2 connectivity| Successful| PASS
R2 to R3 connectivity| Successful| PASS
PC-HQ to ISP Server| Successful| PASS
PC-BRANCH to ISP Server| Successful| PASS

2. Dynamic Routing Verification

Protocol| Verification| Status
OSPF| Neighbor and route verification| PASS
EIGRP| Neighbor and route verification| PASS
BGP| eBGP peering verification| PASS
Redistribution| Routes exchanged between routing domains| PASS

3. OSPF Failover Testing

Test Scenario: Direct link between R1-HQ and R3-BRANCH was temporarily disabled.

Before Failure:

- Next Hop: 10.0.31.1
- Interface: GigabitEthernet0/2
- OSPF Metric: 2

After Failure:

- Next Hop: 10.0.12.1
- Interface: GigabitEthernet0/1
- OSPF Metric: 3

Result: OSPF automatically selected the alternate route through R2-CORE.

4. Recovery Testing

The original R1-HQ to R3-BRANCH link was restored.

- Direct route became available again.
- OSPF selected the preferred direct path.
- PC-HQ to PC-BRANCH connectivity remained successful.

Status: PASS

5. Final Conclusion

The ARCOR Framework successfully demonstrated dynamic routing, protocol interoperability, route redistribution, end-to-end connectivity, and automatic recovery from a network link failure.

The testing confirms that the lab can maintain communication through an alternate routing path when the primary connection becomes unavailable.
