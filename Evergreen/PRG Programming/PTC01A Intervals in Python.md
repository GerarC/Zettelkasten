---
reference: "[[CCPs01 Indexes & Slice in Python]]"
date: 24/01/2023
type: 1 #evergreen
topics: Programming, Code, Software, Iterable, Python, Pythonic Code
alias: PTC01A, Interval, Slice, Slice in Python
tags: programming, code, software, iterable, python, pythonic_code
code: PTC01A
---
# PTC01A Intervals in Python

[[PTC01 Indexes in Python#PTC01 Indexes in Python|Index]] is not the only one object which you can access to an array, there is Intervals too. you can use an interval like an index, i.e., `object[<interval>]` form.
The interval has the next syntax `object[first_index:last_index:steps]`. `first_index` says where init the interval, `last_index` says where finish without the last item, and `steps` says how many items "jump", this can be ignored.
There is some special interval forms: `[index:]` returns all the items from `index` to the final, `[:index]` return from the beginning of the array to `index` and `[::]` just copy all the array.

**Examples:**
~~~ python
my_nums = [2,3,4,6,9,5,8,7]

# Interval without steps
my_nums[2:5]

# Interval with steps
my_nums[0:6:2]

# From an index to the final
my_nums[3:]

# From the beginning to an index
my_nums[:4]

# Copy the list
my_nums[::]
~~~

# PTC01A/1 Slice Class

[[#PTC01A Intervals in Python|Intervals]] in python work due to an built-in class named `slice`, that you can instance without an array and works exactly like the intervals, but putting specifically the `None` values. i.e., where an interval was `[2:]` while with slice is `slice(2, None)` and so on.

**Examples:**
~~~ python
my_nums = [2,3,4,6,9,5,8,7]

# Instance the interval
interval = slice(1,7,2)

# Use it
my_nums[interval]
~~~


# Links
<<[[PTC01 Indexes in Python|PTC01]]|[[PTC01B Create Own Sequences with len and getitem|PTC01B]]>>