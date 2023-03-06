---
reference:
- "[[ITNs08 Configuration Files]]"
- "[[ITNs08A Alter the Running configuration]]"
date: 23/02/2023
type: 1 #evergreen
topics: Networking
alias: ITN08A, Startup Configuration, Startup Config
tags: network, cisco
code: ITN08A
---
# ITN08A Startup Configuration

**Startup Configuration** is the configuration saved in NVRAM (the permanent memory) and is loaded in RAM as the [[ITN08 Running Configuration|Running Config]] when the [[ITN00B Intermediary Device|Device]] is turned on.

If you have some undesired configurations, use `erase startup-config` command in [[ITN05A Privileged EXEC Mode|Privileged EXEC Mode]] and restart the configuration.

# Links
<<[[ITN08 Running Configuration|ITN08]]|[[ITN08B Capture Configuration to a Text File|ITN08B]]>>