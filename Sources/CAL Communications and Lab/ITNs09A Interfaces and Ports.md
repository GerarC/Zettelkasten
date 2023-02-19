---
title: Introduction to Networking
date: 18/02/2023
source: lesson 2.6
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: unfinished, network, university
---
# ITNs09A Interfaces and Ports

## **Reference**
Introduction to Networking, Cisco; Lesson 2.6.

## **Quote**
Network communications depend on end user device interfaces, networking device interfaces, and the cables that connect them. Each physical interface has specifications, or standards, that define it. A cable connecting to the interface must be designed to match the physical standards of the interface.

Different types of network media have different features and benefits. Not all network media have the same characteristics. Not all media are appropriate for the same purpose. These are some of the differences between various types of media:
 -   Distance the media can successfully carry a signal
-   Environment in which the media is to be installed
-   Amount of data and the speed at which it must be transmitted
-   Cost of the media and installation

Cisco IOS Layer 2 switches have physical ports for devices to connect. These ports do not support Layer 3 IP addresses. Therefore, switches have one or more switch virtual interfaces (SVIs). These are virtual interfaces because there is no physical hardware on the device associated with it. An SVI is created in software.

The virtual interface lets you remotely manage a switch over a network using IPv4 and IPv6. Each switch comes with one SVI appearing in the default configuration "out-of-the-box." The default SVI is interface VLAN1.

**Note**: A Layer 2 switch does not need an IP address. The IP address assigned to the SVI is used to remotely access the switch. An IP address is not necessary for the switch to perform its operations.

## **Summary**
<!-- Resume of the idea with the context of the quote. -->
