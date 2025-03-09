---
reference: "[[Operating Systems: Three Easy Pieces]]"
date: 15/08/2023
type: 1 #evergreen
alias: OSY01, Processes, Process, Program
tags: operative_system
code: OSY01
---
# OSY01 Processes

A **Process** is basically a running program, and its **Machine State** that is the description of what the program can read or update, thus **memory**, called address space; **registers** where some important registers such as **Program Counter**, and Finally the **I/O information** are part of the Machine state. ^1

The [[OSY00 Operative System|OS]] [[Virtualizates]] a CPU for each process, Making an illusion that a lot of processes are being executed at the same time ^2

A process can be in one of three states: running, ready and blocked.

Every [[OSY00 Operative System|Operative System]] needs a Process API. It lets to the user and the OS itself manage processes easily. the API must allow send the signal of some functions: **Create**, **Destroy**, put in **Wait**, **Miscellaneous Controls** of and the **Status** of the process. ^4

At the creation of the process the [[OSY00 Operative System|OS]] must load the Program's code in memory (In early OSs the loading is doing all at once, while in modern OSs is loading code blocks), then allocates a runtime's **Stack** and initialization of tasks related to **I/O**. ^5

Each [[#^1|Process]] has assigned a portion of memory where it has the **Runtime stack** and the **Heap**. In the Stack is stored local variables and in the Heap reside variables specifically allocated by the user. It's possible to these data structures collide, in actual machines is virtually impossible though. ^6

All the information about a process is saved in a Data Structure that sometimes is called **Process Control Block (PBC)**
 
# Links
<<[[OSY00 Operative System|]]|[[OSY01A Time Sharing|OSY01A]]>>

**Related notes:**
- [[]] 