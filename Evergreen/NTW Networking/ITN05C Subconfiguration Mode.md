---
reference:
- "[[ITNs05A Configuration Mode and Subconfiguration Modes]]"
- "[[ITNs05B Navigate Between IOS Modes]]"
date: 23/02/2023
type: 1 #evergreen
topics: Networking
alias: ITN05C, Subconfiguration Mode
tags: network, cisco
code: ITN05C
---
# ITN05C Subconfiguration Mode

Line submode is used to configure [[ITN04C Cisco Device Access Methods|Access Methods]] like by Console, SSH, Telnet and etc, it's symbolized by `(config-line)#` at the end of the prompt. To access to this mode use `line <type> <number>` command [[ITN05B Global Configuration Mode|Global Config Mode]] and to exit use `exit` command or if you want to move to the [[ITN05A Privileged EXEC Mode|Privileged EXEC Mode]] `end` command. ^1

Interface submode is used to configure switch ports and router network interfaces, it's symbolized by a `(config-if)#` at the end of the prompt. To access to this mode use `interface <type> <number>` command in global configuration mode and to exit use the same commands used with [[#^1|Line config mode]]. ^2

# Links
<<[[ITN05B Global Configuration Mode|ITN05B]]|[[ITN06 Network Device Name|ITN06]]>>