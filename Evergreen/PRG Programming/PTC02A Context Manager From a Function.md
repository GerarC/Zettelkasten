---
reference: [[CCPs01C Context Manager as Function]]
date: 24/01/2023
type: 1 #evergreen
topics: Programming, Code, Software, Python, Pythonic Code, Context Manager, Good Practices
alias: PTC02A, Context Manager From a Function
tags: programming, code, software, python, pythonic_code, context_manager, good_practices
code: PTC02A
---
# PTC02A Context Manager From a Function

There is module in Python with a lot of useful utils to work with context managers, it is [[contextlib]]. One of the utils it has is the `contextlib.contextmanager` [[decorator]], this converts a function in a context manager. To do it the function must be of a special type named [[generator]] function, once the decorator is applied, split the function into what corresponds to `__enter__` and what corresponds to `__exit__` respectively. The code is split from the `yield` statement.

**Example:**
~~~ python
def context_manager():
	# Code of the enter
	yield # What it should returns
	# Code of the exit
~~~

# Links
<<[[PTC02 Context Manager|PTC02]]|[[PTC02B Context Manager as Decorator|PTC02B]]>>