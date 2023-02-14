---
reference: [[CCPs01D Context Managers As Decorator]]
date: 24/01/2023
type: 1 #evergreen
topics: Programming, Code, Software, Python, Pythonic Code, Context Manager, Good Practices
alias: PTC02B, Context Manager as Decorator
tags: programming, code, software, python, pythonic_code, context_manager, good_practices, decorator
code: PTC02B
---
# PTC02B Context Manager as Decorator

[[contextlib]] module has a helper we can use to make a decorator that wraps functions in a [[PTC02 Context Manager#PTC02 Context Manager|Context Manager]]. To create this decorator you just have to create a class that inherits from `contextlib.ContextDecorator` and create `__enter__` and `__exit__` methods.
Some advantages are that when you use this type of context manager you don't need to use `with` statement and the logic is defined only once, and we can reuse it as many times as we need by simply apply a decorator.
But this form also has a downside: the context manager and the function logic are completely independent (is a good trait actually). The decorator doesn't know anything about the function, and vice versa.

**Example:**
~~~ python
class context_manager(contextlib.ContextDecorator):
	def __enter__(self):
		stop_database()

	def __exit__(self):
		start_database()

@context_manager
def db_backup():
	run("pg_dump database")
~~~

# Links
**Previous:** [[PTC02A Context Manager From a Function|PTC02A]]
**Next:** [[PTC02C Manage Errors with Context Manager|PTC02C]]