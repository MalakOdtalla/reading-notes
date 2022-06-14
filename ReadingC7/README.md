# Reading Class 07

## Python Scope & the LEGB Rule

The concept of scope rules how variables and names are looked up in the code. It determines the visibility of a variable within the code. The scope of a name or variable depends on the place in the code where the variable is created. The Python scope concept is generally presented using a rule known as the LEGB rule (Local, Enclosing, Global, and Built-in) scopes. This summarizes not only the Python scope levels but also the sequence of steps that Python follows when resolving names in a program.

<b>The advantage of Python scopes:</b> to write more reliable and maintainable programs. Using Python scope will help to avoid or minimize bugs related to name collision as well as bad use of global names across your programs.



### Python Scope vs Namespace

- A namespace --  is a mapping from names to objects.It determines which identifiers (e.g. variables, functions, classes) are available for use.

- A scope -- is a textual region of a Python program where a namespace is directly accessible. It defines where — in the written code — a namespace can be accessed.


<b>There are four types of scopes:</b>

- The local scope --  The local scope is determined by whether you are in a class/function definition or not. Inside a class/function, the local scope refers to the names defined inside them. Outside a class/function, the local scope is the same as the global scope.




- The non-local scope --  A non-local scope is midways between the local scope and the global scope, e.g. the non-local scope of a function defined inside another function is the enclosing function itself.




- The global scope -- This refers to the scope outside any functions or class definitions. It also known as the module scope.



- The built-ins scope -- This scope, as the name suggests, is a scope that is built into Python. While it resides in its own module, any Python program is qualified to call the names defined here without requiring special access.



-- Example:


>>  Global Scope A

>> a = 1

>> b = 16


>> def outer():

    >> Local Scope B

   >>  c = 24

    >> d = 'Hello, World!'

    
 >>   def inner():

       >> Non Local Scope C

  >>      e = 'I like'

   >>     f = 'fried chicken'


>> Built Ins Scope D

>> print('Hello!')


