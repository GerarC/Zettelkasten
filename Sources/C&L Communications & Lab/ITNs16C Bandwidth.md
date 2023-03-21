---
title: Introduction to Networking
date: 07/03/2023
source: lesson 4.1
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: unfinished, network
---
# ITNs16C Bandwidth

## **Reference**
<!-- Where do you got it -->

## **Quote**
> ## Bandwidth
Different physical media support the transfer of bits at different rates. Data transfer is usually discussed in terms of bandwidth. Bandwidth is the capacity at which a medium can carry data. Digital bandwidth measures the amount of data that can flow from one place to another in a given amount of time. Bandwidth is typically measured in kilobits per second (kbps), megabits per second (Mbps), or gigabits per second (Gbps). Bandwidth is sometimes thought of as the speed that bits travel, however this is not accurate. For example, in both 10Mbps and 100Mbps Ethernet, the bits are sent at the speed of electricity. The difference is the number of bits that are transmitted per second.
> 
> A combination of factors determines the practical bandwidth of a network:
> -   The properties of the physical media
> -   The technologies chosen for signaling and detecting network signals
> 
> Physical media properties, current technologies, and the laws of physics all play a role in determining the available bandwidth.


> |**Unit of Bandwidth**|**Abbreviation**|**Equivalence**|
|:--|:-:|:-|
|Bits per second|bps|1 bps = fundamental unit of bandwidth|
|Kilobits per second|Kbps|1 Kbps = 1,000 bps = 10<sup>3</sup> bps|
|Megabits per second|Mbps|1 Mbps = 1,000,000 bps = 10<sup>6</sup> bps|
|Gigabits per second|Gbps|1 Gbps = 1,000,000,000 bps = 10<sup>9</sup> bps|
|Terabits per second|Tbps|1 Tbps = 1,000,000,000,000 bps = 10<sup>12</sup> bps|

> ## Bandwidth Terminology
Terms used to measure the quality of bandwidth include:
> -   Latency
> -   Throughput
> -   Goodput

> **Latency**
Latency refers to the amount of time, including delays, for data to travel from one given point to another.
> 
> In an internetwork, or a network with multiple segments, throughput cannot be faster than the slowest link in the path from source to destination. Even if all, or most, of the segments have high bandwidth, it will only take one segment in the path with low throughput to create a bottleneck in the throughput of the entire network.

> **Throughput**
There is a third measurement to assess the transfer of usable data; it is known as goodput. Goodput is the measure of usable data transferred over a given period of time. Goodput is throughput minus traffic overhead for establishing sessions, acknowledgments, encapsulation, and retransmitted bits. Goodput is always lower than throughput, which is generally lower than the bandwidth.

> **Goodput**
There is a third measurement to assess the transfer of usable data; it is known as goodput. Goodput is the measure of usable data transferred over a given period of time. Goodput is throughput minus traffic overhead for establishing sessions, acknowledgments, encapsulation, and retransmitted bits. Goodput is always lower than throughput, which is generally lower than the bandwidth.

## **Summary**
<!-- try to apply the method of the question and the answer, if there is more than one idea, then make a single note or sub note from each idea -->