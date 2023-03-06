---
reference: "[[ITNs07 Device Names]]"
date: 23/02/2023
type: 1 #evergreen
topics: Networking
alias: ITN06, Network Device Name, Device Name
tags: network, cisco
code: ITN06
---
# ITN06 Network Device Name

The **[[ITN00B Intermediary Device|Networking Device]] Name** can be changed in order to avoid confusions at the moment of configure it through *SSH* and other ways. ^1

This name must start with a letter, contain no spaces, end with a letter or digit, use only letters, digits and dashes; and measure less than 64 chars. To choose the name the organization often choose a convention that usually use a reference to the physical position of the device and the type of device. ^2

To rename a Cisco device in [[ITN05B Global Configuration Mode|Global Configuration Mode]] use the `hostname <new_name>` command, if you want to erase the chosen name use `no hostname` command. ^3

**Example**
~~~ bash
enable
conf term
hosname PASSWORD
~~~

# Links
<<[[ITN05C Subconfiguration Mode|ITN05C]]|[[ITN07 Secure Cisco Device Access|ITN07]]>>

**Related notes:**
- [[ITN04C Cisco Device Access Methods|Access Methods]] 
- [[ITN01A Physical Topology Diagram|Physical Topology Diagram]]