---
title: Introduction to Networking
date: 18/02/2023
source: lesson 2.4
source_type: course
author: Cisco
type: 2 #sourcenote
topics: Networking, University
tags: network
---
# ITNs07C Encrypt Passwords

## **Reference**
Introduction to Networking, Cisco; Lesson 2.4.

## **Quote**
> The startup-config and running-config files display most passwords in plaintext. This is a security threat because anyone can discover the passwords if they have access to these files.

> To encrypt all plaintext passwords, use the **service password-encryption** global config command as shown in the example.

> The command applies weak encryption to all unencrypted passwords. This encryption applies only to passwords in the configuration file, not to passwords as they are sent over the network. The purpose of this command is to keep unauthorized individuals from viewing passwords in the configuration file.

> Use the **show running-config** command to verify that passwords are now encrypted.

## **Summary**
If you use the `show running-config` you will see all the configuration in plaintext, even passwords, in order to avoid it just use `service password-encryption` command in global config mode to encrypt all the passwords.