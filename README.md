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

### Worst, Average and Best Cases

Any algorithm can be analysed using 3 cases:
1. **Best Case** - Refers to **Minimum time** taken by the algorithm to complete
2. **Average Case** - Refers to **Average time** taken by the algorithm to complete
3. **Worst Case** - Refers to **Maximum time** taken by the algorithm to complete

For a **linear search algorithm**, in which we search a value in an array one by one here are the three cases:

Let us assume we have an array of *n* items and we have to search for the value *x*

**Best Case** - In the linear search problem, the best case occurs when x is present at the first location. The number of operations in the best case is constant (not dependent on n). So time complexity in the best case would be Θ(1) 

**Worst Case** - For Linear Search, the worst case happens when the element to be searched (*x* in the above code) is not present in the array. In such a scenario *x* is compared with all the elements of array one by one. Therefore, the worst case time complexity of linear search would be Θ(n).

**Average Case** - In average case analysis, we take all possible inputs and calculate computing time for all of the inputs. Sum all the calculated values and divide the sum by total number of inputs. We must know (or predict) distribution of cases. For the linear search problem, let us assume that all cases are uniformly distributed (including the case of *x* not being present in array). So we sum all the cases and divide the sum by (n+1).

`Average Case for Linear Search = Σ Θ(i)/(n+1), where 1<= i<= n+1`
`=Θ(n)`

Most of the times, we do worst case analysis to analyze algorithms. In the worst analysis, we guarantee an upper bound on the running time of an algorithm which is a good metric to determine the performance of an algorithm in a real world scenario. 
The average case analysis is not easy to do in most of the practical cases and it is rarely done. In the average case analysis, we must know (or predict) the mathematical distribution of all possible inputs. 
The Best Case analysis is useless. Guaranteeing a lower bound on an algorithm doesn’t provide any information as in the worst case, an algorithm may take years to run.

### Asymptotic Notations

These notations are mathematical functions which determine the time complexity of an algorithm. The following 3 asymptotic notations are mostly used to represent time complexity of algorithms.

**Θ Notation:** - Theta Notation is used to find the average case time complexity of an algorithm. It represents the most accurate asymptotic behavior. It bounds a function from above and below.

 Mathematically it is represented as:
 `Θ(g(n)) = {f(n): there exist positive constants c1, c2 and n0 such that 0 <= c1*g(n) <= f(n) <= c2*g(n) for all n >= n0}`

**Big O Notation:** - Big O Notation is used to find the worst case time complexity of an algorithm. It bounds a function only from above, which means Big O function is the maximum time taken by the algorithm to complete.

Mathematically it is represented as:
 `O(g(n)) = {f(n): there exist positive constants c and n0 such that 0 <= f(n) <= c*g(n) for all n >= n0}`

**Ω Notation:** - Omega Notation is used to find the best case time complexity of an algorithm. It bounds a function only from below, which means Ω function is the minimum time taken by the algorithm to complete. As discussed, the best case performance of an algorithm is generally not useful, the Omega notation is the least used notation among all three.

Mathematically it is represented as:
 `Ω(g(n)) = {f(n): there exist positive constants c and n0 such that 0 <= c*g(n) <= f(n) for all n >= n0}`

**Properties of Asymptotic Notations :**

 1. **General Property:** 
 If f(n) is O(g(n)) then v*f(n) is also O(g(n)) ; where v is a constant.
 Similarly this property is true for both Θ and Ω notation.

 2. **Reflexive Property:** 
 If f(n) is given f(n) = O(g(n)).
 Similarly this property is true for both Θ and Ω notation.

 3. **Transitive Property:** 
 If f(n) is O(g(n)) and g(n) is O(h(n)) then f(n) = O(h(n)).
 Similarly this property is true for both Θ and Ω notation.

 4. **Symmetric Property:** 
 If f(n) is Θ(g(n)) then g(n) is Θ(f(n)).
 This property is not true for both O and Ω notation.

 5. **Transpose Symmetric Property:** 
 If f(n) is O(g(n)) then g(n) is Ω (f(n)).
 This property only satisfies for O and Ω notations.
 
 ### Big-O Cheatsheet
 To save your time hunting, here is a useful poster showing time and space complexities of famous data structures and algorithms provided by [Big-O Cheat Sheet](https://www.bigocheatsheet.com/)
