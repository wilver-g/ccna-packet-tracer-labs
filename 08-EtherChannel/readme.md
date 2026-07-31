# EtherChannel

EtherChannel is a Layer 2 or Layer 3 technology that combines multiple physical Ethernet links into a single logical interface called a **Port-Channel**. By bundling links together, EtherChannel increases available bandwidth, provides link redundancy, and simplifies network management while allowing Spanning Tree Protocol (STP) to treat multiple links as one logical connection.

In enterprise networks, EtherChannel is commonly deployed between access, distribution, and core switches to improve network resiliency and scalability without introducing Layer 2 loops.

This section contains hands-on Cisco Packet Tracer labs covering Layer 2 EtherChannel, Layer 3 EtherChannel, and EtherChannel trunk links using **Link Aggregation Control Protocol (LACP)**.

---

# Topics Covered

- Layer 2 EtherChannel
- Layer 3 EtherChannel
- Layer 2 EtherChannel Trunk
- Link Aggregation Control Protocol (LACP)
- Port-Channel Interfaces
- Layer 2 vs Layer 3 EtherChannel
- EtherChannel Verification and Troubleshooting
- Enterprise EtherChannel Deployments

---

# Lab Progression

| Lab | Description |
|------|-------------|
| **01 - Layer2-EtherChannel** | Configure a basic Layer 2 EtherChannel using LACP between two switches and observe how STP treats the Port-Channel as a single logical interface. |
| **02 - Layer3-EtherChannel** | Configure a routed EtherChannel by converting physical switchports into Layer 3 interfaces using `no switchport`. |
| **03 - Layer2-EtherChannel-Trunk** | Configure a Layer 2 EtherChannel trunk carrying multiple VLANs between an access switch and a multilayer switch. |

---

# EtherChannel Formation Methods

Cisco switches support three methods of forming an EtherChannel.

| Method | Standard | Modes | Description |
|---------|----------|-------|-------------|
| Static EtherChannel | None | `on` | Manual configuration without negotiation. Both sides must be configured identically. |
| PAgP | Cisco Proprietary | `desirable`, `auto` | Cisco's proprietary negotiation protocol for EtherChannel formation. |
| **LACP** | **IEEE 802.3ad / IEEE 802.1AX** | **active**, **passive** | Open standard protocol and the preferred choice for modern enterprise networks. |

Although all three methods are capable of forming an EtherChannel, **LACP** is the most widely deployed because it supports interoperability between different networking vendors and automatically negotiates the Port-Channel.

---

# Why EtherChannel?

EtherChannel offers several advantages over multiple independent links:

- Increased aggregate bandwidth
- Link redundancy and automatic failover
- Load balancing across bundled interfaces
- Simplified Spanning Tree topology
- Easier management through a single logical interface
- Scalable uplinks between network devices

Rather than forwarding traffic across individual physical links, switches view the entire bundle as one Port-Channel interface.

---

# Common Enterprise Deployments

EtherChannel is widely used throughout enterprise and data center networks, including:

- Access Switch ↔ Distribution Switch
- Distribution Switch ↔ Core Switch
- Core Switch ↔ Core Switch
- Multilayer Switch ↔ Multilayer Switch
- Switch ↔ Virtualization Hosts
- Switch ↔ Storage Networks

Layer 2 EtherChannels are commonly configured as trunk links carrying multiple VLANs, while Layer 3 EtherChannels are used for routed connections between Layer 3 devices.

---

# Skills Demonstrated

By completing the labs in this section, I practiced:

- Configuring Layer 2 EtherChannels
- Configuring Layer 3 EtherChannels
- Building LACP Port-Channels
- Configuring EtherChannel trunk links
- Verifying Port-Channel operation
- Understanding STP interaction with EtherChannel
- Comparing Layer 2 and Layer 3 EtherChannels
- Applying EtherChannel concepts to enterprise network designs

---

# Learning Outcome

After completing this section, I gained practical experience in deploying EtherChannel using LACP across multiple scenarios. These labs demonstrate how link aggregation improves bandwidth, redundancy, and network scalability while integrating with technologies such as VLANs, trunking, inter-VLAN routing, and Spanning Tree Protocol.