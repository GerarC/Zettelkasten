---
reference: "[[Operating Systems: Three Easy Pieces]]"
date: 22/08/2023
type: 1 #evergreen
alias: OSY01C, Scheduling, Scheduler
tags: operative_system
code: OSY01C
---
# OSY01C Scheduling

[[OSY01B Limited Direct Execution|Limited Direct Execution]] and [[OSY01 Processes|Process Management]] at low level is fine, but these processes also require high level **Scheduling Policies (or also called disciplines)** that are used by ***Scheduler***. Using **Workload Assumptions** an scheduler can determine which process should run first and how many time can use the CPU. An important point to have in mind is the [[I/O Operations]], those can block the CPU and the Scheduler must make decisions when the I/O completes. ^1

An Scheduler can operate [[OSY01 Processes|Processes]] in different data structures, like an [[linked List]] or an [[Binary Tree]], and use different algorithms to effect all the Disciplines. ^2

# Links
<<[[OSY01B Limited Direct Execution|OSY01B]]|[[]]>>

**Related notes:**
- [[]] 