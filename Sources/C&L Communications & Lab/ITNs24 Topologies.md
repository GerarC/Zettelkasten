---
title: Introduction to Networking
date: 07/03/2023
source: lesson 6.2
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs24 Topologies

## **Reference**
Introduction to Networking, Cisco; Lesson 3.2.

## **Quote**
> The topology of a network is the arrangement, or the relationship, of the network devices and the interconnections between them.
> 
> There are two types of topologies used when describing LAN and WAN networks:
> 
> -   **Physical topology** – Identifies the physical connections and how end devices and intermediary devices (i.e, routers, switches, and wireless access points) are interconnected. The topology may also include specific device location such as room number and location on the equipment rack. Physical topologies are usually point-to-point or star.
> -   **Logical topology** - Refers to the way a network transfers frames from one node to the next. This topology identifies virtual connections using device interfaces and Layer 3 IP addressing schemes.
> 
> The data link layer "sees" the logical topology of a network when controlling data access to the media. It is the logical topology that influences the type of network framing and media access control used.
> 
> ## Point-to-Point WAN Topology
> Physical point-to-point topologies directly connect two nodes, as shown in the figure. In this arrangement, two nodes do not have to share the media with other hosts. Additionally, when using a serial communications protocol such as Point-to-Point Protocol (PPP), a node does not have to make any determination about whether an incoming frame is destined for it or another node. Therefore, the logical data link protocols can be very simple, as all frames on the media can only travel to or from the two nodes. The node places the frames on the media at one end and those frames are taken from the media by the node at the other end of the point-to-point circuit.
> 
> **Note**: A point-to-point connection over Ethernet requires the device to determine if the incoming frame is destined for this node.
> 
> A source and destination node may be indirectly connected to each other over some geographical distance using multiple intermediary devices. However, the use of physical devices in the network does not affect the logical topology, as illustrated in the figure. In the figure, adding intermediary physical connections may not change the logical topology. The logical point-to-point connection is the same.
> 
> ## LAN Topologies
> In multiaccess LANs, end devices (i.e., nodes) are interconnected using star or extended star topologies, as shown in the figure. In this type of topology, end devices are connected to a central intermediary device, in this case, an Ethernet switch. An **extended star** extends this topology by interconnecting multiple Ethernet switches. The star and extended topologies are easy to install, very scalable (easy to add and remove end devices), and easy to troubleshoot. Early star topologies interconnected end devices using Ethernet hubs.
> 
> At times there may be only two devices connected on the Ethernet LAN. An example is two interconnected routers. This would be an example of Ethernet used on a point-to-point topology.
> 
> **Legacy LAN Topologies**
> 
> Early Ethernet and legacy Token Ring LAN technologies included two other types of topologies:
> 
> -   **Bus** - All end systems are chained to each other and terminated in some form on each end. Infrastructure devices such as switches are not required to interconnect the end devices. Legacy Ethernet networks were often bus topologies using coax cables because it was inexpensive and easy to set up.
> -   **Ring** - End systems are connected to their respective neighbor forming a ring. The ring does not need to be terminated, unlike in the bus topology. Legacy Fiber Distributed Data Interface (FDDI) and Token Ring networks used ring topologies.

## **Summary**
Point-to-Point WAN Topology:
- It directly connects two nodes.
- two nodes don't have to share the media with other host.
- Using Point to Point Protocol or PPP, a node doesn't have to determinate about if an incoming frame is destined for it or another node.
- as all frames only travel to or from the two nodes, this protocol is very simple.
- The use of physical devices in the network doesn't affect the logical topology, i.e.,, the logical Point to Point connection is the same.

LAN Topologies:
- In multiconnected LANs, end devices are interconnected using star or extended star topologies.
- In this type of topologies, host are connected to a central network device.
- star and extended star are easy to install, very scalable, and easy to troubleshoot.
- At times could be only two devices, then is more a Point to Point topolody.
- Old topologies were: Bus, token ring, and ring.