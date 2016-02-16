#ALL EXIT TICKET SOLUTIONS

##Unit 4

###Thursday 1/07: Data Structures and Algorithms

**Question 1**: What is the difference between a data structure and an algorithm?

Answer: An algorithm is a sequence of steps taken to provide output given a set of input.  A data structure is a way to organize data.

###Saturday 1/09: MVC + Swift

**Question 1**: Describe the actions of a Controller in the scope of MVC

Answer: The controller is the hub between the model and the view. The view will send interactions and user inputted data to the controller and the controller passes that to the model to be evaluated. The model sends that back to the controller which in turn may interact with the view. 

**Quesion 2**: Why would you use an optional?

Answer: to represent a value that may be nil - ie: if a search comes back empty, an optional value will not crash your program

###Sunday 1/10: Big O

**Question 1**: What would the big O (time complexity) be of a method with two nested for loops that each go over the whole array?

**Answer**: O(n^2)

**Question 2**: If you had the choice of two algorithms to solve the same problem, and one was O(log(n)) and the other was O(n^2), which would you choose? 
**Answer**: O(log(n)).  Logarithic functions grow much more slowly than quadratic ones.  For large values of n, log(n)<<n^2.

**Question 3**: When you are picking or writing a solution to a problem or debugging a piece of performance sensitive code, should you look at big O, profiling data, or both? Why?

**Answer**: Both. Depending on the complexity of the solution we write, for example (an O(n) vs O(n^2)) looking at Big O helps, and profiling data helps for performance sensitive code. 

###Thursday 1/14: Discrete math and logic

Question 1: How many unique Powerball ticket configurations are there? Each ticket has six numbers total. The first five numbers are chosen from a collection of 69 numbered balls, labeled 1 through 69. The sixth and final “Powerball” number is chosen from a collection of 26 numbered balls, labeled 1 through 26. The order of the first five numbers does not matter (different orderings are equivalent). Show your work!

**Answer**:  69Choose5 * 26

**Question 2**: What is the best-case run-time complexity of an algorithm that generates all permutations of a string? N represents the number of characters in the input string.

**Answer**: O(n!)

**Question 3**: Out of 40 students 30 can jump, 27 can play football and 5 can do neither. How many students can jump and play football? How can you use sets and/or logic to solve this problem?
 
**Answer**: 22

Question 4: True or False: The following boolean expressions are equivalent: !(y && !x) and x || !y

**Answer**: True

###Saturday 1/16: Linked Lists and Sorts

**Question 1**: In big O notation, how long does it take to access an element in an array of lists if you are given a pair of indices?

**Answer**: O(n)

**Question 2**: What is the Big O runtime to bubble sort [2,3,4,5,6,7,8,1] from least to greatest. Why?

**Answer**: O(n^2).  Each pass through the array takes n time and n passess will be made to get the '1' to the beginning.  Performing an O(n) operation n time is O(n^2).

###Sunday 1/17: Sorts

**Question 1**: What is insert(3, intoSortedArray:[1,2,3,4])?

**Answer**: [1, 2, 3, 3, 4]

**Question 2**: What is select([0,1,2,6,3,5,4], startingAt:3)?

**Answer**: 4

**Question 3**: As we implemented them in class today, what is the advantage of selection sort over insertion sort?

**Answer**: It is in-place/it uses less memory

###Thursday 1/21

**Question 1**: In general terms, how would you implement a loop in assembly code?

**Answer**: The LOOP instruction assumes that the ECX register contains the loop count. When the loop instruction is executed, the ECX register is decremented and the control jumps to the target label, until the ECX register value, i.e., the counter reaches the value zero.

**Question 2**: How big (in bytes) is a stack frame for a call to the following C function? https://gist.github.com/cspickert/51795018a93b9fe12f79

**Answer**: 8 bytes or 16 bytes

**Question 3**: Name one **advantage** of dynamic (heap) memory allocation.

**Answer**: Variables may be accessed globally (plenty of other answers)

Quesiton 4: Name one **disadvantage** of static (stack) memory allocation.

**Answer**: Less space for memory/ easier to fill up and cause an overflow because of a function or array that is too large/many other answers

###Sunday 1/24: Recursion

**Question 1**: What are the two cases every recursive function must have?

**Answer**: (1) base case and (2) recursive call

**Question 2**: What is one potential advantage of recursive functions?

**Answer**: Cleaner, better organized code.  Use 'divide and conquer' strategies to solve problems.  Breaks down one complicated problem into several simpler ones.

Quesiton 3: What is one potential disadvantage of recursive functions?

**Answer**: Uses more memory/Can take longer/

###Thursday 2/28: Merge Sort

**Question 1**: What is the big-O time complexity of mergesort?

**Answer**: What is the big-O time complexity of mergesort?

**Question 2**: Using the implementation of mergeSort from class, how many times would mergeSort be called for the following array: [10, 2, 1, 6]

**Answer**: 7 times

**Question 3**: In 1-2 sentences, describe how to implement a loop recursively (without using for or while).

**Answer**: In a recursive function, set a base case that returns when a counter gets to 0.  Then, have the function call itself, passing the counter back.

###Saturday 1/30: Quicksort, Stacks and Queues

**Question 1**: Explain the difference between a stack and a queue

**Answer**: A stack is last in, first out (LIFO).  A queue is first in, first out (FIFO).

**Question 2**: Explain the difference between merge sort and quicksort

**Answer**: Merge sort breaks an array down into single elements, then combines the pieces.  A bunch of calls are pushed to the stack, then resolved.  Quick sort picks a pivot, then sorts the array into two groups, with everything smaller than it on the left, and everything bigger than it on the right.  This process is repeated for the left half and the right half recursively.  You make a bunch of stack calls, but never have to pop them off and go back down.

**Question 3**: Give a scenario that would degrade quicksort to O(N^2)

**Answer**: If the pivot you choose was always the greatest or smallest value in an array

###Sunday 1/31

**Question 1**: What is a hash collision?

**Answer**:  A hash collision is when two different keys hash to the same value.  This means that their lookup ID would be the same, unless the collision is resolved.

**Question 2**: What is the union of these sets: {1, 2, 3} and {4, 5, 2}

**Answer**: {1,2,3} U {5,4,2} = {1,2,3,4,5}

**Question 3**: Briefly describe one of the two common strategies for dealing with hash collisions

**Answer**: Either pick (1)[Open addressing](https://en.wikipedia.org/wiki/Open_addressing) or (2) [Separate Chaining](https://en.wikipedia.org/wiki/Hash_table#Separate_chaining)

###Thursday 2/04

**Question 1**: Name an example of a tree structure you've created or encountered while developing iOS apps.

**Answer**: Many different answers apply.  **Answer**s include view hierarchy and directory/file structure

**Question 2**: What is the height (or depth)  of a "complete" binary tree—where every level is filled with the maximum number of nodes—consisting of 255 nodes?

**Answer**: log(255)

###Saturday 2/06

**Question 1**: What is the runtime of BSF?

**Answer**: The runtime of BFS for any graph is O(n+m) where n=number of nodes and m=number of edges.  In a binary tree, the number of edges is always one less than the number of nodes.  Mathematically, m=n-1 Thus, the runtime is O(n+n-1)=O(2n)=O(n)

**Question 2**: What is a type of graph where BFS can be used to find the shortest path?

**Answer**: An undirected, unweighted graph.

###Sunday 2/07

**Question 1**: Name one situation where you'd prefer DFS over BFS

**Answer**: You want to find paths to the bottom of a tree/You know the information you are looking for is at the bottom.

**Question 2**: What is the big O time complexity of DFS for a graph?

**Answer**: The runtime of DFS for any graph is O(n+m) where n=number of nodes and m=number of edges.  In a binary tree, the number of edges is always one less than the number of nodes.  Mathematically, m=n-1 Thus, the runtime is O(n+n-1)=O(2n)=O(n)

**Question 3**: What are the B and the D for in BFS and DFS?

**Answer**: B = Breadth.  D = Depth.

