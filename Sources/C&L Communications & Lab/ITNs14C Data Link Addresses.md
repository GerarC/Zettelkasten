---
title: Introduction to Networking
date: 07/03/2023
source: lesson 3.7
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs14C Data Link Addresses

## **Reference**
Introduction to Networking, Cisco; Lesson 3.7.

## **Quote**
> The data link Layer 2 physical address has a different role. The purpose of the data link address is to deliver the data link frame from one network interface to another network interface on the same network.

> Before an IP packet can be sent over a wired or wireless network, it must be encapsulated in a data link frame, so it can be transmitted over the physical medium.

> As the IP packet travels from host-to-router, router-to-router, and finally router-to-host, at each point along the way the IP packet is encapsulated in a new data link frame. Each data link frame contains the source data link address of the NIC card sending the frame, and the destination data link address of the NIC card receiving the frame.

> The Layer 2, data link protocol is only used to deliver the packet from NIC-to-NIC on the same network. The router removes the Layer 2 information as it is received on one NIC and adds new data link information before forwarding out the exit NIC on its way towards the final destination.

> The IP packet is encapsulated in a data link frame that contains the following data link information:
> -   **Source data link address** - The physical address of the NIC that is sending the data link frame.
> -   **Destination data link address** - The physical address of the NIC that is receiving the data link frame. This address is either the next hop router or the address of the final destination device.

## **Summary**
Data Link Addresses:
	- The purpose of this type of addresses is to deliver data link frame from one NIC to another NIC on the same network.
	- Before an IP packet can be sent through media, it must be encapsulated in a data link frame.
	- IP packet is encapsulated in a new data link frame in each point (device) of its way to the destination.
	- Data link protocol is only used to deliver packets NIC to NIC, so the router removes packet information and add new data link information before send it to its destination.
	- Data link frame has the physical address of the NIC that is sending the frame, and the physical address of the next hop router or the final destination.