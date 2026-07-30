# Spanning Tree Protocol (STP)

This directory contains my Cisco Packet Tracer labs covering **Spanning Tree Protocol (STP)**, one of the core Layer 2 technologies used in enterprise networks to prevent switching loops while maintaining redundancy.

Throughout these labs, I explored how STP builds a loop-free topology, elects a Root Bridge, optimizes host connectivity using PortFast, and protects access ports with BPDU Guard. Each lab focuses on a practical concept commonly encountered in enterprise environments.

---

# Learning Objectives

Through these labs, I will:

- Understand why Spanning Tree Protocol is required in Layer 2 networks.
- Observe how STP prevents switching loops.
- Learn how the Root Bridge is elected.
- Understand how changing the Root Bridge affects the forwarding topology.
- Configure PortFast on access ports.
- Configure BPDU Guard to protect PortFast-enabled interfaces.
- Verify STP operation using Cisco IOS commands.
- Observe how STP responds to topology changes.

---

# Labs

| Lab | Description |
|------|-------------|
| **01 - STP Loop Prevention** | Introduces STP by demonstrating how it prevents Layer 2 loops in a redundant switched topology. |
| **02 - Root Bridge Election** | Explores how STP elects the Root Bridge and how manually changing the Root Bridge affects forwarding paths. |
| **03 - PortFast** | Demonstrates how PortFast allows end devices to begin forwarding traffic immediately without waiting for STP convergence. |
| **04 - BPDU Guard** | Shows how BPDU Guard protects PortFast-enabled access ports by placing them into an err-disabled state when BPDUs are received. |

---

# Skills Practiced

- Spanning Tree Protocol (STP)
- Root Bridge Election
- Bridge Priority Configuration
- PortFast Configuration
- BPDU Guard Configuration
- STP Verification
- STP Failover Observation
- Layer 2 Redundancy
- Cisco IOS Troubleshooting Commands

---

# Common Verification Commands

```cisco
show spanning-tree

show spanning-tree summary

show spanning-tree interface

show interfaces status

show running-config
```

---

# Key Takeaways

After completing this section, I was able to:

- Explain why Layer 2 loops occur and how STP prevents them.
- Identify the Root Bridge and understand its role in calculating a loop-free topology.
- Observe how changing the Root Bridge changes the active forwarding path.
- Configure PortFast to improve end-device connectivity.
- Configure BPDU Guard to protect access ports from unauthorized switch connections.
- Verify STP operation using Cisco IOS commands and Packet Tracer Simulation Mode.

---

# Repository Structure

```text
06-STP
│
├── 01-STP Loop Prevention
├── 02-Root Bridge Election
├── 03-PortFast
├── 04-BPDU Guard
└── README.md
```

---

# What's Next?

The next section of this repository focuses on **EtherChannel**.

While STP prevents Layer 2 loops by blocking redundant links, EtherChannel allows multiple physical links to be bundled into a single logical interface. This provides both increased bandwidth and redundancy while allowing STP to treat the bundled links as one logical path.

This progression builds naturally from Layer 2 loop prevention to efficient utilization of redundant links in enterprise networks.