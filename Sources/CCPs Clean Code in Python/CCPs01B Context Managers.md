---
title: Clean code in Python
date: 22/01/2023
source: [chapter 2, pages: [77, 80]]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: programming, python, pythonic_code
---
# CCPs01B Context Managers

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Pages \[77, 80\].

## **Quote** 
> Context managers are a distinctively useful feature that Python provides. The reason why they are so useful is that they correctly respond to a pattern. The pattern is actually every situation where we want to run some code, and has preconditions and postconditions, meaning that we want to run things before and after a certain main action.  Most of the time, we see context managers around resource management. For example, on situations when we open files, we want to make sure that they are closed after processing (so we do not leak file descriptors), or if we open a connection to a service (or even a socket), we also want to be sure to close it accordingly, or when removing temporary files, and so on. *Page 77*

> Context managers consist of two magic methods: `__enter__` and `__exit__`. On the first line of the context manager, the with statement will call the first method, `__enter__`, and whatever this method returns will be assigned to the variable labeled after `as`. This is optional—we don't really need to return anything specific on the `__enter__` method, and even if we do, there is still no strict reason to assign it to a variable if it is not required. *page 78*

> As a general rule, it should be good practice (although not mandatory), to always return something on the `__enter__`. *page 80*

## **Summary**
Python has a good feature name context managers, this managers follow the pattern where we want to run a part of code that has preconditions and postconditions, The most of the time we use context managers for the resource management, Or if we open any connection to a service or socket and want to close it correctly.

The context managers work based on two methods: `__enter__` and `__exit__`. When you init a context manager with the special word `with` it calls to the `__enter__` method and this does the stuff and returns an object that you can label with the work `as` and then the code enter in the context. Finally, when the code in the context is passed, the manager calls `__exit__` method and it manage any error that could occur.

It should be a good practice return something on the `__enter__` method, although it isn't mandatory and even if it returns something, there is no reason yet to label it with `as`.