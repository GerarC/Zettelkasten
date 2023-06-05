---
title: Introduction to Networking
date: 07/03/2023
source: lesson 7.2
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs27 MAC Address

## **Reference**
Introduction to Networking, Cisco; Lesson 3.2.

## **Quote**
> ## MAC Address and Hexadecimal
> An Ethernet MAC address consists of a 48-bit binary value. Hexadecimal is used to identify an Ethernet address because a single hexadecimal digit represents four binary bits. Therefore, a 48-bit Ethernet MAC address can be expressed using only 12 hexadecimal values.
> 
> When using hexadecimal, leading zeroes are always displayed to complete the 8-bit representation. For example, in the table, the binary value 0000 1010 is shown in hexadecimal as 0A.
> 
> Hexadecimal numbers are often represented by the value preceded by **0x** (e.g., 0x73) to distinguish between decimal and hexadecimal values in documentation.
> 
> Hexadecimal may also be represented by a subscript 16, or the hex number followed by an H (e.g., 73H).
> 
> ## Ethernet MAC Address
> In an Ethernet LAN, every network device is connected to the same, shared media. The MAC address is used to identify the physical source and destination devices (NICs) on the local network segment. MAC addressing provides a method for device identification at the data link layer of the OSI model.
> 
> An Ethernet MAC address is a 48-bit address expressed using 12 hexadecimal digits, as shown in the figure. Because a byte equals 8 bits, we can also say that a MAC address is 6 bytes in length.
> 
> ![[Pasted image 20230320180200.png]]
> 
> All MAC addresses must be unique to the Ethernet device or Ethernet interface. To ensure this, all vendors that sell Ethernet devices must register with the IEEE to obtain a unique 6 hexadecimal (i.e., 24-bit or 3-byte) code called the organizationally unique identifier (OUI).
> 
> When a vendor assigns a MAC address to a device or Ethernet interface, the vendor must do as follows:
> 
> -   Use its assigned OUI as the first 6 hexadecimal digits.
> -   Assign a unique value in the last 6 hexadecimal digits.
> 
> Therefore, an Ethernet MAC address consists of a 6 hexadecimal vendor OUI code followed by a 6 hexadecimal vendor-assigned value, as shown in the figure.
> 
> ![[Pasted image 20230320180249.png]]
> 
> For example, assume that Cisco needs to assign a unique MAC address to a new device. The IEEE has assigned Cisco a OUI of **00-60-2F**. Cisco would then configure the device with a unique vendor code such as **3A-07-BC**. Therefore, the Ethernet MAC address of that device would be **00-60-2F-3A-07-BC.**
> 
> It is the responsibility of the vendor to ensure that none of its devices be assigned the same MAC address. However, it is possible for duplicate MAC addresses to exist because of mistakes made during manufacturing, mistakes made in some virtual machine implementation methods, or modifications made using one of several software tools. In any case, it will be necessary to modify the MAC address with a new NIC or make modifications via software.
> 
> ## Frame Processing
> Sometimes the MAC address is referred to as a burned-in address (BIA) because the address is hard coded into read-only memory (ROM) on the NIC. This means that the address is encoded into the ROM chip permanently.
> 
> **Note**: On modern PC operating systems and NICs, it is possible to change the MAC address in software. This is useful when attempting to gain access to a network that filters based on BIA. Consequently, filtering or controlling traffic based on the MAC address is no longer as secure.
> 
> When the computer boots up, the NIC copies its MAC address from ROM into RAM. When a device is forwarding a message to an Ethernet network, the Ethernet header includes these:
> 
> -   **Source MAC address** - This is the MAC address of the source device NIC.
> -   **Destination MAC address** - This is the MAC address of the destination device NIC.
> 
> When a NIC receives an Ethernet frame, it examines the destination MAC address to see if it matches the physical MAC address that is stored in RAM. If there is no match, the device discards the frame. If there is a match, it passes the frame up the OSI layers, where the de-encapsulation process takes place.
> 
> **Note:** Ethernet NICs will also accept frames if the destination MAC address is a broadcast or a multicast group of which the host is a member.
> 
> Any device that is the source or destination of an Ethernet frame, will have an Ethernet NIC and therefore, a MAC address. This includes workstations, servers, printers, mobile devices, and routers.
> 
> ## Unicast MAC Address
> In Ethernet, different MAC addresses are used for Layer 2 unicast, broadcast, and multicast communications.
> 
> A unicast MAC address is the unique address that is used when a frame is sent from a single transmitting device to a single destination device.
> 
> ## Broadcast MAC Address
> 
> An Ethernet broadcast frame is received and processed by every device on the Ethernet LAN. The features of an Ethernet broadcast are as follows:
> 
> -   It has a destination MAC address of FF-FF-FF-FF-FF-FF in hexadecimal (48 ones in binary).
> -   It is flooded out all Ethernet switch ports except the incoming port.
> -   It is not forwarded by a router.
> 
> If the encapsulated data is an IPv4 broadcast packet, this means the packet contains a destination IPv4 address that has all ones (1s) in the host portion. This numbering in the address means that all hosts on that local network (broadcast domain) will receive and process the packet.
> 
> n, the source host sends an IPv4 broadcast packet to all devices on its network. The IPv4 destination address is a broadcast address, 192.168.1.255. When the IPv4 broadcast packet is encapsulated in the Ethernet frame, the destination MAC address is the broadcast MAC address of FF-FF-FF-FF-FF-FF in hexadecimal (48 ones in binary).
> 
> DHCP for IPv4 is an example of a protocol that uses Ethernet and IPv4 broadcast addresses.
> 
> However, not all Ethernet broadcasts carry an IPv4 broadcast packet. For example, ARP Requests do not use IPv4, but the ARP message is sent as an Ethernet broadcast.
> 
> 
> ## Multicast MAC Address
> An Ethernet multicast frame is received and processed by a group of devices on the Ethernet LAN that belong to the same multicast group. The features of an Ethernet multicast are as follows:
> 
> -   There is a destination MAC address of 01-00-5E when the encapsulated data is an IPv4 multicast packet and a destination MAC address of 33-33 when the encapsulated data is an IPv6 multicast packet.
> -   There are other reserved multicast destination MAC addresses for when the encapsulated data is not IP, such as Spanning Tree Protocol (STP) and Link Layer Discovery Protocol (LLDP).
> -   It is flooded out all Ethernet switch ports except the incoming port, unless the switch is configured for multicast snooping.
> -   It is not forwarded by a router, unless the router is configured to route multicast packets.
> 
> If the encapsulated data is an IP multicast packet, the devices that belong to a multicast group are assigned a multicast group IP address. The range of IPv4 multicast addresses is 224.0.0.0 to 239.255.255.255. The range of IPv6 multicast addresses begins with ff00::/8. Because multicast addresses represent a group of addresses (sometimes called a host group), they can only be used as the destination of a packet. The source will always be a unicast address.
> 
> As with the unicast and broadcast addresses, the multicast IP address requires a corresponding multicast MAC address to deliver frames on a local network. The multicast MAC address is associated with, and uses addressing information from, the IPv4 or IPv6 multicast address.
> 
> Routing protocols and other network protocols use multicast addressing. Applications such as video and imaging software may also use multicast addressing, although multicast applications are not as common.

## **Summary**
MAC Address:
- An Ethernet MAC address is a 48-bit (6 bytes) value.
- it's expressed using only 12 hexadecimal values.
- Is used to identify the physical device NIC on the local segment.
- It provides a method for device identification at the data link layer.
- All MAC addresses must be unique to the Ethernet device or interface (Nowadays just need to be unique in the same network).
- Ethernet device vendors must register with the IEEE to obtain a unique 6 hexadecimal code called Organizationally Unique Identifier (OUI).
- to assign a MAC address, the vendor must: use its OUI as the first 6 hex digits and assign a unique value in the last 6.

Types of MAC addresses:
- There are some types of MAC addresses:
	- Unicast MAC address: is the unique address used when a frame is sent from a single transmitting or destination device.
	- Broadcast MAC Address: It's a MAC with all bits in 1, is flooded to all devices except the source, Its not forwarded by a router and is used as destination address when an IPv4 broadcast packets is encapsulated.
	- Multicast MAC Address: It's received and processed by a group of devices on the LAN, begins with a 01-00-5E when the upper protocol is IPv4 and 33-33 when is IPv6, It's flooded to all the LAN except the source device, and could be forward by the router if it's configured to it.