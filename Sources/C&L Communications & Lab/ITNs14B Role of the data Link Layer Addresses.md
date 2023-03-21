---
title: Introduction to Networking
date: 07/03/2023
source: lesson 3.7
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: unfinished, network
---
# ITNs14B Role of the data Link Layer Addresses

## **Reference**
Introduction to Networking, Cisco; Lesson 3.7.

## **Quote**
> ### Same IP Network
When the sender and receiver of the IP packet are on the same network, the data link frame is sent directly to the receiving device. On an Ethernet network, the data link addresses are known as Ethernet Media Access Control (MAC) addresses
> MAC addresses are physically embedded on the Ethernet NIC.
> -   **Source MAC address** - This is the data link address, or the Ethernet MAC address, of the device that sends the data link frame with the encapsulated IP packet. The MAC address of the Ethernet NIC of PC1 is AA-AA-AA-AA-AA-AA, written in hexadecimal notation.
> -   **Destination MAC address** - When the receiving device is on the same network as the sending device, this is the data link address of the receiving device. In this example, the destination MAC address is the MAC address of the FTP server: CC-CC-CC-CC-CC-CC, written in hexadecimal notation.

> ### Devices on a Remote Network
When the sender of the packet is on a different network from the receiver, the source and destination IP addresses will represent hosts on different networks. This will be indicated by the network portion of the IP address of the destination host.
> -   **Source IPv4 address** - The IPv4 address of the sending device, the client computer PC1: 192.168.1.110.
> -   **Destination IPv4 address** - The IPv4 address of the receiving device, the server, Web Server: 172.16.1.99.

> ### Different IP Networks
When the sender and receiver of the IP packet are on different networks, the Ethernet data link frame cannot be sent directly to the destination host because the host is not directly reachable in the network of the sender. The Ethernet frame must be sent to another device known as the router or default gateway.
> -   **Source MAC address** - The Ethernet MAC address of the sending device, PC1. The MAC address of the Ethernet interface of PC1 is AA-AA-AA-AA-AA-AA.
> -   **Destination MAC address** - When the receiving device, the destination IP address, is on a different network from the sending device, the sending device uses the Ethernet MAC address of the default gateway or router.
> It is important that the IP address of the default gateway be configured on each host on the local network. All packets to a destination on remote networks are sent to the default gateway. Ethernet MAC addresses and the default gateway are discussed in more detail in other modules.

## **Summary**
<!-- try to apply the method of the question and the answer, if there is more than one idea, then make a single note or sub note from each idea -->