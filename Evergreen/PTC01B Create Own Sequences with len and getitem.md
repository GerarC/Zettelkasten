---
reference: [[CCPs01A Creating Sequenses]]
date: 24/01/2023
type: 1 #evergreen
topics: Programming, Code, Software, Iterable, Python, Pythonic Code
alias: PTC01B, Own Sequences in Python, getitem
tags: programming, code, software, iterable, python, pythonic_code
code: PTC01B
---
# PTC01B Create Own Sequences

Things like [[PTC01 Indexes in Python#PTC01 Indexes in Python|indexes]] and [[PTC01A Intervals in Python#PTC01A Intervals in Python|intervals]] work by the following two methods: `__getitem__` and `__len__`. The first method gives you the possibility of get a item when you call the structure like `object[item]`, `item` can be any object you need, such as index, slice, string, etc. The second method returns the size of the object.
If you implement this methods in a custom class that isn't a [[#PTC01B/1 Sequences in a Wrapper Class|wrapper]] of any built-in data structure, then you must to keep in mind two things. The first one is that the object returned by the method should be of the same type of the class. The other thing you must keep in mind is try to respect the semantics that Python uses, i.e., the intervals exclude the last item.

# PTC01B/1 Sequences in a Wrapper Class

When you are implementing a class that wraps a built-in object, such as a list, a tuple, a dict and so on. Always try to delegate as much as you can the behavior of `__getitem__` and `__len__` to the wrapped class. 

**Example** of a **wrapper class** delegating:
~~~ python
class Items:
	def __init__(self, *values):
	self._values = list(values)

def __len__(self):
	return len(self._values)

def __getitem__(self, item):
	return self._values.__getitem__(item)
~~~

# Links
**Previous:** [[PTC01A Intervals in Python|PTC01A]]
**Next:** [[PTC02 Context Manager|PTC02]]