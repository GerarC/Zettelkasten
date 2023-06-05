---
title: Introduction to Networking
date: 07/03/2023
source: lesson 3.6
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs13B Protocol Data Units

## **Reference**
Introduction to Networking, Cisco; Lesson 3.6.

## **Quote**
> As application data is passed down the protocol stack on its way to be transmitted across the network media, various protocol information is added at each level. This is known as the encapsulation process.

> The form that a piece of data takes at any layer is called a protocol data unit (PDU). During encapsulation, each succeeding layer encapsulates the PDU that it receives from the layer above in accordance with the protocol being used. At each stage of the process, a PDU has a different name to reflect its new functions. Although there is no universal naming convention for PDUs, in this course, the PDUs are named according to the protocols of the TCP/IP suite.

![[Pasted image 20230306122816.png]]

## **Summary**
Protocol Data Unit:
- Protocol information is added to data passing down the protocol stack.
- This is named encapsulation process.
- The form that a data piece takes at a layer is called a **Protocol Data Unit** or **PDU**.
- Each layer encapsulates the PDU it receives in accordance with the protocol being used.
- PDU has a different name at each layer, reflecting its new funtions.
- The name of the PDU are Transport Segment, IP packet and Data link frame.