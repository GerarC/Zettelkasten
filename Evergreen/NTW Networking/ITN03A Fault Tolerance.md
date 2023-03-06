---
reference: "[[ITNs03A Fault Tolerance]]"
date: 23/02/2023
type: 1 #evergreen
topics: Networking
alias: ITN03A, Fault Tolerance
tags: network
code: ITN03A
---
# ITN03A Fault Tolerance

A **Fault Tolerant** network is which limits affected devices during a failure and it's build to be of quick recovery. These characteristics depends on multiple paths between source and destination, in other words, redundancy. If any links fails, there should be other paths to send data.

Other way to implement redundancy is the *Packet Switching*, it means to split traffic in various packets, each packet has information about the source and the destination. [[ITN00B Intermediary Device|Routers]] can direct each packet over different pathways depending on the state of the network's state.

# Links
<<[[ITN03 Network Reliability|ITN03]]|[[ITN03B Scalability|ITN03B]]>>

**Related notes:**
- [[ITN00 Host|End Devices]]
- [[ITN03 Network Reliability|Network Reliability]]