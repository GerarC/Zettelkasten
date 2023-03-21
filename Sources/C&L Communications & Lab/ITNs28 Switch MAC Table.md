---
title: Introduction to Networking
date: 07/03/2023
source: lesson 7.3
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: unfinished, network
---
# ITNs28 Switch MAC Table

## **Reference**
<!-- Where do you got it -->

## **Quote**
> ## Switch Fundamentals
> Now that you know all about Ethernet MAC addresses, it is time to talk about how a switch uses these addresses to forward (or discard) frames to other devices on a network. If a switch just forwarded every frame it received out all ports, your network would be so congested that it would probably come to a complete halt.
> 
> A Layer 2 Ethernet switch uses Layer 2 MAC addresses to make forwarding decisions. It is completely unaware of the data (protocol) being carried in the data portion of the frame, such as an IPv4 packet, an ARP message, or an IPv6 ND packet. The switch makes its forwarding decisions based solely on the Layer 2 Ethernet MAC addresses.
> 
> An Ethernet switch examines its MAC address table to make a forwarding decision for each frame, unlike legacy Ethernet hubs that repeat bits out all ports except the incoming port. In the figure, the four-port switch was just powered on. The table shows the MAC Address Table which has not yet learned the MAC addresses for the four attached PCs.
> 
> **Note**: MAC addresses are shortened throughout this topic for demonstration purposes.
> 
> 
> **Note**: The MAC address table is sometimes referred to as a content addressable memory (CAM) table. While the term CAM table is fairly common, for the purposes of this course, we will refer to it as a MAC address table.
> 
> ## Switch Learning and Forwarding
> 
> The switch dynamically builds the MAC address table by examining the source MAC address of the frames received on a port.  The switch forwards frames by searching for a match between the destination MAC address in the frame and an entry in the MAC address table.
> 
> 
> ### Learn
> **Examine the Source MAC Address**
> 
> Every frame that enters a switch is checked for new information to learn. It does this by examining the source MAC address of the frame and the port number where the frame entered the switch. If the source MAC address does not exist, it is added to the table along with the incoming port number. If the source MAC address does exist, the switch updates the refresh timer for that entry in the table. By default, most Ethernet switches keep an entry in the table for 5 minutes.
> 
> In the figure for example, PC-A is sending an Ethernet frame to PC-D. The table shows the switch adds the MAC address for PC-A to the MAC Address Table.
> 
> **Note**: If the source MAC address does exist in the table but on a different port, the switch treats this as a new entry. The entry is replaced using the same MAC address but with the more current port number.
> 
> ### Forward
> **Find the Destination MAC Address**
> 
> If the destination MAC address is a unicast address, the switch will look for a match between the destination MAC address of the frame and an entry in its MAC address table. If the destination MAC address is in the table, it will forward the frame out the specified port. If the destination MAC address is not in the table, the switch will forward the frame out all ports except the incoming port. This is called an unknown unicast.
> 
> As shown in the figure, the switch does not have the destination MAC address in its table for PC-D, so it sends the frame out all ports except port 1.
> 
> **Note**: If the destination MAC address is a broadcast or a multicast, the frame is also flooded out all ports except the incoming port.
> 
> ## Filtering Frames
> 
> As a switch receives frames from different devices, it is able to populate its MAC address table by examining the source MAC address of every frame. When the MAC address table of the switch contains the destination MAC address, it is able to filter the frame and forward out a single port.
> 
> ## MAC Address Tables on Connected Switches
> A switch can have multiple MAC addresses associated with a single port. This is common when the switch is connected to another switch. The switch will have a separate MAC address table entry for each frame received with a different source MAC address.
> 
> ## Sending the Frame to the Default Gateway
> When a device has an IP address that is on a remote network, the Ethernet frame cannot be sent directly to the destination device. Instead, the Ethernet frame is sent to the MAC address of the default gateway, the router.

## **Summary**
<!-- try to apply the method of the question and the answer, if there is more than one idea, then make a single note or sub note from each idea -->