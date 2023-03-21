---
title: Introduction to Networking
date: 07/03/2023
source: lesson 7.1
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: unfinished, network
---
# ITNs26 Ethernet Frame

## **Reference**
<!-- Where do you got it -->

## **Quote**
> ## Ethernet Encapsulation
> Ethernet operates in the data link layer and the physical layer. It is a family of networking technologies defined in the IEEE 802.2 and 802.3 standards. Ethernet supports data bandwidths of the following:
> 
> -   10 Mbps
> -   100 Mbps
> -   1000 Mbps (1 Gbps)
> -   10,000 Mbps (10 Gbps)
> -   40,000 Mbps (40 Gbps)
> -   100,000 Mbps (100 Gbps)
> 
> 
> ## Data Link Sublayers
> 
> IEEE 802 LAN/MAN protocols, including Ethernet, use the following two separate sublayers of the data link layer to operate. They are the Logical Link Control (LLC) and the Media Access Control (MAC), as shown in the figure.
> 
> Recall that LLC and MAC have the following roles in the data link layer:
> 
> -   **LLC Sublayer** - This IEEE 802.2 sublayer communicates between the networking software at the upper layers and the device hardware at the lower layers. It places information in the frame that identifies which network layer protocol is being used for the frame. This information allows multiple Layer 3 protocols, such as IPv4 and IPv6, to use the same network interface and media.
> -   **MAC Sublayer** - This sublayer (IEEE 802.3, 802.11, or 802.15 for example) is implemented in hardware and is responsible for data encapsulation and media access control. It provides data link layer addressing and is integrated with various physical layer technologies.
> 
> ## MAC Sublayer
> The MAC sublayer is responsible for data encapsulation and accessing the media.
> 
> **Data Encapsulation**
> 
> IEEE 802.3 data encapsulation includes the following:
> 
> -   **Ethernet frame** - This is the internal structure of the Ethernet frame.
> -   **Ethernet Addressing** - The Ethernet frame includes both a source and destination MAC address to deliver the Ethernet frame from Ethernet NIC to Ethernet NIC on the same LAN.
> -   **Ethernet Error detection** - The Ethernet frame includes a frame check sequence (FCS) trailer used for error detection.
> 
> **Accessing the Media**
> 
> As shown in the figure, the IEEE 802.3 MAC sublayer includes the specifications for different Ethernet communications standards over various types of media including copper and fiber.
> 
> The diagram is showing various Ethernet standards in the MAC sublayer. At the top of the diagram is the network layer and the network layer protocol. Below that is the data link layer and its sublayers. The top sublayer is the IEEE 802.2 LLC sublayer. Next is the Ethernet IEEE 802.3 MAC sublayer. Below that are five columns with various Ethernet standards and media types that span the lower part of the MAC sublayer and the entire OSI physical layer. From left to right the columns are: IEEE 802.3u Fast Ethernet; IEEE 802.3z Gigabit Ethernet over Fiber; IEEE 802.ab Gigabit Ethernet over Copper; IEEE 802.3ae 10 Gigabit Ethernet over Fiber; and Etc.
> 
> ### Ethernet Standards in the MAC Sublayer
> ![[Pasted image 20230320174957.png]]
> Recall that legacy Ethernet using a bus topology or hubs, is a shared, half-duplex medium. Ethernet over a half-duplex medium uses a contention-based access method, carrier sense multiple access/collision detection (CSMA/CD) This ensures that only one device is transmitting at a time. CSMA/CD allows multiple devices to share the same half-duplex medium, detecting a collision when more than one device attempts to transmit simultaneously. It also provides a back-off algorithm for retransmission.
> 
> Ethernet LANs of today use switches that operate in full-duplex. Full-duplex communications with Ethernet switches do not require access control through CSMA/CD.
> 
> 
> ## Ethernet Frame Fields
> 
> The minimum Ethernet frame size is 64 bytes and the expected maximum is 1518 bytes. This includes all bytes from the destination MAC address field through the frame check sequence (FCS) field. The preamble field is not included when describing the size of the frame.
> 
> **Note**: The frame size may be larger if additional requirements are included, such as VLAN tagging. VLAN tagging is beyond the scope of this course.
> 
> Any frame less than 64 bytes in length is considered a “collision fragment” or “runt frame” and is automatically discarded by receiving stations. Frames with more than 1500 bytes of data are considered “jumbo” or “baby giant frames”.
> 
> If the size of a transmitted frame is less than the minimum, or greater than the maximum, the receiving device drops the frame. Dropped frames are likely to be the result of collisions or other unwanted signals. They are considered invalid. Jumbo frames are usually supported by most Fast Ethernet and Gigabit Ethernet switches and NICs.
> 
> The figure shows each field in the Ethernet frame. Refer to the table for more information about the function of each field.
> 
> ![[Pasted image 20230320175031.png]]
> 
> ### Ethernet Frame Fields Detail
> ![[Pasted image 20230320175101.png]]

## **Summary**
<!-- try to apply the method of the question and the answer, if there is more than one idea, then make a single note or sub note from each idea -->