---
reference: [[CCPs01 Indexes & Slice in Python]]
date: 21/01/2023
type: 1 #evergreen
topics: Programming, Code, Software, Iterable, Python, Pythonic Code
alias: PTC01, Index, Index in Python
tags: programming, code, software, iterable, python, pythonic_code
code: PTC01
---
# PTC01 Indexes in Python

Like in others programming languages, in Python, there is some built-in data structures, and those have a way to access its elements. For example, but no the only one, with indexes. In an array you can access to its item using this syntax: `object[index]`. where `object` is the reference to the data structure and `index`, redundantly, the index of the item.
The Index of the first item is `0`, index of the second item is `1` and so on. But unlike other languages, Python allows to access items from the last to the first, and this it with negative numbers, `-1` is the index of the last item, `-2` is of the second to last and so on.

**Examples:**
~~~ python
mylist = [2,35,8,4,7]

# First element
print(mylist[0])

# Second element
print(mylist[1])

# Last element
print(mylist[-1])
~~~

# Links
**Previous:** [[PTC00A Documentation in Python|PTC00A]]
**Next:** [[PTC01A Intervals in Python|PTC01A]]