# Campus Area Network (CAN) – University Network

## Project Overview

This project presents the design and simulation of a **Campus Area Network (CAN)** for a university environment using Cisco Packet Tracer.

The network connects multiple university buildings and provides centralized network connectivity using Cisco's **three-layer hierarchical network architecture**.

## Objectives

* Design a scalable university campus network
* Connect multiple academic and administrative buildings
* Implement Access, Distribution, and Core layers
* Separate network traffic using VLANs
* Provide centralized network management
* Implement basic network security
* Configure secure device access
* Connect the campus network to a central server room
* Improve network performance and scalability

## Network Architecture

The network follows Cisco's three-layer hierarchical architecture.

### 1. Access Layer

The Access Layer connects end devices such as:

* PCs
* Printers
* IP Phones
* Other end devices

### 2. Distribution Layer

The Distribution Layer connects Access switches and provides:

* Network aggregation
* Inter-VLAN routing
* Security policies
* Traffic management

### 3. Core Layer

The Core Layer provides high-speed connectivity between different parts of the campus network.

It connects:

* Academic buildings
* Administration block
* Server room
* Distribution switches

## Campus Buildings

### Administration Block

Contains:

* PCs
* Printer
* IP Phone
* Administration Access Switch
* Distribution Switch

### Academic Building 01

Contains:

* Access Switches
* Distribution Switch
* End-user network

### Academic Building 02

Contains:

* Access Switches
* Distribution Switch
* End-user network

### Server Room

Contains:

* Core Switch
* Distribution Switch
* Server Switch
* Network Servers

## VLAN Design

Different types of network traffic are separated using VLANs.

| VLAN     | Purpose    |
| -------- | ---------- |
| VLAN 10  | IP Cameras |
| VLAN 20  | IP Phones  |
| VLAN 30  | Internet   |
| VLAN 100 | Servers    |

VLAN segmentation helps organize network traffic and provides better control over different network services.

## Network Security

Basic security configurations have been implemented on network devices to improve device protection and management.

Security-related configurations include:

* Console password protection
* Privileged EXEC mode password
* Encrypted passwords
* Login security
* Device access protection
* Secure remote management where configured

These configurations help prevent unauthorized access to network devices.

## Device Management and Remote Access

Network devices can be managed from the centralized server room.

Management features include:

* Management VLAN
* IP addressing
* Console access
* Remote device access
* Device naming
* Password protection
* Network documentation

Where configured, **SSH remote access** allows an administrator to securely access network switches from a remote computer or server without physically connecting to the switch.

## Console Access

Console access provides local management of Cisco network devices.

It can be used for:

* Initial device configuration
* Password configuration
* Troubleshooting
* Device management when remote access is unavailable

Console access is protected using authentication credentials configured on the Cisco devices.

## Physical Connectivity

Building-to-building connectivity is designed as a backbone connection between distribution and core devices.

In a real-world campus network, **fiber-optic cables** can be used for long-distance building-to-building connections because they provide high bandwidth and better resistance to electromagnetic interference.

## Network Management

Centralized network management can be performed from the server room.

The network administrator can manage and monitor devices using:

* Console access
* Remote access
* Management VLAN
* IP addressing
* Device documentation

## Documentation

Network documentation contains:

* Device names
* Device types
* IP addresses
* VLAN information
* Port information
* Cable connections
* Building/location
* Network purpose
* Security configuration
* Management information

## Network Devices

The topology uses Cisco networking devices including:

* Core Switch
* Distribution Switches
* Access Switches
* PCs
* Printer
* IP Phone
* Servers

## Tools Used

* Cisco Packet Tracer
* Cisco Networking Devices
* Microsoft Excel / Documentation Tools
* GitHub

## Project Files

* `Campus_Area_Network.pkt` – Cisco Packet Tracer project
* `Screenshots/` – Project configuration and testing screenshots

## Screenshots

The Screenshots folder contains visual evidence of:

* Complete network topology
* VLAN configuration
* Security configuration
* Console access configuration
* Remote/SSH access testing
* Network connectivity testing

## Topology

The complete network topology is available in:

`topology.png`

## Learning Outcomes

This project demonstrates practical understanding of:

* Campus Area Network design
* Cisco three-layer architecture
* Access, Distribution and Core layers
* VLAN configuration
* Network segmentation
* Switch connectivity
* Basic network security
* Console access
* Remote device management
* SSH concepts
* Network documentation
* Cisco Packet Tracer simulation
