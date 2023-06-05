---
title: Introduction to Networking
date: 07/03/2023
source: lesson 5.1
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs21 Binary System

## **Reference**
Introduction to Networking, Cisco; Lesson 3.2.

## **Quote**
> ## Binary and IPv4 Addresses
> Binary is important for us to understand because hosts, servers, and network devices use binary addressing. Specifically, they use binary IPv4 addresses,
> 
> Each address consists of a string of 32 bits, divided into four sections called octets. Each octet contains 8 bits (or 1 byte) separated with a dot. For example, PC1 in the figure is assigned IPv4 address 11000000.10101000.00001010.00001010. Its default gateway address would be that of R1 Gigabit Ethernet interface 11000000.10101000.00001010.00000001.
> 
> Binary works well with hosts and network devices. However, it is very challenging for humans to work with.
> 
> For ease of use by people, IPv4 addresses are commonly expressed in dotted decimal notation.
> 
> ## Binary Positional Notation
> Learning to convert binary to decimal requires an understanding of positional notation. Positional notation means that a digit represents different values depending on the “position” the digit occupies in the sequence of numbers. You already know the most common numbering system, the decimal (base 10) notation system.
> 
> |Radix|10|10|10|10|
|:--|:-|:-|:-|:-|
|Position in Number|3|2|1|0|
|Calculate|(10<sup>3</sup>)|(10<sup>2</sup>)|(10<sup>1</sup>)|(10<sup>0</sup>)|
 |Position value|1000|100|10|1|
> 
> The following bullets describe each row of the table.
> -   Row 1, Radix is the number base. Decimal notation is based on 10, therefore the radix is 10.
> -   Row 2, Position in number considers the position of the decimal number starting with, from right to left, 0 (1st position), 1 (2nd position), 2 (3rd position), 3 (4th position). These numbers also represent the exponential value use to calculate the positional value in the 4th row.
> -   Row 3 calculates the positional value by taking the radix and raising it by the exponential value of its position in row 2.  
>     **Note:** n0 is = 1.
> 
> | |Thousands|Hundreds|Tens|Ones|
|:-|:-|:-|:-|:-|
|Positional Value|1000|100|10|1|
|Decimal Number (1234)|1|2|3|4|
|Calculate|1 x 1000|2 x 100|3 x 10|4 x 1|
|Add them up…|1000|+ 200|+ 30|+ 4|
|**Result**|**1,234**|
> 
> In contrast, the binary positional notation operates as described in the table.
> 
>|Radix|2|2|2|2|2|2|2|2|
|:-|:-|:-|:-|:-|:-|:-|:-|:-|
|Position in Number|7|6|5|4|3|2|1|0|
|Calculate|(2<sup>7</sup>)|(2<sup>6</sup>)|(2<sup>5</sup>)|(2<sup>4</sup>)|(2<sup>3</sup>)|(2<sup>2</sup>)|(2<sup>1</sup>)|(2<sup>0</sup>)|
|Position value|128|64|32|16|8|4|2|1|

## **Summary**
Binary System for IPV4:
- As IPv4 IP's below are represented by binary numbers, it's necessary to know how it works.
- To convert a binary number into a decimal number you just need to know the positional notation of the binary numbers.
- The positional notation means that the rightest one equals $2^0 = 1$, the second at the right equals to $2^1 = 2$, the third to $2^2 = 4$ and so on.
- As IPv4 use the Dotted notation then you just need to worry about binary numbers with 8 bits length. 