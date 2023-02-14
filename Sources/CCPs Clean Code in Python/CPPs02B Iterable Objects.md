---
title: Clean code in Python
date: 31/01/2023
source: [chapter 2, page 96]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: programming, python, pythonic_code, iterable
---
# CPPs02B Iterable Objects

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Page 96.

## **Quote** 
> Iteration works in Python by its own protocol (namely the iteration protocol). When you try to iterate an object in the form `for e in myobject:`..., what Python checks at a very high level are the following two things, in order:
> - If the object contains one of the iterator methods `__next__` or `__iter__`
> -  If the object is a sequence and has `__len__` and `__getitem__` Therefore, as a fallback mechanism, sequences can be iterated, and so *Page 96*

## **Summary**