---
title: Clean code in Python
date: 22/01/2023
source: [chapter 2, pages: [74, 75]]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: programming, python, pythonic_code
---
# CCPs01A Creating Sequenses

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Pages \[74, 75\].

## **Quote** 
> The functionality we just discussed works thanks to a magic method called `__getitem__`. This is the method that is called, when something like `object[key]` is called, passing the key (value inside the square brackets) as a parameter. A sequence, in particular, is an object that implements both `__getitem__` and `__len__`, and for this reason, it can be iterated over. Lists, tuples, and strings are examples of sequence objects in the standard library. *Page 74*

> In the case that your class is a wrapper around a standard library object, you might as well delegate the behavior as much as possible to the underlying object. This means that if your class is actually a wrapper on the list, call all of the same methods on that list to make sure that it remains compatible. *Page 74*

> If, however, you are implementing your own sequence, that is not a wrapper or does not rely on any built-in object underneath, then keep in mind the following points:
> -  When indexing by a range, the result should be an instance of the same type of the class
> -  In the range provided by the slice, respect the semantics that Python uses, excluding the element at the end
> *Page 75*

## **Summary**
All the things related with slices and indexes work due to the next methods `__getitem__` and `__len__`. The first method allows get items when you call an objects like `object[item]`, item can be any object you need, like an index, slice, string and other objects like that. The second method returns the size of the object.

If the class you have is a wrapper of an built-in object, such as a list, a tuple, a string, and so on. try to delegate all the behavior to the underlying object.

If your class isn't a wrapper and it isn't related with any built-in object, then you must keep in mind two things. The first one is that the object returned by the method should be of the same type of the class of the method. The second one is that you should respect the semantics that python uses, i.e., the intervals are \[a, b\) or in other words, the last item item is excluded.