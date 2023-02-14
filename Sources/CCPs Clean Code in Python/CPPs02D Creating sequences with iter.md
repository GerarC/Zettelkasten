---
title: Clean code in Python
date: 31/01/2023
source: [chapter 2, page 103]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: programming, python, pythonic_code, iterable
---
# CPPs02D Creating sequences with iter

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Page 103.

## **Quote** 
Maybe our object does not define the `__iter__()` method, but we still want to be able to iterate over it. If `__iter__` is not defined on the object, the `iter()` function will look for the presence of `__getitem__`, and if this is not found, it will raise `TypeError`. *Page 103*

A sequence is an object that implements `__len__` and `__getitem__` and expects to be able to get the elements it contains, one at a time, in order, starting at zero as the first index. This means that you should be careful in the logic so that you correctly implement `__getitem__` to expect this type of index, or the iteration will not work. *Page 103*

The implementation with an iterable will use less memory, but it takes up to O(n) to get an element, whereas implementing a sequence will use more memory (because we have to hold everything at once), but supports indexing in constant time, O(1). *Page 103*

## **Summary**