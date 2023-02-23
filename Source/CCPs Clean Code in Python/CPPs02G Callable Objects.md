---
title: Clean code in Python
date: 31/01/2023
source: [chapter 2, page 112]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: unfinished, programming, python, pythonic_code
---
# CPPs02G Callable Objects

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Page 112.

## **Quote** 
It is possible (and often convenient) to define objects that can act as functions. One of the most common applications for this is to create better decorators, but it's not limited to that. *Page 112*

The magic method `__call__` will be called when we try to execute our object as if it were a regular function. Every argument passed to it will be passed along to the `__call__` method. *Page 112*

The main advantage of implementing functions this way, through objects, is that objects have states, so we can save and maintain information across calls. *Page 112*

When we have an object, a statement like this `object(*args, **kwargs)` is translated in Python to `object.__call__(*args, **kwargs)`. *Page 112*

This method is useful when we want to create callable objects that will work as parameterized functions, or in some cases functions with memory. *Page 112*

## **Summary**