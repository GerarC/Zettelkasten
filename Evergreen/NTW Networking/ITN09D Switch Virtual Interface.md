---
reference: 
- "[[ITNs09A Interfaces and Ports]]"
- "[[ITNs09C Switch Virtual Interface Configuration]]"
date: 23/02/2023
type: 1 #evergreen
topics: Networking
alias: ITN09D, Switch Virtual Interface, SVI
tags: network, cisco
code: ITN09D
---
# ITN09D Switch Virtual Interface

Since Cisco *Switches* don't support [[ITN09 IP Address|IP Address]], then have one or more **Switch Virtual Interfaces** or **SVI**. This type of interface is created by the software, it is not a physical port, it's why are called virtual. SVI lets connect either [[ITN09A IPv4|IPv4]] and [[ITN09B IPv6|IPv6]] and is configure through its default interface *VLAN1*. A switch doesn't need a IP to work, the SVI IP is just to configure it. ^1

# ITN09D/1 Configure SVI

[[#^1|SVI]] is to access switch remotely, then you must configure a [[ITN09 IP Address|IP Address]] and a *Subnet mask*, to do it enter to the VLAN1 Interface [[ITN05C Subconfiguration Mode|Subconfiguration Mode]] using `interface vlan 1` in [[ITN05B Global Configuration Mode|Global Configuration Mode]], so you can configure the IP address and the subnet mask using `ip address <ip-address> <subnet-mask>` command, next you must enable the interface using `no shutdown`. Finally, the switch needs the default gateway to be able to use SVI, set it using `ip default-gateway <ip-address>` command in Global Config Mode.

**Example:**
~~~ bash
# enter to global config mode
conf term
# enter to the specific sub mode
interface vlan 1
ip address 192.168.1.40 255.255.255.000
no shutdown
# return to global config mode
exit
ip default-gateway 192.168.1.1
~~~

# Links
<<[[ITN09C Automatic IPv4 Configuration|ITN09C]]|[[ITN09E Test Connectivity|ITN09E]]>>

**Related notes:**
- [[ITN00B Intermediary Device|Intermediary Device]]
- [[ITN09B IPv6|IPv6]]
- [[ITN09A IPv4|IPv4]]