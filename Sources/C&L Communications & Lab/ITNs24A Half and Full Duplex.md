---
title: Introduction to Networking
date: 07/03/2023
source: lesson 6.2
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs24A Half and Full Duplex

## **Reference**
Introduction to Networking, Cisco; Lesson 3.2.

## **Quote**
> ## Half and Full Duplex Communication
> **Half-duplex communication**
> Both devices can transmit and receive on the media but cannot do so simultaneously. WLANs and legacy bus topologies with Ethernet hubs use the half-duplex mode. Half-duplex allows only one device to send or receive at a time on the shared medium.
> 
> **Full-duplex communication**
> Both devices can simultaneously transmit and receive on the shared media. The data link layer assumes that the media is available for transmission for both nodes at any time. Ethernet switches operate in full-duplex mode by default, but they can operate in half-duplex if connecting to a device such as an Ethernet hub.
> 
> In summary, half-duplex communications restrict the exchange of data to one direction at a time. Full-duplex allows the sending and receiving of data to happen simultaneously.
> 
> It is important that two interconnected interfaces, such as a host NIC and an interface on an Ethernet switch, operate using the same duplex mode. Otherwise, there will be a duplex mismatch creating inefficiency and latency on the link.

## **Summary**
Half-duplex communication:
- Both devices can transmit and receive data, but not at the same time.
- WLANs and legacy bus with ethernet hubs use it.

Full-duplex communication:
- Both Devices can transmit and receive data at the same time.
- Layer 2 assumes that the media is available for transmission at any time.
- Switches operate in full-duplex mode by default, but can be change.
- It's important that both NICs operate using the same duplex mode.