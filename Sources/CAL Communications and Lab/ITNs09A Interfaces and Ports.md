---
title: Introduction to Networking
date: 18/02/2023
source: lesson 2.6
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs09A Interfaces and Ports

## **Reference**
Introduction to Networking, Cisco; Lesson 2.6.

## **Quote**
> Network communications depend on end user device interfaces, networking device interfaces, and the cables that connect them. Each physical interface has specifications, or standards, that define it. A cable connecting to the interface must be designed to match the physical standards of the interface.

> Cisco IOS Layer 2 switches have physical ports for devices to connect. These ports do not support Layer 3 IP addresses. Therefore, switches have one or more switch virtual interfaces (SVIs). These are virtual interfaces because there is no physical hardware on the device associated with it. An SVI is created in software.

> The virtual interface lets you remotely manage a switch over a network using IPv4 and IPv6. Each switch comes with one SVI appearing in the default configuration "out-of-the-box." The default SVI is interface VLAN1.

> **Note**: A Layer 2 switch does not need an IP address. The IP address assigned to the SVI is used to remotely access the switch. An IP address is not necessary for the switch to perform its operations.

## **Summary**

interface:
- Each physical interface has specifications or standards that define it.

Switch Virtual Interface:
- The Cisco switches don't support IP address.
- Have one or more switch virtual interfaces.
- Are virtual 'cause there is not a physical port.
- SVI are created by the software.
- Lets to connect remotely using IPv4 or IPv6.
- Default SVI is interface VLAN1.
- A switch doesn't need a IP to work, the SVI IP is just to configure.

