---
title: Introduction to Networking
date: 07/03/2023
source: lesson 3.6
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: unfinished, network
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
<!-- try to apply the method of the question and the answer, if there is more than one idea, then make a single note or sub note from each idea -->