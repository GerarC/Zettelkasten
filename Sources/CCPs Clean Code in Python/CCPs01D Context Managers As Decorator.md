---
title: Clean code in Python
date: 22/01/2023
source: [chapter 2, pages: [84, 85]]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: programming, python, pythonic_code
---
# CCPs01D Context Managers As Decorator

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Pages \[84, 85\].

## **Quote** 
> Another helper we could use is `contextlib.ContextDecorator`. This is a mixin base class that provides the logic for applying a decorator to a function that will make it run inside the context manager, while the logic for the context manager itself has to be provided by implementing the aforementioned magic methods. *Page 84*

> Do you notice something different from the previous examples? There is no with statement. We just have to call the function, and `offline_backup()` will automatically run inside a context manager. This is the logic that the base class provides to use it as a decorator that wraps the original function so that it runs inside a context manager. *Page 85*

> The only downside of this approach is that by the way the objects work, they are completely independent (which is a good trait)—the decorator doesn't know anything about the function that is decorating, and vice versa. *Page 85*
	
> Being a decorator, this also poses the advantage that the logic is defined only once, and we can reuse it as many times as we want by simply applying the decorators to other functions that require the same invariant logic. *Page 85*

## **Summary**
The `context` module have a helper we can use, `contextlib.ContextDecorator`. It is a base class that provides a way to implement a Decorator that wraps the function in a context manager while the logic of the manager 

To make this decorator you have to create a class that inherits of `ContextDecorator` and create `__enter__` and `__exit__` methods.

When you use this form you don't have to use `with` statement.

The downside of this form is that the context manager and the function are completely independent (is a good trait) the decorator doesn't know anything about the function, a vice versa.

Being a decorator also adds an extra advantage: the logic is defined only once, and we can reuse it as many times as we need by simply applying  the decorator.