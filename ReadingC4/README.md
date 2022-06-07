# Reading Class 04
## Classes and Objects

<b> Object </b> -- an encapsulation of data along with functions that act upon that data.
An object consists of:

- Name : the variable name we give it

- Member data : the data that describes the object

- Member functions : behavior aspects of the object 
(functions related to the object itself)

<b>Class</b> -- a blueprint for objects. A class is a user-defined type that describes what a certain type of object will look like. A class description consists of a declaration and a definition. Usually these pieces are split into separate files.

An object is a single instance of a class. and we can create many objects from the same class type.

A very basic class would look something like this:


class MyClass:

    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

## Thinking Recursively in Python

the essence of thinking recursively, is break computer science down into smaller chunks to solve it.

### Recursive Functions in Python
 A recursive function is a function defined in terms of itself via self-referential expressions. This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case.

 ### Recursive Data Structures in Python
A data structure is recursive if it can be deﬁned in terms of a smaller version of itself. A list is an example of a recursive data structure. ex:  if we have only an empty list at your disposal, and the only operation we can perform on it is this:

>> Return a new list that is the result of

>> adding element to the head (i.e. front) of input_list

>> def attach_head(element, input_list):

 >>   return [element] + input_list


 Using the empty list and the attach_head operation, can generate any list.

 Recursive data structures and recursive functions go together like bread and butter. The recursive function’s structure can often be modeled after the definition of the recursive data structure it takes as an input
