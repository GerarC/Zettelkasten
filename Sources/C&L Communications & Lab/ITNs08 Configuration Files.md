---
title: Introduction to Networking
date: 18/02/2023
source: lesson 2.5
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs08 Configuration Files

## **Reference**
Introduction to Networking, Cisco; Lesson 2.5.

## **Quote**
> There are two system files that store the device configuration:
> -   **startup-config** - This is the saved configuration file that is stored in NVRAM. It contains all the commands that will be used by the device upon startup or reboot. Flash does not lose its contents when the device is powered off.
> -   **running-config** - This is stored in Random Access Memory (RAM). It reflects the current configuration. Modifying a running configuration affects the operation of a Cisco device immediately. RAM is volatile memory. It loses all of its content when the device is powered off or restarted.

> The **show running-config** privileged EXEC mode command is used to view the running config. As shown in the example, the command will list the complete configuration currently stored in RAM.

> To view the startup configuration file, use the **show startup-config** privileged EXEC command.

> If power to the device is lost, or if the device is restarted, all configuration changes will be lost unless they have been saved. To save changes made to the running configuration to the startup configuration file, use the **copy running-config startup-config** privileged EXEC mode command.

## **Summary**
Cisco devices have two type of configuration files, one is saved in the permanent memory (NVRAM) and other than runs in the RAM. the first is named *startup-config*, the second is named *running-config*

the startup-config is the configuration with the system inits, and the running is the actual config

To save the running-configuration use the `copy running-config startup-config` in **privileged EXEC mode**