# Algorithm Analysis and Data Structures: Arrays vs. Linked Lists

This document outlines the fundamental concepts of Big O notation for algorithm analysis and provides a comparison between arrays and linked lists.

## 1. Big O Notation Rules

Big O notation is used to describe the efficiency and complexity of algorithms. [cite: 1] It helps us understand how the runtime or space requirements of an algorithm grow as the input size increases.

### 1.1 Constants Are Dropped

Big O notation ignores constant factors. [cite: 2]

* For example, an algorithm with a time complexity of 5n + 3 is simplified to O(n). [cite: 3]

### 1.2 Non-Dominant Terms Are Eliminated

Big O notation only considers the dominant term. [cite: 4]

* For example, an algorithm with a time complexity of n² + n is expressed as O(n²). [cite: 5]

### 1.3 Common Growth Rates

Here are some common Big O time complexities: [cite: 6]

* **O(1) - Constant Time:** The execution time does not depend on the input size (e.g., accessing an array element). [cite: 6, 7]
* **O(log n) - Logarithmic Time:** The runtime grows slowly as the input size increases (e.g., binary search). [cite: 7, 8]
* **O(n) - Linear Time:** The runtime increases linearly with the input size (e.g., iterating through an array). [cite: 8, 9]
* **O(n²) - Quadratic Time:** The runtime increases exponentially with the input size (e.g., nested loops). [cite: 9, 10]

### 1.4 Worst-Case vs. Best-Case Analysis

Big O notation typically describes the worst-case scenario. [cite: 10]

* For example, in searching an array:
    * Worst case: O(n) (element not found or at the end). [cite: 11]

### 1.5 Multiplication Rule

* Consecutive loops result in cumulative complexities. [cite: 12, 13]
* Nested loops also result in cumulative complexities. [cite: 13]
    * Example: A code snippet with nested loops, each iterating 'n' times, has a time complexity of O(n²). [cite: 13]

## 2. Arrays and Linked Lists

### Memory Allocation

* **Arrays:** Elements are stored in contiguous memory locations. [cite: 14]
* **Linked Lists:** Elements are stored in non-contiguous memory locations using dynamic memory allocation. [cite: 14]

### Performance

* **Arrays:** Provide faster access to elements by index (O(1)). [cite: 15]
* **Linked Lists:** Accessing elements requires traversal, resulting in O(n) access time. [cite: 15]

### Insertion

* **Arrays:** Insertion in the middle is time-consuming (O(n)). [cite: 16]
* **Linked Lists:** Insertion at the front is fast (O(1)) if the node pointer is available. [cite: 16]
