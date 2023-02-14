---
title: Clean code in Python
date: 31/01/2023
source: [chapter 2, pages: [87,91]]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: programming, python, pythonic_code
---
# CPPs02 Underscores in Python

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Pages \[87, 91\].

## **Quote** 
> All of the properties and functions of an object are public in Python, which is different from other languages where properties can be public, private, or protected. That is, there is no point in preventing caller objects from invoking any attributes an object has. *Page 87*

> The interpretation of this code is that `_timeout` should be accessed only within connector itself and never from a caller. This means that you should organize the code in a way so that you can safely refactor the timeout at all of the times it's needed, relying on the fact that it's not being called from outside the object (only internally) *Page 89*

> There is, however, a common misconception that some attributes and methods can be actually made private. This is, again, a misconception. *Page 89*

> modify it. Now, take a look at the exception that is raised when trying to access `__timeout`. It's `AttributeError`, saying that it doesn't exist. It doesn't say something like "`this is private`" or "`this can't be accessed`" and so on. It says it does not exist. This should give us a clue *Page 90*

> What's actually happening is that with the double underscores, Python creates a different name for the attribute (this is called name mangling). What it does is create the attribute with the following name instead: "`_<class-name>__<attribute-name>`". *Page 90*

> The idea of the double underscore in Python is completely different. It was created as a means to override different methods of a class that is going to be extended several times, without the risk of having collisions with the method names. *Page 91*

> Double underscores are a non-Pythonic approach. If you need to define attributes as private, use a single underscore, and respect the Pythonic convention that it is a private attribute.
> <sub>Do not use double underscores.</sub> *Page 91*

<!--Yes, I know it is a lot of quotes just for a one source note, but all of them are on the same topic-->

## **Summary**

In python ain't got anything like private or protected attributes or methods. All is public, even double underscore things are public.

double underscore just change the name, but doesn't make it private. For example, if you try to access to the `__attr` attribute of the class `Class` will raise an `AttributeError` exception indicating that it doesn't exist. This should be a clue about what is happening. Actually double underscore just change the name of the attribute to something like `_Class__attr`, this change is called name mangling. This type of name was created as a means to override methods of a class that would extend several times, without risks of collisions.

The recommendation is doesn't use double underscore to make private objects 'cause this is a non-Pythonic approach, use just one underscore instead