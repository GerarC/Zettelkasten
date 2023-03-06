---
reference: 
- "[[ITNs07A Password Guidelines]]"
- "[[ITNs07B Password Configuration]]"
- "[[ITNs07C Encrypt Passwords]]"
- "[[ITNs07D Banner Messages]]"
date: 23/02/2023
type: 1 #evergreen
topics: Networking, Cisco
alias: ITN07, Secure Cisco Device Access, Password, Encrypt, Banner
tags: network, cisco
code: ITN07
---
# ITN07 Secure Cisco Device Access

To limit who access to the [[ITN00B Intermediary Device|Networking Device]] yo need to set a password to the all the available accessing modes since [[ITN05 User EXEC Mode|User EXEC]] until remote [[ITN04C Cisco Device Access Methods|Access Methods]]. ^1

A good password must have more than eight chars, use a combination of lower and uppercase letters, numbers and special chars; and do not use common words. Also you shouldn't use the same password for all devices. ^2

# ITN07/1 Securing Console Access

To secure the [[ITN04C Cisco Device Access Methods|Console]] access to the you have to configure the [[ITN05C Subconfiguration Mode#^1|Line]] console 0, this line represents the first, and usually the only, console interface. To secure it just enter to the line subconfiguration mode and use the `password <password>` command, after it, use the `login` command to enable the access. ^3

**Example**
~~~ bash
# In configuration mode
line console 0
password PASSWORD
login
~~~

# ITN07/2 Securing Enable Mode

[[ITN05A Privileged EXEC Mode|Privileged EXEC Mode]] is the most important mode that an administrator has to protect with a password. To protect it you have to enter to enable mode and enter the `enable secret <password>` command. ^4

# INT07/3 Securing SSH Access

To secure remote access through *SSH* you have to protect the first 16 *VTY* [[ITN05C Subconfiguration Mode#^1|Line]]. Use `line vty 0 15` command in [[ITN05B Global Configuration Mode|Global Config Mode]] to access to this subconfiguration mode so you can use `password <password>` command to set the password and `login` to enable accessing through it. ^5

**Example**
~~~ bash
# In global configuration mode
line vty 0 15
password PASSWORD
login
~~~

# ITN07/4 Password Encryption

All the *Configuration* can be viewed showing the [[ITN08 Running Configuration|Running Configuration]] even the [[ITN07 Secure Cisco Device Access#ITN07 Secure Cisco Device Access|Passwords]] in plain text, to hide passwords, you can encrypt them using the `passsword-encryption` command. ^6

# ITN07/5 Banner Messages

Having a **Banner** is a good way to declaring only authorized personnel should access to the device, It could seem useless, but some legal system don't allow prosecution, or monitoring of users unless a notification is visible. ^7

`banner motd # <message> #` [[ITN05B Global Configuration Mode|Global Config]] command is used to create a banner message when you access to the Cisco [[ITN00B Intermediary Device|Networking Device]]. The '#' is a delimiting character, can be any symbol as long as it doesn't be in the message. ^7

# Links
<<[[ITN06 Network Device Name|ITN06]]|[[ITN08 Running Configuration|ITN08]]>>