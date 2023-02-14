---
title: Clean code in Python
date: 31/01/2023
source: [chapter 2, page 121]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: programming, python, pythonic_code
---
# CPPs03A Extending built-in types

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Page 121.

## **Quote** 
The correct way of extending built-in types such as lists, strings, and dictionaries is by means of the collections module. *Page 121*

If you create a class that directly extends dict, for example, you will obtain results that are probably not what you are expecting. The reason for this is that in CPython the methods of the class don't call each other (as they should), so if you override one of them, this will not be reflected by the rest, resulting in unexpected outcomes. For example, you might want to override `__getitem__`, and then when you iterate the object with a for loop, you will notice that the logic you have put on that method is not applied. *Page 121*

## **Summary**