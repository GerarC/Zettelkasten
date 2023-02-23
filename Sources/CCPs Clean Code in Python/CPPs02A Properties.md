---
title: Clean code in Python
date: 31/01/2023
source: [chapter 2, pages: [92, 95]]
author: Mariano Anaya
type: 2 #sourcenote
topics: Programming, Python, Pythonic Code
tags: programming, python, pythonic_code
---
# CPPs02A Properties

## **Reference** 
Clean code in python, Mario Anaya; Chapter 2, Pages \[87, 91\].

# **Quote**
> Properties are to be used when we need to define access control to some attributes in an object, which is another point where Python has its own way of doing things. In other programming languages (like Java), you would create access methods (getters and setters), but idiomatic Python would use properties instead. *Page 92

> By putting email under a property, we obtain some advantages for free. In this example, the first `@property` method will return the value held by the private attribute `email`. *Page 93*

> Then, the second method uses @email.setter, with the already defined property of the previous method. This is the one that is going to be called when `<user>.email` = `<new_email>` runs from the caller code, and `<new_email>` will become the parameter of this method. *Page 93*

> <small>Don't write custom <code>get\_\*</code> and <code>set\_\*</code> methods for all attributes on your objects. Most of the time, leaving them as regular attributes is just enough. If you need to modify the logic for when an attribute is retrieved or modified, then use properties.</small> *Page 94*

> With properties, we can avoid this kind of confusion. The `@property` decorator is the query that will answer to something, and the `@<property_name>.setter` is the command that will do something. *Page 94*


## **Summary**
How in python there are not private or protected things, so create things like getters and setters is useless and there is an idiomatic python option: the properties.

To create a property you just have to use the decorator `@property` and that method will be the "getter" of the attribute and will be called when you use `Class.getter`. On other method use `@<property_name>.setter` to create the "setter" and will be called when you use `Class.<property> = some`.

The recommendation is to use it only if you need to verify or modify the value if you doesn't will do it, then use just public attribute, without underscores.
