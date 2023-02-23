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
# ITNs08A Alter the Running configuration

## **Reference**
Introduction to Networking, Cisco; Lesson 2.5.

## **Quote**
> If changes made to the running config do not have the desired effect and the running-config has not yet been saved, you can restore the device to its previous configuration. Remove the changed commands individually, or reload the device using the **reload** privileged EXEC mode command to restore the startup-config.

> The downside to using the **reload** command to remove an unsaved running config is the brief amount of time the device will be offline, causing network downtime.

> When a reload is initiated, the IOS will detect that the running config has changes that were not saved to the startup configuration. A prompt will appear to ask whether to save the changes.

> Alternatively, if undesired changes were saved to the startup config, it may be necessary to clear all the configurations. This requires erasing the startup config and restarting the device. The startup config is removed by using the **erase startup-config** privileged EXEC mode command.

## **Summary**
Reload the *configuration*
- using `reload` command in *privileged EXEC mode*.
- but after using the command the *device* will be offline for a while. will be offline for a while.
- will ask about saving the changes of the running config.


Delete the *startup configuration*
- using `erase startup-config` command in *Privileged EXEC mode* and restart the device.
- use it if you have saved undesired configurations. 