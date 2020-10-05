# Data Structures and Algorithms in Javascript
This repository contains popular data structures and algorithms implemented in Javascript. Also included is a test file with every problem statement to verify whether it passes the testcases.  
  
Each data-structure and algorithm will also contain a readme file to explain the necessary concepts as well as the approach to be followed for solving the problem. At the end, the space and time complexities will also be mentioned for the solution.  
  
🎉 If you are a beginner Javascript developer I hope you will learn a lot from this repository. If you are an experiencied developer I hope you could find something useful.  
  
All contributions to this repository is welcomed with ❤️  
  
## Quick Overview of Data Structures and Algorithms

A **data structure** is a particular way of organizing data in a computer so that it can be used effectively. This is particularly important when we have to deal with large amounts of data. If we do not posses the knowledge of common data structures, our programs will consume a lot of space in the memory and will be very difficult to access. 

For example, suppose we have to store a bank statement of a customer. By using arrays we can store it easily. This helps in reducing the use of number of variables as we don’t need to create a separate variable for every credit or debit. All records can be accessed by simply traversing the array.

Data Structures that we will discuss in this repository are: 

- [Array](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Matrix](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [LinkedList](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Stack](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Queue](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Graph](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Binary Tree](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Binary Search Tree](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Hashing](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Heaps](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Segment Tree](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [AVL Tree](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Binary Indexed Tree](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Red Black Tree](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Trie](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Suffix Array and Suffix Tree](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Splay Tree](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [B Tree](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [K Dimensional Tree](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Advanced Lists](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
- [Other Advanced Data Structures](https://github.com/rahulSlash/data-structures-algorithms-javascript)  
---
An **algorithm** is a set of finite and well-defined instructions, typically to solve a class of problems or to perform a computation. Algorithms are a very important topic in Computer Science because they help software developers create efficient and error free programs. The most important thing to remember about algorithms is that there can be many different algorithms for the same problem, but some are much better than others.

Computers are incredibly fast at manipulating, moving and looking through data. However the amount of data computers use is often so large that it doesn't matter how fast the computer is, it will take it far too long to examine every single piece of data (companies like Google, Facebook and Twitter routinely process billions of things per day, and in some cases, per minute!). This is where algorithms come in. If a computer is given a better algorithm to process the data then it doesn't matter how much information it has to look through, it will still be able to do it in a reasonable amount of time. [Further Reading...](https://csfieldguide.org.nz/en/chapters/algorithms/)

### Asymptotic Analysis of Algorithm

Analysing Algorithm is a process of **measuring the performance** of a certain algorithm. One way to do it is to run two different algorithms for different inputs and see which one performs better. However, for some inputs, first algorithm performs better than the second and for some inputs second performs better. Also, for some inputs, first algorithm perform better on one machine and the second works better on other machine for some other inputs.

In Asymptotic Analysis, we evaluate the performance of an algorithm in terms of input size. We calculate, how the time (or space) taken by an algorithm increases with the input size.

For eg. Let us take two sorting algorithms Linear Search **LS**(growth is linear) and Binary Search **BS**(growth is logarithmic) to search a value in a sorted array. Let us say we have a fast machine **A** with a constant **0.2**  and a slow machine **B** with a constant **1000** which means that A is 5000 times more powerful than B. **A** runs **LS** and **B** runs **BS**. For a small sized array, A will complete faster but beyond a cetain size of array **B** will take less time.

**Linear Search running time in seconds on A: 0.2 * n  
Binary Search running time in seconds on B: 1000*log(n)**

Here is the proof:
| Input size(n)      | LS in A  | BS in B  | 
| -----------        | -------- | -------- |
| 10                 | 2 sec    | ~1 hr    |
| 100                | 20 sec   | ~1.8 hr  |
| 10^6               | ~55 hr   | ~5.5 hr  |
| 10^9               | ~6.3 yr  | ~8.3 hr  |


