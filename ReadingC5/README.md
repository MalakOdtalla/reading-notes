# Reeading Class 05

## Big O: Analysis of Algorithm Efficiency
- what is big O ?

Big O(oh) notation is used to describe the efficiency of an algorithm or function( the Worst Case of efficiency an algorithm can have in performing it’s job), This efficiency is evaluated based on 2 factors:

1- Running Time (also known as time efficiency / complexity)
The amount of time a function needs to complete.

2- Memory Space (also known as space efficiency / complexity)
The amount of memory resources a function uses to store data and instructions.

- How we can analyze these factors?
we should consider 4 Key Areas for analysis:

1- Input Size

Input Size refers to the size of the parameter values that are read by the algorithm. This does not simply refer to the number of parameters an algorithm reads, but takes into account the size of each parameter value as well.

<b>Example:</b> If a function uses an array or list as one parameter, then the number of elements within that array or list will directly increase the Input Size of that parameter.


2- Units of Measurement

To evaluate a function for Time and Space complexity, we need a way to measure each of these factors.

In order to quantify the Running Time in our analysis, we will consider Three Measurements of time:

1) The time in milliseconds from the start of a function execution until it ends.
2) The number of operations that are executed
3) The number of “Basic Operations” that are executed.

In order to quantify Memory Space, we can consider Four Sources of Memory Usage during function run-time:

1) The amount of space needed to hold the code for the algorithm.

2) The amount of space needed to hold the input data.
3) The amount of space needed for the output data.

4) The amount of space needed to hold working space during the calculation



3- Orders of Growth

We can describe overall efficiency by using the input size n and measuring the overall Units of Space and Time required for the given input size n. As the value of n grows, the Order of Growth represents the increase in Running Time or Memory Space.

4- Best Case, Worst Case, and Average Case

Even though Big O describes the Worst Case for algorithm efficiency, we can still think about Best and Average cases. Each of these cases could be analyzed as we consider the overall question: As inputs n fluctuate in size and order, how does this affect our orders of Growth?

<b>worst Case:</b> The efficiency for the worst possible input of size n

<b>Best Case:</b> The efficiency for the best possible input of size n

<b>Average Case:</b> The efficiency for a “typical” or “random” input of size n.


## Linked List
- What is a Linked List?

A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.

- Terminology:

Linked List - A data structure that contains nodes that links/points to the next node in the list.

Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.

Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.

Node - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.

Next - Each node contains a property called Next. This property contains the reference to the next node.

Head - The Head is a reference of type Node to the first node in a linked list.

Current - The Current is a reference of type Node to the node that is currently being looked at. When traversing, you create a new Current variable at the Head to guarantee you are starting from the beginning of the linked list.

- What is the types of linked list?

Even though the parts of a linked list don’t change, the way that we structure our linked lists can be quite different. Like most things in software, depending on the problem that we’re trying to solve, one type of linked lists might be a better tool for the job than another.

1) Singly linked lists:

 are the simplest type of linked list, based solely on the fact that they only go in one direction. There is a single track that we can traverse the list in; we start at the head node, and traverse from the root until the last node, which will end at an empty null value.

 2)  doubly linked list:
 
   there are two references contained within each node: a reference to the next node, as well as the previous node. This can be helpful if we wanted to be able to traverse our data structure not just in a single track or direction, but also backwards, too.

   3) circular linked list:
   
   is a little odd in that it doesn’t end with a node pointing to a null value. Instead, it has a node that acts as the tail of the list (rather than the conventional head node), and the node after the tail node is the beginning of the list.

![img](https://miro.medium.com/max/1400/1*AeMDLFUjR0w0J4n8CP4H6g.jpeg)