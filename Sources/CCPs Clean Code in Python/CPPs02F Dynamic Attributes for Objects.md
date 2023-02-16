---
title: Clean code in Python
date: 31/01/2023
source: [chapter 2, pages: [109, 111]]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: programming, python, pythonic_code
---
# CPPs02F Dynamic Attributes for Objects

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Pages \[109, 111\].

## **Quote** 
It is possible to control the way attributes are obtained from objects by means of the `__getattr__` magic method. When we call something like `<myobject>.<myattribute>`, Python will look for `<myattribute>` in the dictionary of the object, calling `__getattribute__` on it. If this is not found (namely, the object does not have the attribute we are looking for), then the extra method, `__getattr__`, is called, passing the name of the attribute (`myattribute`) as a parameter. By receiving this value, we can control the way things should be returned to our objects. We can even create new *Page 109*

Take another look at the code in the `__getattr__` method. Notice the exception it raises when the value is not retrievable `AttributeError`. This is not only for consistency (as well as the message in the exception) but also required by the built-in `getattr()` function. Had this exception been any other, it would raise, and the default *Page 111*

## **Summary**
