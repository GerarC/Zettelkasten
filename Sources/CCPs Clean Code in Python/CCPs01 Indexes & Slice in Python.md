---
title: Clean code in Python
date: 22/01/2023
source: [chapter 2, pages: [71, 73]]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: programming, python, pythonic_code
---
# CCPs01 Indexes & Slice in Python

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Pages \[71, 73\].

## **Quotes**
> In Python, as in other languages, some data structures or types support accessing its elements by index. Another thing it has in common with most programming languages is that the first element is placed in the index number zero. However, unlike those languages, when we want to access the elements in a different order than usual, Python provides extra features. *Page 71*

> I would get the element in the position of the length of the array minus one. This could work, but we could also use a negative index number, which will start counting from the last. *Page 71*

> You should always prefer to use this built-in syntax for slices, as opposed to manually trying to iterate the tuple, string, or list inside a for loop, excluding the elements by hand. *Page 73*

## **Summary**
As in other programming languages, in python, there is some data structures that support to access its elements with indexes. The index of the first element in an array is zero. But unlike the most of the languages, python lets you accessing data structures since minus -1 to below, being -1 the last element of the structure.

In python you can access to specifics intervals using an specific syntax. It is built-in, but below it there is a class that manage this intervals named slice.

You should rather slices than iterate with a `for` loop.



