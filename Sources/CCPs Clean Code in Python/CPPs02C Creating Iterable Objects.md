---
title: Clean code in Python
date: 31/01/2023
source: [chapter 2, pages: [98, 101]]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: unfinished, programming, python, pythonic_code, iterable
---
# CPPs02C Creating Iterable Objects

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Pages \[98, 101\].

## **Quote** 
> When we try to iterate an object, Python will call the `iter()` function over it. One of the first things this function checks for is the presence of the `__iter__` method on that object, which, if present, will be executed. *Page 98*

> Here, the for loop is starting a new iteration over our object. At this point, Python will call the `iter()` function on it, which in turn will call the `__iter__` magic method. On this method, it is defined to return self, indicating that the object is an iterable itself, so at that point every step of the loop will call the `next()` function on that object, which delegates to the `__next__` method. In this method, we decide how to produce the elements and return one at a time. When there is nothing else to produce, we have to signal this to Python by raising the `StopIteration` exception. *Page 99*

> This example works, but it has a small problem—once exhausted, the iterable will continue to be empty, hence raising `StopIteration`. This means that if we use this on two or more consecutive `for` loops, only the first one will work, while the second one will be empty *Page 100*

> can make `__iter__` use a generator (which are iterator objects), which is being created every time *Page 101*

## **Summary**