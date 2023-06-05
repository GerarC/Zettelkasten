---
title: Introduction to Networking
date: 07/03/2023
source: lesson 4.1
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs16C Bandwidth

## **Reference**
Introduction to Networking, Cisco; Lesson 4.1.

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
Throughput is the measure of the transfer of bits across the media over a given period of time.
> 
> Due to a number of factors, throughput usually does not match the specified bandwidth in physical layer implementations. Throughput is usually lower than the bandwidth. There are many factors that influence throughput:
> -   The amount of traffic
> -   The type of traffic
> -   The latency created by the number of network devices encountered between source and destination
> There are many online speed tests that can reveal the throughput of an internet connection. The figure provides sample results from a speed test.

> **Goodput**
There is a third measurement to assess the transfer of usable data; it is known as goodput. Goodput is the measure of usable data transferred over a given period of time. Goodput is throughput minus traffic overhead for establishing sessions, acknowledgments, encapsulation, and retransmitted bits. Goodput is always lower than throughput, which is generally lower than the bandwidth.

## **Summary**
Bandwidth:
- Is the capacity at which a medium can carry data.
- Basically measures how many data can flow over a medium in a given time.
- This rate change depending of the media.
- It's measure on bits per second (bps), Kbps, Mbps and Gbps.
- The practical bandwidth of a network is determined by the properties of the media and the technologies chosen for signals.

Latency:
- It's defined as the time for data to travel from a point to another, including delays.

Throughput:
- is the real measure of the transfer of bits across the media in a given time.
- Throughput usually doesn't match with the bandwidth.
- Is usually slower to the bandwidth, influenced by the amount and type of traffic, and the latency.
- Throughput is "bottlenecked" by the lowest segment of the network and the medium throughput cannot be higher than that segment." by the lowest segment of the network and the medium throughput cannot be higher than that segment, even if the other segments are faster.

Goodput:
- It's the usable data transferred over a given time.
- Is the throughput minus the traffic.
- It's slower than the throughput that is slower than the bandwidth.