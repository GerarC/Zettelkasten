---
title: Introduction to Networking
date: 07/03/2023
source: lesson 6.1
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs23 Data Link Layer

## **Reference**
Introduction to Networking, Cisco; Lesson 3.2.

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
Data Link Layer:
- Data link layer or Layer 2 of the OSI model is responsible for NIC to NIC communication.
- It does: Enables upper layers media access regardless of the type, Access data from the Layer 3 and encapsulates it, Controls how data is placed and received on the media, share frames between endpoints over the media, Receives encapsulated data and directs it to up and detects errors to reject any corrupt frame.
- without data link layer, layer 3 protocols, would have to make provisions to connect to each type of media and should adapt to every new media or network technology.

Logical Link Control (LLC):
- Its the IEEE 802.2 sublayer of Layer 2.
- Communicates between the sofware at the upper layers and the harware at the lower layers.
- It adds information about which layer 3 protocol is being used for the frame, this info allows multiple network layer protocols to use the same net interface and media.
- Takes network protocol data and adds layer 2 control information to help to deliver the packet.
- 

Media Access Control (MAC):
- This sublayer is in the hardware (802.3, 802.11, 802.15).
- It encapsulates the data and is responsible of Media Access Control.
- Provies Data Link Layer addressing and it's integrated with various physical layer technologies.
- 802.3 for Ethernet, 802.11 for WLAN, and 802.15 for WPAN.
- Controls the NIC and other hardware that is responsible to data sending and receiving.
- MAC encapsulation consist in three parts: Frame delimiting to identify fields within a frame. Addressing having source and destination addres for transporting the layer 2, and Error detection including a trailer.
- this sublayer also allows multiple devices to communicate over half-duplex shared medium.

Providing Access to Media:
- each environment in the Packets travel from local to a remote can have different characteristics. 
- MAC sublayer resolves the problems that it can involve.
- Routers encapsulate the packet into a frame.
- At each hop routers perform: Accepts a frame from a medium, de-encapsulates it, re-encapsulates the packet into a new frame and forwars the new frame to the medium.


