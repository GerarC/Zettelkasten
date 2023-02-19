---
title: Clean code in Python
date: 31/01/2023
source: [chapter 2, pages: [118, 119]]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: unfinished, programming, python, pythonic_code
---
# CPPs03 Mutable Default Arguments

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Pages \[87, 91\].

## **Quote** 
Simply put, don't use mutable objects as the default arguments of functions. If you use mutable objects as default arguments, you will get results that are not the expected ones. *Page 118* 

The explanation is simple—by assigning the dictionary with the default data to `user_metadata` on the definition of the function, this dictionary is actually created once and the variable `user_metadata` points to it. The body of the function modifies this object, which remains alive in memory so long as the program is running. When we pass a value to it, this will take the place of the default argument we just created. When we don't want this object it is called again, and it has been modified since the previous run; the next time we run it, will not contain the keys since they were removed on the previous call. *Page 119*

The fix is also simple—we need to use `None` as a default sentinel value and assign the default on the body of the function. Because each function has its own scope and life cycle, `user_metadata` will be assigned to the dictionary every time None appears *Page 119*

## **Summary**