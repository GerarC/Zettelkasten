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
# ITNs07 Device Names

## **Reference**
Introduction to Networking, Cisco; Lesson 2.4.

## **Quote**
> By default, all devices are assigned a factory default name. For example, a Cisco IOS switch is "Switch."

> The problem is if all switches in a network were left with their default names, it would be difficult to identify a specific device. For instance, how would you know that you are connected to the right device when accessing it remotely using SSH? The hostname provides confirmation that you are connected to the correct device.

> The default name should be changed to something more descriptive. By choosing names wisely, it is easier to remember, document, and identify network devices. Here are some important naming guidelines for hosts:
> -   Start with a letter
> -   Contain no spaces
> -   End with a letter or digit
> -   Use only letters, digits, and dashes
> -   Be less than 64 characters in length

> An organization must choose a naming convention that makes it easy and intuitive to identify a specific device. The hostnames used in the device IOS preserve capitalization and lowercase characters. For example, the figure shows that three switches, spanning three different floors, are interconnected together in a network. The naming convention that was used incorporated the location and the purpose of each device. Network documentation should explain how these names were chosen so additional devices can be named accordingly.

> The diagram shows three interconnected switches spanning three floors. The top switch is named Sw-Floor-3, the middle switch is named Sw-Floor-2, and the bottom switch is name Sw-Floor-1. A user sitting at a host PC is connected to the Sw-Floor-1 switch. Text at bottom reads: when network devices are named, they are easy to identify for configuration purposes.

> When the naming convention has been identified, the next step is to use the CLI to apply the names to the devices.

> From global configuration mode, enter the command **hostname** followed by the name of the switch and press **Enter**.

> **Note**: To return the switch to the default prompt, use the **no hostname** global config command.

## **Summary**
The *Network device* name can be changed in order to avoid confusions at the moment of configure it through *SSH* and other ways, this name have to start with a letter, contain no spaces, end with a letter or digit, use only letters, digits and dashes; and measure less than 64 chars. To choose the name the organization often choose a convention that usually use a reference to the physical position of the device and the type of device

To rename a Cisco device in *global configuration mode* use the `hostname <new_name>`  command, if you want to erased the chosen name just use `no hostname` command.