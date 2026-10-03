# Campus Area Network (CAN) – University Network

## Project Overview

This project presents the design and simulation of a Campus Area Network (CAN) for a university environment using Cisco Packet Tracer.

The network connects multiple university buildings and provides centralized network connectivity through a structured three-layer network architecture.

## Objectives

- Design a scalable university campus network
- Connect multiple academic and administrative buildings
- Implement Access, Distribution, and Core layers
- Separate different types of network traffic using VLANs
- Provide centralized network management
- Connect the campus network to a central server room
- Improve network performance and scalability

## Network Architecture

The network follows Cisco's three-layer hierarchical architecture:

### 1. Access Layer

The Access Layer connects end devices such as:

- PCs
- Printers
- IP Phones
- Other end devices

### 2. Distribution Layer

The Distribution Layer connects Access switches and provides:

- Network aggregation
- Inter-VLAN routing
- Security policies
- Traffic management

### 3. Core Layer

The Core Layer provides high-speed connectivity between different parts of the campus network.

It connects:

- Academic buildings
- Administration block
- Server room
- Distribution switches

## Campus Buildings

The topology contains the following main areas:

### Administration Block

Contains:

- PC
- Printer
- IP Phone
- Administration switch
- Distribution switch

### Academic Building 01

Contains:

- Access switches
- Distribution switch
- End-user network

### Academic Building 02

Contains:

- Access switches
- Distribution switch
- End-user network

### Server Room

Contains:

- Core Switch
- Distribution Switch
- Server Switch
- Network servers

## VLAN Design

Different types of network traffic can be separated using VLANs.

| VLAN | Purpose |
|------|---------|
| VLAN 10 | IPCameras |
| VLAN 20 | IP Phones |
| VLAN 30 | Internet |
| VLAN 100 | Servers |

## Network Devices

The topology uses Cisco networking devices including:

- Core Switch
- Distribution Switches
- Access Switches
- PCs
- Printer
- IP Phone
- Servers

## Physical Connectivity

Building-to-building connectivity is designed as a backbone connection between distribution/core devices.

In a real-world campus network, fiber optic cables can be used for long-distance building-to-building connections because they provide high bandwidth and better resistance to electromagnetic interference.

## Network Management

Network management can be performed from the centralized server room.

Management access can be configured using:

- Management VLAN
- IP addressing
- Remote access
- Device documentation

## Documentation

Network documentation should contain:

- Device names
- Device types
- IP addresses
- VLAN information
- Port information
- Cable connections
- Building/location
- Network purpose

## Tools Used

- Cisco Packet Tracer
- Cisco Networking Devices
- Microsoft Excel / Documentation tools
- GitHub

## Project Files

- `Campus_Area_Network.pkt` – Cisco Packet Tracer project
- `Screenshots/` – Project screenshots
- `Documentation/` – Network documentation and topology image

## Topology

The complete network topology is available in:

`Documentation/topology.png`

## Learning Outcomes

This project demonstrates practical understanding of:

- Campus Area Network design
- Cisco three-layer architecture
- Access, Distribution and Core layers
- VLAN concepts
- Network segmentation
- Switch connectivity
- Network documentation
- Cisco Packet Tracer simulation
- Basic network management
