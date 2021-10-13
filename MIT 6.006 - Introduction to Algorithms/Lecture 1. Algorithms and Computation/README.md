# Lecture 1. Algorithms and Computation

1. Goal of class: be able to **communicate** to others that a solution to a problem is both **correct** and **efficient**.
2. **Algorithms**: solves a problem if it returns a correct output for every problem input
3. Correctness: (example problem) In this room, is there a pair of students with same birthday? 
   1. Use **induction**
   2. Assume first k students don't contain match, and consider k = k + 1
   3. Algorithm checks whether birthday of student k + 1 exist in first k
4. Efficiency: 
   1. Measure the performance, which is machine **independent**
   2. **Asymptotic** Notation: Upper bounds (O), lower bounds (Ω), tight bounds (Θ), which ignore constant factors and low order terms
5. Model of computation
   1. Word-RAM: memory = array of w-bits random accessible words (32 bits -> about 4GB addressable)
   2. Computer operations that could be performed in constant time *O*(1) 
6. Design of algorithm
   * Brute Force
   * Decrease and Conquer
   * Divide and Conquer
   * Dynamic Programming
   * Greedy / Incremental