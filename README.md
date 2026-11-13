# VTP, VLAN Trunking & Inter-VLAN Routing Lab

## Project Overview

This project demonstrates the implementation of VLAN Trunking Protocol (VTP), IEEE 802.1Q trunking, and Router-on-a-Stick (ROAS) Inter-VLAN Routing using Cisco Packet Tracer.

The network represents a three-floor company environment for TechSolutions Inc., where departments are separated into different VLANs to improve network organization and management.

## Objectives

- Configure VLANs for different departments.
- Implement VTP Server, Client, and Transparent modes.
- Configure IEEE 802.1Q trunk links between switches.
- Implement Router-on-a-Stick using router subinterfaces.
- Enable communication between different VLANs.
- Verify network connectivity and troubleshoot Layer 2 and Layer 3 issues.

## Network Design

The network contains four switches and one router.

| Device | VTP Mode | Role |
|---|---|---|
| Switch0 | Server | Central VLAN management |
| Switch1 | Client | Receives VLAN information |
| Switch2 | Transparent | Maintains a local VLAN database |
| Switch3 | Client | Receives VLAN information |
| Router0 | N/A | Inter-VLAN routing |

## VLAN and IP Addressing Plan

| Department | VLAN ID | Devices | Network | Default Gateway |
|---|---:|---|---|---|
| Sales | 10 | PC0, PC4 | 192.168.10.0/24 | 192.168.10.1 |
| Marketing | 20 | PC5, PC2 | 192.168.20.0/24 | 192.168.20.1 |
| IT Support | 30 | PC1, PC3 | 192.168.30.0/24 | 192.168.30.1 |

## Technologies and Concepts

- Cisco Packet Tracer
- Virtual LANs (VLANs)
- VLAN Trunking Protocol (VTP)
- VTP Server, Client and Transparent Modes
- IEEE 802.1Q Trunking
- Router-on-a-Stick (ROAS)
- Inter-VLAN Routing
- IPv4 Addressing
- ICMP Connectivity Testing
- Network Troubleshooting

## Implementation Tasks

1. Configure the VTP domain and operating modes on the switches.
2. Create VLANs 10, 20 and 30 on the VTP Server.
3. Configure trunk links between interconnected switches.
4. Verify VLAN propagation to the VTP Client switches.
5. Configure the required local VLANs on the Transparent switch.
6. Configure Router0 subinterfaces using 802.1Q encapsulation.
7. Assign IP addresses and default gateways to PCs.
8. Test communication within and between VLANs.

## Verification Commands

```bash
show vtp status
show vlan brief
show interfaces trunk
show ip interface brief
show running-config
```

Connectivity testing:

```bash
ping 192.168.10.1
ping 192.168.20.1
ping 192.168.30.1
```

## Important Learning Outcomes

- Understand how VTP distributes VLAN information between switches.
- Understand the differences between VTP Server, Client and Transparent modes.
- Learn how trunk links carry traffic from multiple VLANs.
- Understand how 802.1Q tagging identifies VLAN traffic.
- Configure router subinterfaces for Inter-VLAN communication.
- Develop Layer 2 and Layer 3 troubleshooting skills.

## Repository Contents

- Cisco Packet Tracer topology file
- Network configuration screenshots
- Connectivity test screenshots
- Lab documentation

## Project Status

Update this section after completing and verifying the implementation.

**Status:** In Progress

## Author

BICT Undergraduate | Networking Specialization  
University of Sri Jayewardenepura
