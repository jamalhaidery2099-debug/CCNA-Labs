# Lab 01 - Basic Router Configuration

## Objective
Configure the basic settings of a Cisco router using the console cable.

## Software
- Cisco Packet Tracer

## Devices Used
- 1 Cisco Router
- 1 PC
- Console Cable

## Configuration Commands

```bash
enable
configure terminal
hostname R1
no ip domain-lookup
enable secret cisco123

line console 0
password console123
login
exit

line vty 0 4
password vty123
login
exit

service password-encryption

banner motd # Unauthorized Access Prohibited #

end

copy running-config startup-config
```

## Verification
- Router hostname changed to **R1**
- Console password configured
- VTY password configured
- Enable secret configured
- Password encryption enabled
- MOTD banner configured
- Configuration saved successfully

## Conclusion
The router was successfully configured with basic security settings using the console cable.
