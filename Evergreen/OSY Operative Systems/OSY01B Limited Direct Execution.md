---
reference: "[[Operating Systems: Three Easy Pieces]]"
date: 22/08/2023
type: 1 #evergreen
alias: OSY01B, Limited Direct Execution
tags: operative_system
code: OSY01B
---
# OSY01B Limited Direct Execution

Any [[OSY00 Operative System|OS]] must limit the execution of the process in favor of security, stability and efficiency, to realize that the [[OSY00A Kernel|Kernel]] uses the **Limited Direct Execution** which is a Technic to limit the CPU usage from the process. These technics are:
- have two modes: a user mode and one privileged
- User processes use user mode and require a [[System Call]] to **trap** into the Kernel to request OS operations.
- When OS finishes the request It returns the program from trap, which reduces privileges.
- The **Trap Table** must be set up at boot time by the OS and Cannot be modified by the user processes.
- When a program is running the OS must have hardware mechanisms to to interrupt the program anytime, i.e, [[Timer Interrupt]].
- Sometimes the OS would wish change from the current process to another during a [[Timer Interrupt]] or a [[System Call]], this is known as **Context Switcher**^1

# Links
<<[[OSY01A Time Sharing|OSY01A]]|[[]]>>

**Related notes:**
- [[]] 