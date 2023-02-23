---
title: Introduction to Networking
date: 18/02/2023
source: lesson 2.1
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs04D Access Methods

## **Reference**
Introduction to Networking, Cisco; Lesson 2.1.

## **Quote**
> |**Method**|**Description**|
|:--------:|:------------- |
|**Console**|This is a physical management port that provides out-of-band access to a Cisco device. Out-of-band access refers to access via a dedicated management channel that is used for device maintenance purposes only. The advantage of using a console port is that the device is accessible even if no networking services are configured, such as performing the initial configuration. A computer running terminal emulation software and a special console cable to connect to the device are required for a console connection.|
|**Secure Shell (SSH)**|SSH is an in-band and recommended method for remotely establishing a secure CLI connection, through a virtual interface, over a network. Unlike a console connection, SSH connections require active networking services on the device, including an active interface configured with an address. Most versions of Cisco IOS include an SSH server and an SSH client that can be used to establish SSH sessions with other devices.|
|**Telnet**|Telnet is an insecure, in-band method of remotely establishing a CLI session, through a virtual interface, over a network. Unlike SSH, Telnet does not provide a secure, encrypted connection and should only be used in a lab environment. User authentication, passwords, and commands are sent over the network in plaintext. The best practice is to use SSH instead of Telnet. Cisco IOS includes both a Telnet server and Telnet client.|

> **Note:** Some devices, such as routers, may also support a legacy auxiliary port that was used to establish a CLI session remotely over a telephone connection using a modem. Similar to a console connection, the AUX port is out-of-band and does not require networking services to be configured or available.

## **Summary**
There are some method to access to a *Network device*, through the *Console* connecting the network device directly to a *PC*, using *SSH* to access through the network, it requires the network has some pre-configurations though, there are more, but nowadays are obsolete.