---
title: Introduction to Networking
date: 18/02/2023
source: lesson 2.7
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs09C Switch Virtual Interface Configuration

## **Reference**
Introduction to Networking, Cisco; Lesson 2.7.

## **Quote**
> To access the switch remotely, an IP address and a subnet mask must be configured on the SVI. To configure an SVI on a switch, use the **interface vlan 1** global configuration command. Vlan 1 is not an actual physical interface but a virtual one. Next assign an IPv4 address using the **ip address** _ip-address subnet-mask_ interface configuration command. Finally, enable the virtual interface using the **no shutdown** interface configuration command.

> **Note**: Similar to a Windows hosts, switches configured with an IPv4 address will typically also need to have a default gateway assigned. This can be done using the **ip default-gateway** _ip-address_ global configuration command. The _ip-address_ parameter would be the IPv4 address of the local router on the network

## **Summary**
Switch Virtual Interface configuration:
- this configuration is to access switch remotely.
- An IP address and a sub-net mask must be configured.
- To Enter in the sub configuration mode of the VLAN1 Interface use `interface vlan 1` command in global configuration mode.
- Use the `ip address <ip-address> <subnet-mask>` command to set the IP and the mask.
- Used the `no shutdown` command to enable the interface.
- Vlan 1 is not a physical port but a virtual one.
- Switch needs the default gateway to use the SVI, you can set it using `ip default-gateway <ip-address` command in global configuration mode.