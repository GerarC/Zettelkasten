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
# ITNs13 Segmenting Messages

## **Reference**
Introduction to Networking, Cisco; Lesson 3.6.

## **Quote**
> In theory, a single communication, such as a video or an email message with many large attachments, could be sent across a network from a source to a destination as one massive, uninterrupted stream of bits. However, this would create problems for other devices needing to use the same communication channels or links.

> A better approach is to divide the data into smaller, more manageable pieces to send over the network. Segmentation is the process of dividing a stream of data into smaller units for transmissions over the network. Segmentation is necessary because data networks use the TCP/IP protocol suite send data in individual IP packets. Each packet is sent separately, similar to sending a long letter as a series of individual postcards.

> This leads to segmenting messages having two primary benefits:
> -   **Increases speed** - Because a large data stream is segmented into packets, large amounts of data can be sent over the network without tying up a communications link. This allows many different conversations to be interleaved on the network called multiplexing.
> -   **Increases efficiency** -If a single segment is fails to reach its destination due to a failure in the network or network congestion, only that segment needs to be retransmitted instead of resending the entire data stream.

## **Summary**
Message Segmentation:
- Though is possible send large messages through the media, but it isn't the better approach.
- A better way to send data is dividing data into smaller and more manageable packages. This is called segmentation.
- This is necessary because the TCP/IP suite send data in individual IP packets.
- Segmentation has mainly two benefits: Increases speed because a large packet is not using the entire media for itself letting many conversations be interleaved and Increases the efficiency because if some packet fails only those segments need to be retransmitted and not the whole message.