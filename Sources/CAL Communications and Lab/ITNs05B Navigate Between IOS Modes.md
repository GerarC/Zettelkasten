---
title: Introduction to Networking
date: 18/02/2023
source: lesson 2.2
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: unfinished, network, university
---
# ITNs05B Navigate Between IOS Modes

## **Reference**
Introduction to Networking, Cisco; Lesson 2.2.

## **Quote**
Various commands are used to move in and out of command prompts. To move from user EXEC mode to privileged EXEC mode, use the **enable** command. Use the **disable** privileged EXEC mode command to return to user EXEC mode.

**Note**: Privileged EXEC mode is sometimes called _enable mode_.

To move in and out of global configuration mode, use the **configure terminal** privileged EXEC mode command. To return to the privileged EXEC mode, enter the **exit** global config mode command.

There are many different subconfiguration modes. For example, to enter line subconfiguration mode, you use the **line** command followed by the management line type and number you wish to access.
To move from any subconfiguration mode of the global configuration mode to the mode one step above it in the hierarchy of modes, enter the **exit** command.

To move from any subconfiguration mode to the privileged EXEC mode, enter the **end** command or enter the key combination **Ctrl+Z**.

## **Summary**
<!-- Resume of the idea with the context of the quote. -->
