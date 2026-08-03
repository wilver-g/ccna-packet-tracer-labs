# HSRP (Hot Standby Router Protocol)

## Overview

This directory contains Cisco Packet Tracer labs demonstrating **Hot Standby Router Protocol (HSRP)**, Cisco's First Hop Redundancy Protocol (FHRP) that provides gateway redundancy for end devices.

HSRP allows multiple routers to present a **single virtual default gateway**. One router actively forwards traffic while another remains on standby, ready to take over automatically if the active router fails. This minimizes downtime and ensures continuous network connectivity.

## Topics Covered

* HSRP operation
* Active and Standby router roles
* Virtual IP and Virtual MAC address
* HSRP priority
* Preemption
* Failover process
* Gateway redundancy
* Basic HSRP verification and troubleshooting

## Labs

| Lab                               | Description                                                                                                                        |
| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| **01 - Basic HSRP Configuration** | Configure HSRP between two routers, verify Active/Standby roles, and observe automatic failover during a simulated router failure. |

## Learning Objectives

After completing these labs, you should be able to:

* Configure HSRP on Cisco routers
* Assign a virtual IP address for hosts
* Modify HSRP priorities
* Enable preemption
* Verify HSRP status using IOS commands
* Observe seamless gateway failover
* Troubleshoot common HSRP configuration issues

## Verification Commands

```text
show standby
show standby brief
show running-config
show ip interface brief
```

## Skills Practiced

* First Hop Redundancy Protocols (FHRP)
* Gateway redundancy
* High availability
* Network resiliency
* Cisco IOS configuration
* Network troubleshooting
