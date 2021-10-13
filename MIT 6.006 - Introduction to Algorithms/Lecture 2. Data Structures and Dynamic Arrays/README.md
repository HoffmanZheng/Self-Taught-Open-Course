# Lecture 2. Data Structures and Dynamic Arrays

1. Data structure: store non-constant data, support a set of operations

2. Array: **consecutive** chunk of memory, which could be addressed by index (random access, constant time (assume w >= lg(n)))

3. Array: constant time in static operations, but need to reallocate new array or shift all items during inserting and removing

4. Linked List: **pointer** data structure, could insert and delete from the front in *Θ(1)* time, but take *Θ(i)* in get/set operations

5. Dynamic Array: allocate **extra** space so reallocation does not occur with every dynamic operation, insert or delete  at last in Θ(1) time

6. Amortized analysis: Inserting into a dynamic array takes *Θ(1)* amortized time (more amortization analysis in [6.046](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-046j-design-and-analysis-of-algorithms-spring-2015/))

7. Reallocate cost from 0 to n, amortized time per insert operations: 

![](https://github.com/NervousOrange/Self-Taught-Open-Course/raw/main/MIT%206.006%20-%20Introduction%20to%20Algorithms/images/Lecture2-amortizationOfDynamicArray.png)

| Data Structure | Container | Static | insert_first(x) delete_first | insert_last(x) delete_last | insert_at(i,x) delete_at(i) |
| -------------- | --------- | ------ | ---------------------------- | -------------------------- | --------------------------- |
| Array          | n         | 1      | n                            | n                          | n                           |
| Linked List    | n         | n      | 1                            | n                          | n                           |
| Dynamic Array  | n         | 1      | n                            | 1<sub>(a)</sub>            | n                           |



