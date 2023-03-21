---
title: Introduction to Networking
date: 07/03/2023
source: lesson 6.2
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: unfinished, network
---
# ITNs24B Access Control

## **Reference**
<!-- Where do you got it -->

## **Quote**
> ## Access Control Methods
> Ethernet LANs and WLANs are examples of multiaccess networks. A multiaccess network is a network that can have two or more end devices attempting to access the network simultaneously.
> 
> Some multiaccess networks require rules to govern how devices share the physical media. There are two basic access control methods for shared media:
> 
> -   Contention-based access
> -   Controlled access
> 
> **Contention-based access** 
> 
> In contention-based multiaccess networks, all nodes are operating in half-duplex, competing for the use of the medium. However, only one device can send at a time. Therefore, there is a process if more than one device transmits at the same time. Examples of contention-based access methods include the following:
> 
> -   Carrier sense multiple access with collision detection (CSMA/CD) used on legacy bus-topology Ethernet LANs
> -   Carrier sense multiple access with collision avoidance (CSMA/CA) used on Wireless LANs
> 
> **Controlled access**
> 
> In a controlled-based multiaccess network, each node has its own time to use the medium. These deterministic types of legacy networks are inefficient because a device must wait its turn to access the medium. Examples of multiaccess networks that use controlled access include the following:
> 
> -   Legacy Token Ring
> -   Legacy ARCNET
> 
> **Note**: Today, Ethernet networks operate in full-duplex and do not require an access method.
> 
> ## Contention-Based Access - CSMA/CD
> Examples of contention-based access networks include the following:
> 
> -   Wireless LAN (uses CSMA/CA)
> -   Legacy bus-topology Ethernet LAN (uses CSMA/CD)
> -   Legacy Ethernet LAN using a hub (uses CSMA/CD)
> 
> These networks operate in half-duplex mode, meaning only one device can send or receive at a time. This requires a process to govern when a device can send and what happens when multiple devices send at the same time.
> 
> If two devices transmit at the same time, a collision will occur. For legacy Ethernet LANs, both devices will detect the collision on the network. This is the collision detection (CD) portion of CSMA/CD. The NIC compares data transmitted with data received, or by recognizing that the signal amplitude is higher than normal on the media. The data sent by both devices will be corrupted and will need to be resent.
> 
> ## Contention-Based Access - CSMA/CA
> Another form of CSMA used by IEEE 802.11 WLANs is carrier sense multiple access/collision avoidance (CSMA/CA).
> 
> CMSA/CA uses a method similar to CSMA/CD to detect if the media is clear. CMSA/CA uses additional techniques. In wireless environments it may not be possible for a device to detect a collision. CMSA/CA does not detect collisions but attempts to avoid them by waiting before transmitting. Each device that transmits includes the time duration that it needs for the transmission. All other wireless devices receive this information and know how long the medium will be unavailable.
> 
> After a wireless device sends an 802.11 frame, the receiver returns an acknowledgment so that the sender knows the frame arrived.
> 
> Whether it is an Ethernet LAN using hubs, or a WLAN, contention-based systems do not scale well under heavy media use.
> 
> **Note**: Ethernet LANs using switches do not use a contention-based system because the switch and the host NIC operate in full-duplex mode.

## **Summary**
<!-- try to apply the method of the question and the answer, if there is more than one idea, then make a single note or sub note from each idea -->