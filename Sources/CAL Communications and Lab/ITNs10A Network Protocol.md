---
title: Introduction to Networking
date: 07/03/2023
source: lesson 3.2
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs10A Network Protocol

## **Reference**
Introduction to Networking, Cisco; Lesson 3.2.

## **Quote**
> You know that for end devices to be able to communicate over a network, each device must abide by the same set of rules. These rules are called protocols and they have many functions in a network.

> Network protocols define a common format and set of rules for exchanging messages between devices. Protocols are implemented by end devices and intermediary devices in software, hardware, or both. Each network protocol has its own function, format, and rules for communications.

> |**Protocol Type**|**Description**|
|:-:|:--|
|**Network Communications Protocols**|Protocols enable two or more devices to communicate over one or more networks. The Ethernet family of technologies involves a variety of protocols such as IP, Transmission Control Protocol (TCP), HyperText Transfer Protocol (HTTP), and many more.|
|**Network Security Protocols**|Protocols secure data to provide authentication, data integrity, and data encryption. Examples of secure protocols include Secure Shell (SSH), Secure Sockets Layer (SSL), and Transport Layer Security (TLS).|
|**Routing Protocols**|Protocols enable routers to exchange route information, compare path information, and then to select the best path to the destination network. Examples of routing protocols include Open Shortest Path First (OSPF) and Border Gateway Protocol (BGP).|
|**Service Discovery Protocols**|Protocols are used for the automatic detection of devices or services. Examples of service discovery protocols include Dynamic Host Configuration Protocol (DHCP) which discovers services for IP address allocation, and Domain Name System (DNS) which is used to perform name-to-IP address translation.|

> ## Network Protocol Functions
Computers and network devices use agreed-upon protocols to communicate. The table lists the functions of these protocols.

> |**Function**|**Description**|
|:-:|:-|
|**Addressing**|This identifies the sender and the intended receiver of the message using a defined addressing scheme. Examples of protocols that provide addressing include Ethernet, IPv4, and IPv6.|
|**Reliability**|This function provides guaranteed delivery mechanisms in case messages are lost or corrupted in transit. TCP provides guaranteed delivery.|
|**Flow control**|This function ensures that data flows at an efficient rate between two communicating devices. TCP provides flow control services.|
|**Sequencing**|This function uniquely labels each transmitted segment of data. The receiving device uses the sequencing information to reassemble the information correctly. This is useful if the data segments are lost, delayed or received out-of-order. TCP provides sequencing services.|
|**Error Detection**|This function is used to determine if data became corrupted during transmission. Various protocols that provide error detection include Ethernet, IPv4, IPv6, and TCP.|
|**Application Interface**|This function contains information used for process-to-process communications between network applications. For example, when accessing a web page, HTTP or HTTPS protocols are used to communicate between the client and server web processes.|

## **Summary**
**Network Protocols:**
- define a common format and rules to exchange messages.
- these are implemented by end and intermediary devices through the software, hardware or sometimes both.
- each protocol has its function, format and rules.


**Type of protocols:**
- network communications protocols (*TCP*, *HTTP*, *IP*,...).
- network security protocols (*SSH*, SSL, TLS...).
- routing protocols (BGP, *OSPF*).
- service discovery protocols.

**Network Protocol Functions:**
- Addressing (IPv4, IPv6).
- Reliability (TCP).
- Flow Control (TCP again).
- Sequencing (TCP again).
- Error Detection (Ethernet, IPv4, IPv6).
- Application Interface (HTTP, HTTPS).