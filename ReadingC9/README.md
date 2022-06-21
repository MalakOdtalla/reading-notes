# Reading Class 09

## Dunder Methods or “magic methods”

Predefined methods used to enrich classes. They are easy to recognize because they start and end with double underscores, for example _ _init_ _ (or)  _ _str_ _.
Pythonistas adopted the term “dunder methods”, a short form of “double under.”


Dunder methods let you emulate the behavior of built-in types. For example, to get the length of a string you can call len('string'). But an empty class definition doesn’t support this behavior out of the box:

>> class LenSupport:

>>    def __len__(self):

>>        return 42

>>> obj = LenSupport()

>>> len(obj)

> 42

we can use dunder methods to unlock some of python language features:

- Object Initialization: _ _init_ _
- Object Representation: _ _str_ _, _ _repr_ _,
 to provide a string representation of objects in the class.
- Iteration: _ _len_ _,  _ _getitem_ _ , _ _reversed_ _,
to iterate over class objects.
- Operator Overloading for Comparing python objects: _ _eq_ _, _ _lt_ _.
- Operator Overloading for Merging objects: _ _add_ _
- Callable Python Objects: _ _call_ _
- Context Manager Support and the With Statement: _ _enter_ _, _ _exit _ _,

A context manager is a simple “protocol” (or interface) that your object needs to follow so it can be used with the with statement. Basically all you need to do is add _ _enter__ and _ _exit__ methods to an object if you want it to function as a context manager.
 