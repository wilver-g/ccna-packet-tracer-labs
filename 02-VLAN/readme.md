# VLANs (Virtual Local Area Networks)

This folder contains my Cisco Packet Tracer labs focused on **Virtual Local Area Networks (VLANs)** and related switching concepts covered in the CCNA 200-301 certification.

VLANs are one of the core technologies used in modern networks to logically segment devices into separate broadcast domains. They improve network organization, security, and scalability by allowing multiple logical networks to coexist on the same physical infrastructure.

These labs progress from basic VLAN configuration to trunking, inter-VLAN communication, and troubleshooting, providing a practical understanding of how VLANs are deployed and managed in enterprise networks.

## Labs

### 01 - Basic VLAN Configuration

Configured multiple VLANs on a single Layer 2 switch and assigned access ports to each VLAN. This lab demonstrates how VLANs logically separate devices into different broadcast domains while sharing the same physical switch.

**Topics Covered**

- VLAN Creation
- Access Ports
- Static IP Addressing
- Broadcast Domain Segmentation
- VLAN Verification

---

### 02 - VLAN Trunking (802.1Q)

Configured an IEEE 802.1Q trunk between two switches to allow multiple VLANs to traverse a single physical link. This lab demonstrates how VLANs are extended across multiple switches while maintaining logical separation.

**Topics Covered**

- IEEE 802.1Q Trunking
- Access vs Trunk Ports
- Allowed VLANs
- VLAN Extension Across Switches
- Trunk Verification

---

### 03 - Inter-VLAN Routing (Router-on-a-Stick)

Configured Router-on-a-Stick (ROAS) using router subinterfaces and an 802.1Q trunk to enable communication between multiple VLANs through a single physical router interface.

**Topics Covered**

- Router-on-a-Stick (ROAS)
- Router Subinterfaces
- IEEE 802.1Q Encapsulation
- Default Gateways
- Inter-VLAN Routing
- Routing Verification

---

### 04 - VLAN Troubleshooting

Introduced common VLAN configuration issues and followed a structured troubleshooting process to identify, isolate, and resolve each problem using Cisco IOS verification commands.

**Topics Covered**

- VLAN Troubleshooting
- Incorrect VLAN Assignments
- Trunk Misconfiguration
- Missing Router Subinterfaces
- Cisco IOS Verification Commands
- Structured Troubleshooting Methodology

---

## What I Learned

Through these labs, I developed a solid understanding of VLAN implementation and Layer 2 switching concepts used in enterprise networks.

The progression from basic VLAN configuration to trunking, Router-on-a-Stick, and troubleshooting reinforced how VLANs are created, extended across switches, and integrated with Layer 3 routing to support scalable network designs.

Each lab includes:

- Objectives
- Network topology
- Configuration snippets
- Verification screenshots
- Cisco IOS verification commands
- Key concepts learned