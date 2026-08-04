# Layer 2 Security Labs

This directory contains hands-on Cisco Packet Tracer labs covering common **Layer 2 security technologies** used to protect enterprise access networks. These labs demonstrate how Cisco switches mitigate threats such as unauthorized network access, rogue DHCP servers, ARP spoofing, and MAC address violations.

Each lab focuses on a specific security feature and includes step-by-step configuration, verification commands, and practical demonstrations of how the feature behaves under normal and attack scenarios.

---

# Topics Covered

| Lab | Description |
|------|-------------|
| DHCP Snooping | Protects the network against rogue DHCP servers by allowing DHCP replies only on trusted interfaces. |
| Dynamic ARP Inspection (DAI) | Prevents ARP spoofing attacks by validating ARP packets against the DHCP Snooping binding table. |
| Port Security | Restricts switch port access based on MAC addresses using static, sticky, and secure MAC learning. |

---

# Learning Objectives

After completing these labs, I was able to:

- Configure Layer 2 security features on Cisco switches.
- Protect access networks from common Layer 2 attacks.
- Configure trusted and untrusted interfaces.
- Verify security features using Cisco IOS commands.
- Understand how multiple Layer 2 security mechanisms work together to secure enterprise networks.

---

# Enterprise Relevance

Layer 2 attacks often originate from within the local network and can bypass traditional perimeter security devices. Cisco access switches provide several security mechanisms that help mitigate these threats before they impact end users.

The technologies demonstrated in this directory are commonly deployed in enterprise environments to:

- Prevent rogue DHCP servers from assigning malicious IP configurations.
- Protect hosts from ARP spoofing and man-in-the-middle attacks.
- Restrict unauthorized devices from connecting to switch access ports.
- Improve overall security at the network edge.

---

# Lab Progression

The labs are organized in the following order:

```text
Layer2-Security
│
├── DHCP-Snooping
├── Dynamic-ARP-Inspection
└── Port-Security
```

Each lab builds upon the previous one where applicable. For example:

- **Dynamic ARP Inspection** relies on the DHCP Snooping binding table.
- **Port Security** provides an additional layer of protection by restricting which devices may connect to an access port.

---

# Technologies Used

- Cisco Catalyst Switches
- Cisco IOS
- Cisco Packet Tracer
- DHCP Snooping
- Dynamic ARP Inspection (DAI)
- Port Security
- Sticky MAC Address Learning

---

# Repository Structure

```text
Layer2-Security/
├── DHCP-Snooping/
├── Dynamic-ARP-Inspection/
└── Port-Security/
```

---

# Notes

Some Layer 2 attacks, such as true ARP poisoning or MAC spoofing, cannot be fully simulated in Cisco Packet Tracer due to platform limitations. Where applicable, the labs focus on accurate configuration, verification, and demonstrating the expected behavior of the security features while noting these limitations.

---

# Skills Demonstrated

- Cisco IOS configuration
- Switch security hardening
- Layer 2 attack mitigation
- DHCP Snooping deployment
- Dynamic ARP Inspection deployment
- Port Security configuration
- IOS verification and troubleshooting
- Enterprise access layer security

---

# Files

- `README.md`
- `DHCP-Snooping/`
- `Dynamic-ARP-Inspection/`
- `Port-Security/`