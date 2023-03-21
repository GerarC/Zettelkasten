---
title: Introduction to Networking
date: 07/03/2023
source: lesson 6.1
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: unfinished, network
---
# ITNs23 Data Link Layer

## **Reference**
<!-- Where do you got it -->

## **Quote**
> ## The Data Link Layer
> The data link layer of the OSI model (Layer 2), as shown in the figure, prepares network data for the physical network. The data link layer is responsible for network interface card (NIC) to network interface card communications. The data link layer does the following:
> 
> -   Enables upper layers to access the media. The upper layer protocol is completely unaware of the type of media that is used to forward the data.
> -   Accepts data, usually Layer 3 packets (i.e., IPv4 or IPv6), and encapsulates them into Layer 2 frames.
> -   Controls how data is placed and received on the media.
> -   Exchanges frames between endpoints over the network media.
> -   Receives encapsulated data, usually Layer 3 packets, and directs them to the proper upper-layer protocol.
> -   Performs error detection and rejects any corrupt frame.
> 
> In computer networks, a node is a device that can receive, create, store, or forward data along a communications path. A node can be either an end device such as a laptop or mobile phone, or an intermediary device such as an Ethernet switch.
> 
> Without the data link layer, network layer protocols such as IP, would have to make provisions for connecting to every type of media that could exist along a delivery path. Additionally, every time a new network technology or medium was developed IP, would have to adapt.
> 
> ## IEEE 802 LAN/MAN Data Link Sublayers
> 
> IEEE 802 LAN/MAN standards are specific to Ethernet LANs, wireless LANs (WLAN), wireless personal area networks (WPAN) and other types of local and metropolitan area networks. The IEEE 802 LAN/MAN data link layer consists of the following two sublayers:
> -   **Logical Link Control (LLC)** - This IEEE 802.2 sublayer communicates between the networking software at the upper layers and the device hardware at the lower layers. It places information in the frame that identifies which network layer protocol is being used for the frame. This information allows multiple Layer 3 protocols, such as IPv4 and IPv6, to use the same network interface and media.
> -   **Media Access Control (MAC)** – Implements this sublayer (IEEE 802.3, 802.11, or 802.15) in hardware. It is responsible for data encapsulation and media access control. It provides data link layer addressing and it is integrated with various physical layer technologies.
> ![[Pasted image 20230319172653.png]]
> 
> The LLC sublayer takes the network protocol data, which is typically an IPv4 or IPv6 packet, and adds Layer 2 control information to help deliver the packet to the destination node. 
> 
> The MAC sublayer controls the NIC and other hardware that is responsible for sending and receiving data on the wired or wireless LAN/MAN medium.
> 
> The MAC sublayer provides data encapsulation:
> 
> -   **Frame delimiting** - The framing process provides important delimiters to identify fields within a frame. These delimiting bits provide synchronization between the transmitting and receiving nodes.
> -   **Addressing** - Provides source and destination addressing for transporting the Layer 2 frame between devices on the same shared medium.
> -   **Error detection** - Includes a trailer used to detect transmission errors.
> 
> The MAC sublayer also provides media access control, allowing multiple devices to communicate over a shared (half-duplex) medium. Full-duplex communications do not require access control.
> 
> ## Providing Access to Media
> Each network environment that packets encounter as they travel from a local host to a remote host can have different characteristics. For example, an Ethernet LAN usually consists of many hosts contending for access on the network medium. The MAC sublayer resolves this. With serial links the access method may only consist of a direct connection between only two devices, usually two routers. Therefore, they do not require the techniques employed by the IEEE 802 MAC sublayer.
> Router interfaces encapsulate the packet into the appropriate frame. A suitable media access control method is used to access each link. In any given exchange of network layer packets, there may be numerous data link layers and media transitions.
> 
> At each hop along the path, a router performs the following Layer 2 functions:
> 1.  Accepts a frame from a medium
> 2.  De-encapsulates the frame
> 3.  Re-encapsulates the packet into a new frame
> 4.  Forwards the new frame appropriate to the medium of that segment of the physical network
> 
> Press play to view the animation. The router in the figure has an Ethernet interface to connect to the LAN and a serial interface to connect to the WAN. As the router processes frames, it will use data link layer services to receive the frame from one medium, de-encapsulate it to the Layer 3 PDU, re-encapsulate the PDU into a new frame, and place the frame on the medium of the next link of the network.

## **Summary**
<!-- try to apply the method of the question and the answer, if there is more than one idea, then make a single note or sub note from each idea -->