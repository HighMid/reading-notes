## Data Structures and Algorithms

1. **What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem?**
    
- Ensuring that you choose the most efficient data structure for a given problem as time complexity is very important.

    - Arrays are great at retrieving data at a specific index and is very fast because of direct access. However they are not very efficient for adding or removing data as the size is fixed and requires the shifting of elements if it's in the middle of the array.

    - Linked Lists are efficient for adding and removing data at the beginning and end of the list and are dynamic in size. Because of this they require more memory and could potentially be slower if you start from the beginning.

    - Hash Tables are considered average in time complexity but any hashable object can be used as a key, but they do not maintain any order.

2. **How can we ensure that we’ll avoid an infinite recursive call stack?**

- Use of a base case, this is a condition that stops the function from calling itself. Each recursive calls should be progressing to the base case as this leads to the end. You can also limit your usage of recursion by using Iterative solutions as these typically have the same efficiency without the risks involved with stack overflow.