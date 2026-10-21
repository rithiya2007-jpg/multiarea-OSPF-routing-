# Multi-Area OSPF Configuration

## Project Overview
This Cisco Packet Tracer lab demonstrates a multi-router network using Open Shortest Path First (OSPF) routing across multiple areas. The topology contains routers, switches, and end devices connected through LAN and point-to-point networks. The goal is to enable routing between different LANs and verify communication.

## Features
- Multi-router network topology.
- OSPF configuration using multiple areas.
- IPv4 LAN and point-to-point addressing.
- Dynamic route learning between routers.
- Connectivity verification using ping.
- Troubleshooting practice using router show commands.

## Technologies Used
- Cisco Packet Tracer — network simulation.
- Cisco IOS CLI — router configuration.
- OSPF — dynamic link-state routing protocol.
- IPv4 — network addressing and subnetting.
- ICMP — connectivity testing.

## Topology Notes
The supplied screenshot shows these labels:
- LANs: `192.168.1.0/24`, `192.168.2.0/24`, `192.168.3.0/24`
- Inter-router network labels include `10.10.10.8/30`, `11.11.11.8/30`, and `12.12.12.8/30`
- OSPF areas are marked as Area 0, Area 1, and Area 2.

## Project Structure
```text
Multi-Area-OSPF/
├── topology-screenshot.jpg
└── README.md
```

## How to Recreate and Test
1. Open Cisco Packet Tracer and recreate the topology shown in `topology-screenshot.jpg`.
2. Configure IPv4 addresses on router interfaces and PCs.
3. Enable OSPF on each router and assign the correct networks to the intended areas.
4. Ensure PC default gateways point to their local router interfaces.
5. Test connectivity between PCs using `ping`.

## Useful Verification Commands
```text
show ip interface brief
show ip ospf neighbor
show ip route ospf
show running-config
ping <destination-ip>
```

## Expected Result
When interface addressing, OSPF areas, and PC gateways are configured correctly, routers should form OSPF neighbor relationships and remote LANs should be reachable.

## Important Note
This repository contains the screenshot and documentation prepared from the supplied image. The original Cisco Packet Tracer `.pkt` file was not supplied, so the topology must be recreated in Packet Tracer. Confirm all interface names, IP addresses, subnet masks, and OSPF network statements against your actual topology before using any configuration.
