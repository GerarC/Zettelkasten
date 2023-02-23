---
title: Clean code in Python
date: 23/01/2023
source: [chapter 2, page 86]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: programming, python, pythonic_code
---
# CCPs01E Managing errors with context manager

## **Reference**
Clean code in python, Mario Anaya; Chapter 2, Page 86.

## **Quote** 
> Note that `contextlib.suppress` is a util package that enters a context manager, which, if one of the provided exceptions is raised, doesn't fail. It's similar to running that same code on a `try`/`except` block and passing an exception or logging it, but the difference is that calling the `suppress` method makes it more explicit that those exceptions that are controlled as part of our logic. *Page 86*

## **Summary**
A good way to manages Error in python is using context managers, `contextlib` module has a function to do it. `suppress` is a funct with you can swap `try` and `except`. In `suppress` you pass a type of error and inside the context put the code that can raise errors.