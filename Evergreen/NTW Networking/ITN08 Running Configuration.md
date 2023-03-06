---
reference:
- "[[ITNs08 Configuration Files]]"
- "[[ITNs08A Alter the Running configuration]]"
date: 23/02/2023
type: 1 #evergreen
topics: Networking
alias: ITN08, Running Configuration, Running Config
tags: network, cisco
code: ITN08
---
# ITN08 Running Configuration

**Running Configuration** is the configurations on a Cisco [[ITN00B Intermediary Device|Devices]] that is running on the ram while device is on and is changed immediately when you run a configuration command. You can see all the running config using `show running config` command. ^1

To save this configuration you have to replace current [[ITN08A Startup Configuration|Startup Configuration]] using `copy running-config startup-config` in [[ITN05A Privileged EXEC Mode|privileged EXEC mode]]. ^2

If you have any error in the running configuration and you wanna recharge the [[ITN08A Startup Configuration|Startup Config]] you can use `reload` command, but there is an inconvenience with it, and it's that device will be offline for a while. ^3

# Links
<<[[ITN07 Secure Cisco Device Access|ITN07]]|[[ITN08A Startup Configuration|ITN08A]]>>