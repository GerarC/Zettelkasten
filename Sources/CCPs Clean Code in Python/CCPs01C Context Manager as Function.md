---
title: Clean code in Python
date: 22/01/2023
source: [chapter 2, pages: [82, 83]]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: programming, python, pythonic_code
---
# CCPs01C Context Manager as Function

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Pages \[82, 83\].

## **Quote** 
> The `contextlib` module contains a lot of helper functions and objects to either implement context managers or use some already provided ones that can help us write more compact code. *Page 82*

> When the `contextlib.contextmanager` decorator is applied to a function, it converts the code on that function into a context manager. The function in question has to be a particular kind of function called a generator function, which will separate the statements into what is going to be on the `__enter__` and `__exit__` magic methods, respectively. *page 82*

> All we need to know is that when this decorator is applied, everything before the yield statement will be run as if it were part of the `__enter__` method. Then, the yielded value is going to be the result of the context manager evaluation (what `__enter__` would return), and what would be assigned to the variable if we chose to assign it like `as x:` *page 83*

## **Summary**
In Python, there is a module with a lot of useful utils to work with context managers, this module is `contextlib` and it contains functions and classes to implement context managers. One of them permits to convert a function in a context manager, this one helps us to write more compact code.

If you want to convert the code of a function in a context manager, just apply the `contextlib.contextmanager` decorator. The function has to be a particular type of function named `generator` function, which will separate the code into what is the part that corresponds to `__enter__` and what corresponds with `__exit__` respectively.

~~~ python
def function():
	# Code of __enter__
	yield
	# Code of __exit__
~~~

When this decorator is applied, all before `yield` statements run as if it were part of the `__enter__` method, yielded value is the object that should return `__enter__` and everything after it belong to `__exit__`.