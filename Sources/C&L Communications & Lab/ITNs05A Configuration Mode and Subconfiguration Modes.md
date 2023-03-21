---
title: Introduction to Networking
date: 18/02/2023
source: lesson 2.2
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs05A Configuration Mode and Subconfiguration Modes

## **Reference**
Introduction to Networking, Cisco; Lesson 2.2.

## **Quote**
> To configure the device, the user must enter global configuration mode, which is commonly called global config mode.

> From global config mode, CLI configuration changes are made that affect the operation of the device as a whole. Global configuration mode is identified by a prompt that ends with (config)# after the device name, such as **Switch(config)#**.

> Global configuration mode is accessed before other specific configuration modes. From global config mode, the user can enter different subconfiguration modes. Each of these modes allows the configuration of a particular part or function of the IOS device. Two common subconfiguration modes include:

> -   **Line Configuration Mode -** Used to configure console, SSH, Telnet, or AUX access.
> -   **Interface Configuration Mode -** Used to configure a switch port or router network interface.

> When the CLI is used, the mode is identified by the command-line prompt that is unique to that mode. By default, every prompt begins with the device name. Following the name, the remainder of the prompt indicates the mode.
**Switch(config-line)#** and the default prompt for interface configuration mode is **Switch(config-if)#**.

## **Summary**
To configure Cisco devices the user have to access to the global configuration mode, this mode is identified by a prompt that ends with (config)#. It lets you enter interface and line subconfigurations.
Line submode is used to configure the access by console, SSH, Telnet and ETC. Interface submode is used to configure switch ports and router networks interfaces. A prompt that ends with (config-line)# and one with (config-if)# symbolized a line configuration mode and a interface configuration mode respectively.