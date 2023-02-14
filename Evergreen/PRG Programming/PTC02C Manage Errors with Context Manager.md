---
reference: [[CCPs01E Managing errors with context manager]]
date: 24/01/2023
type: 1 #evergreen
topics: Programming, Code, Software, Python, Pythonic Code, Context Manager, Good Practices
alias: PTC02C, Context Manager as Decorator
tags: programming, code, software, python, pythonic_code, context_manager, good_practices
code: PTC02C
---
# PTC02C Manage Errors with Context Manager

When we wanna handle an error we usually use `try`/ `except` statements,l but there is other way to do this, and it's using [[PTC02 Context Manager|context managers]]. [[contextlib]] module has an util to implement it, named `suppress`. `contextlib.suppress` is a function that can replace `try` and `except`, you just need to pass the Error Type as parameter and inside the context write the code that can raise this exception.

**Example:**
~~~ python
# Managing an error with a context manager
with contextlib.suppress(DataCoversionError):
	parse_data(json_info)
~~~

# Links
<<[[PTC02B Context Manager as Decorator|PTC02B]]|[[]]>>