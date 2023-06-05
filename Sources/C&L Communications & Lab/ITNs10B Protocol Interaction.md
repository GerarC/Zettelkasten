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
# ITNs10B Protocol Interaction

## **Reference**
Introduction to Networking, Cisco; Lesson 3.2.

## **Quote**
> A message sent over a computer network typically requires the use of several protocols, each one with its own functions and format.

> - **Hypertext Transfer Protocol (HTTP) -** This protocol governs the way a web server and a web client interact. HTTP defines the content and formatting of the requests and responses that are exchanged between the client and server. Both the client and the web server software implement HTTP as part of the application. HTTP relies on other protocols to govern how the messages are transported between the client and server.
> - **Transmission Control Protocol (TCP) -** This protocol manages the individual conversations. TCP is responsible for guaranteeing the reliable delivery of the information and managing flow control between the end devices.
> - **Internet Protocol (IP) -** This protocol is responsible for delivering messages from the sender to the receiver. IP is used by routers to forward the messages across multiple networks.
> - **Ethernet -** This protocol is responsible for the delivery of messages from one NIC to another NIC on the same Ethernet local area network (LAN).

## **Summary**
Interaction between protocols:
- Each message sent over a network requires some protocols.
- These protocols are: HTTP, TCP, IP and Ethernet.
- The first one defines content and formatting of the request and responses.
- The second manages the individual conversations between devices.
- IP is the one who responds for delivering messages from the source to the destiny.
- The last one looks for delivering from one NIC to other NIC on the same LAN.