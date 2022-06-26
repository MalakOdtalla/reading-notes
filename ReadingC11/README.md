# Reading Class 11

## NumPy Tutorial: Data Analysis with Python

<b>NumPy</b> is the fundamental package for scientific computing in Python. It is a Python library that provides a multidimensional array object, various derived objects (such as masked arrays and matrices), and an assortment of routines for fast operations on arrays, including mathematical, logical, shape manipulation, sorting, selecting, I/O, discrete Fourier transforms, basic linear algebra, basic statistical operations, random simulation and much more.
One of the limitations of NumPy is that all the elements in an array have to be of the same type.

## The difference between a Python list and a NumPy array

NumPy gives  an enormous range of fast and efficient ways of creating arrays and manipulating numerical data inside them.

 While a Python list can contain different data types within a single list, all of the elements in a NumPy array should be homogeneous. The mathematical operations that are meant to be performed on arrays would be extremely inefficient if the arrays weren’t homogeneous.


NumPy arrays are faster and more compact than Python lists. An array consumes less memory and is convenient to use. 

NumPy uses much less memory to store data and it provides a mechanism of specifying the data types. This allows the code to be optimized even further.



### Creating A NumPy Array
- We can create a NumPy array using the <b>numpy.array </b>function. If we pass in a list of lists, it will automatically create a NumPy array with the same number of rows and columns.

- Anathor method we can use :  <b>numpy.zeros</b>
It’s useful to create an array with all zero elements in cases when you need an array of fixed size, but don’t have any values for it yet.

- also we can create an array where each element is a random number using <b>numpy.random.rand</b>

### Using NumPy To Read In Files
It’s possible to use NumPy to directly read csv or other files into arrays. We can do this using the <b>numpy.genfromtxt</b> function.



