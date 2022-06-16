# Reading Class 08

## List Comprehensions in Python

List comprehension is a powerful and concise method for creating lists in Python that becomes essential the more you work with lists, and lists of lists. It offers a shorter syntax when creating a new list based on the values of an existing list.

### The Syntax

>>  newlist = [x for x in list]

- with condition

>> newlist = [expression for item in iterable if condition == True]

- with iterable we can use range

>> newlist = [x for x in range(10)]

- with expressions 

>> newlist = [x if x != "banana" else "orange" for x in fruits]

- with functions

>> def double(x):

>>    return x*2

>> even_nums = [double(x) for x in range(1,10) if x%2 == 0]

>> print(even_nums)


