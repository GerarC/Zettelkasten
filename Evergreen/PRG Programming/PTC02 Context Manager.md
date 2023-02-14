---
reference: [[CCPs01B Context Managers]]
date: 24/01/2023
type: 1 #evergreen
topics: Programming, Code, Software, Python, Pythonic Code, Context Manager, Good Practices
alias: PTC02, Context Manager
tags: programming, code, software, python, pythonic_code, context_manager, good_practices
code: PTC02
---
# PTC02 Context Manager

A context manager is a feature that python has, this managers follow a pattern where it runs code that needs preconditions and postconditions. The most of the time we use them for the resource management or if we open any connection to a service or socket. The context manager can work thanks to two method: `__enter__` and `__exit__`. When you init a context manager with the special word `with`, it calls `__enter__` method, this "contextualizes" and returns an object that you can label with the word `as`, then enter in the context. Finally, when the code is executed, the manager calls `__exit__` method and it manage any error that could occur.
It's a good practice return something on the `__enter__` method, although it isn't mandatory and even if it returns something, there is no reason yet to label it with `as`.

**Examples:**
**1.** 
~~~ python
# When you open a file, usually you do something like this:
try:
	file = open(filename)
	process_file(file)
finally:
	file.close()

# With context manager is easier:
with open(filename) as file:
	process_file(file)
~~~

**2.**
~~~ python
# Create a context manager
def stop_database():
	run("systemctl stop postgresql.service")

def start_database():
	run("systemctl start postgresql.service")

class DBHandler():
	def __enter__(self):
		stop_database()
		return self

	def __exit__(self, ex_type, ex_value, ex_traceback):
		star_database()

def bd_backup():
	run("pg_dump database")

def main():
	with DBHandler():
		bd_backup()
~~~

# Links
<<[[PTC01B Create Own Sequences with len and getitem|PTC01B]]|[[PTC02A Context Manager From a Function|PTC02A]]>>