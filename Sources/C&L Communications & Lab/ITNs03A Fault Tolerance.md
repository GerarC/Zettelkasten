---
title: Introduction to Networking
date: 18/02/2023
source: lesson 1.6
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs03A Fault Tolerance

## **Reference**
Introduction to Networking, Cisco; Lesson 1.6.

## **Quote**
> A fault tolerant network is one that limits the number of affected devices during a failure. It is built to allow quick recovery when such a failure occurs. These networks depend on multiple paths between the source and destination of a message. If one path fails, the messages are instantly sent over a different link. Having multiple paths to a destination is known as redundancy.

> Implementing a packet-switched network is one way that reliable networks provide redundancy. Packet switching splits traffic into packets that are routed over a shared network. A single message, such as an email or a video stream, is broken into multiple message blocks, called packets. Each packet has the necessary addressing information of the source and destination of the message. The routers within the network switch the packets based on the condition of the network at that moment. This means that all the packets in a single message could take very different paths to the same destination.

## **Summary**
A network that limits affected devices and during a failure and it's built to allow quick recovery is a network that has **Fault Tolerance**. A network with this characteristic depends on multiple paths between source and destination, i.e., redundancy, If the any link fails, then there are other paths to send data.

Other way to implement redundancy is the packet switching, it splits traffic in various packets, each packet has information about the source and the destination. Routers can direct each packet in a different pathway depending on the state of the network.