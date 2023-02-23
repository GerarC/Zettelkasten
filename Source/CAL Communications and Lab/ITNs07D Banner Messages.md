---
title: Introduction to Networking
date: 18/02/2023
source: lesson 2.4
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs07D Banner Messages

## **Reference**
Introduction to Networking, Cisco; Lesson 2.4.

## **Quote**
> Although requiring passwords is one way to keep unauthorized personnel out of a network, it is vital to provide a method for declaring that only authorized personnel should attempt to access the device. To do this, add a banner to the device output. Banners can be an important part of the legal process in the event that someone is prosecuted for breaking into a device. Some legal systems do not allow prosecution, or even the monitoring of users, unless a notification is visible.

> To create a banner message of the day on a network device, use the **banner motd #** _the message of the day_ **#** global config command. The “#” in the command syntax is called the delimiting character. It is entered before and after the message. The delimiting character can be any character as long as it does not occur in the message. For this reason, symbols such as the "#" are often used. After the command is executed, the banner will be displayed on all subsequent attempts to access the device until the banner is removed.

## **Summary**
have a Banner is a good way to declaring only authorized personnel should access to the device, It could seem useless, but some legal system don't allow prosecution, or monitoring of users unless a notification is visible.

the `banner motd # message #` global config command is used for create a banner message. the "#" is a delimiting character, can be any symbol as long as it doesn't be in the message. 