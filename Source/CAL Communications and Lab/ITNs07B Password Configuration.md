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
# ITNs07B Password Configuration

## **Reference**
Introduction to Networking, Cisco; Lesson 2.4.

## **Quote**
> When you initially connect to a device, you are in user EXEC mode. This mode is secured using the console.

> To secure user EXEC mode access, enter line console configuration mode using the **line console 0** global configuration command, as shown in the example. The zero is used to represent the first (and in most cases the only) console interface. Next, specify the user EXEC mode password using the **password** _password_ command. Finally, enable user EXEC access using the **login** command.

> To have administrator access to all IOS commands including configuring a device, you must gain privileged EXEC mode access. It is the most important access method because it provides complete access to the device.

> To secure privileged EXEC access, use the **enable secret** _password_ global config command, as shown in the example.

> Virtual terminal (VTY) lines enable remote access using Telnet or SSH to the device. Many Cisco switches support up to 16 VTY lines that are numbered 0 to 15.

> To secure VTY lines, enter line VTY mode using the **line vty 0 15** global config command. Next, specify the VTY password using the **password** _password_ command. Lastly, enable VTY access using the **login** command.

## **Summary**
To secure the access to the *user EXEC mode* you have to configure the line console 0, this line represents the first, and often the only, console interface.
To secure it just enter in the line subconfiguration mode and use the `password <password>` command, after it use `login` command.

The most important mode that you have to protect with a password is the *privileged EXEC mode*, to do this you have to enter in enable mode and use the `enable secret <password>` command.

And to secure remote access through *SSH* you have to protect the first  16 *VTY* lines. Using `line vty 0 15` in global config mode you will access to their configuration, then use `password <password>` command and lastly enable the VTY access with `login` command.