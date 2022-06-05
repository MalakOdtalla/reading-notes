## Reading Class 03

# Reading and Writing Files in Python
## What Is a File?

a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

## Opening and Closing a File in Python

When you want to work with a file, the first thing to do is to open it. This is done by invoking the open() built-in function. open() has a single required argument that is the path to the file. open() has a single return, the file object:
file = open('dog_breeds.txt')

It’s important to remember that it’s your responsibility to close the file. and there are two ways that you can use to ensure that a file is closed properly, even when encountering an error. The first way to close a file is to use the try-finally block:<br>
reader = open('dog_breeds.txt')

 try:

    # Further file processing goes here
finally:

    reader.close()

The second way to close a file is to use the with statement:<br>

with open('dog_breeds.txt', 'r') as reader:

    # Further file processing goes here

the second positional argument, mode. This argument is a string that contains multiple characters to represent how you want to open the file. The default and most common is 'r', which represents opening the file in read-only mode as a text file.

'w'	Open for writing, truncating (overwriting) the file first.

'rb' or 'wb'	Open in binary mode (read/write using byte data).

## Reading and Writing Opened Files

There are multiple methods that can be called on a file object for reading a file:
- .read(size=-1)	This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read.
- .readline(size=-1)	This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read.
- .readlines()	This reads the remaining lines from the file object and returns them as a list.

file objects have multiple methods that are useful for writing to a file:

- .write(string)	This writes the string to the file.
- .writelines(seq)	This writes the sequence to the file. No line endings are appended to each sequence item. It’s up to you to add the appropriate line ending(s).



# Python Exceptions

A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception.

Syntax errors:  occur when the parser detects an incorrect statement.

 exception error: This type of error occurs whenever syntactically correct Python code results in an error.

 ## Raising an Exception
We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.

If we want to throw an error when a certain condition occurs using raise, we could go about it like this:

x = 10

if x > 5:

    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))

## The AssertionError Exception
Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError exception.

Have a look at the following example, where it is asserted that the code will be executed on a Linux system:

import sys

assert ('linux' in sys.platform), "This code runs on Linux only."

## The try and except Block: Handling Exceptions
The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.

try:

    with open('file.log') as file:
        read_data = file.read()

except:
    print('Could not open file.log')

If file.log does not exist, this block of code will output: Could not open file.log


## The else Clause
In Python, using the else statement, it can instruct a program to execute a certain block of code only in the absence of exceptions.

try:

    linux_interaction()
except AssertionError as error:

    print(error)
else:

    print('Executing the else clause.')


## Cleaning Up After Using finally
Imagine that we always had to implement some sort of action to clean up after executing your code. Python enables to do so using the finally clause.

everything in the finally clause will be executed. It does not matter if we encounter an exception somewhere in the try or else clauses

[Back To Main](/README.md)