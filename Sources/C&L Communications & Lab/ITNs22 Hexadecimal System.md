---
title: Introduction to Networking
date: 07/03/2023
source: lesson 5.2
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: unfinished, network
---
# ITNs22 Hexadecimal System

## **Reference**
<!-- Where do you got it -->

## **Quote**
> Just as decimal is a base ten number system, hexadecimal is a base sixteen system. The base sixteen number system uses the digits 0 to 9 and the letters A to F. The figure shows the equivalent decimal and hexadecimal values for binary 0000 to 1111.
> 
> ![[Pasted image 20230319170900.png]]
> 
> Binary and hexadecimal work well together because it is easier to express a value as a single hexadecimal digit than as four binary bits.
> 
> The hexadecimal numbering system is used in networking to represent IP Version 6 addresses and Ethernet MAC addresses.
> 
> Pv6 addresses are 128 bits in length and every 4 bits is represented by a single hexadecimal digit; for a total of 32 hexadecimal values. IPv6 addresses are not case-sensitive and can be written in either lowercase or uppercase.
> 
> the preferred format for writing an IPv6 address is x:x:x:x:x:x:x:x, with each “x” consisting of four hexadecimal values. When referring to 8 bits of an IPv4 address we use the term octet. In IPv6, a _hextet_ is the unofficial term used to refer to a segment of 16 bits or four hexadecimal values.
> 
> 
> ## Decimal to Hexadecimal Conversions
> Converting decimal numbers to hexadecimal values is straightforward. Follow the steps listed:
> 
> 1.  Convert the decimal number to 8-bit binary strings.
> 2.  Divide the binary strings in groups of four starting from the rightmost position.
> 3.  Convert each four binary numbers into their equivalent hexadecimal digit.
> 
> The example provides the steps for converting **168** to hexadecimal.
> 
> For example, **168** converted into hex using the three-step process.
> 
> 1.  **168** in binary is **10101000**.
> 2.  **10101000** in two groups of four binary digits is **1010** and **1000**.
> 3.  **1010**is hex **A** and **1000** is hex **8**.
> 
> ## Hexadecimal to Decimal Conversion
> Converting hexadecimal numbers to decimal values is also straightforward. Follow the steps listed:
> 
> 1.  Convert the hexadecimal number to 4-bit binary strings.
> 2.  Create 8-bit binary grouping starting from the rightmost position.
> 3.  Convert each 8-bit binary grouping into their equivalent decimal digit.
> 
> This example provides the steps for converting **D2** to decimal.
> 
> 1.  **D2** in 4-bit binary strings is **1101** and **0010**.
> 2.  **1101** and **0010** is **11010010** in an 8-bit grouping.
> 3.  **11010010** in binary is equivalent to **210** in decimal.

## **Summary**
<!-- try to apply the method of the question and the answer, if there is more than one idea, then make a single note or sub note from each idea -->