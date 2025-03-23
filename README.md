


1. Rules of Big O Notation in Algorithm Analysis
Big O notation is used to describe the efficiency of an algorithm in terms of both the time and the space complexity. Key rules include:
1.1. Take Constants
Big O ignores the dominant term and ignores the constants.
Eg. If an algorithm runs in 5n+35n + 35n+3 time, then in Big O notation, it would be O(n), ignoring the constant 5 and the additional 3.
1.2. Remove Non-Dominant Terms
We do not care about the maximal term within the complexity function.
Eg. Big O of n2+nn^2 + nn2+n is O(n²) because n2n^2n2 grows faster than nnn as nnn grows.
1.3. Multiple Growth Rates
Average time complexities are:
•	O(1) (Constant Time) Time taken by the function does not depend upon the input size. (i.e., accessing the array element)
•	O(log n) (Time: Logarithmic) - the running time increases gradually as nnn increases. (e.g., binary search)
•	O(n) (Linear Time): The time taken varies linearly with input size. (e.g., scanning through an array)
•	O(n²) (Quadratic Time): The running time grows exponentially with input size. (e.g., nested loops)
1.4. Worst-Case vs. Best-Case Analysis
Big O is the most extreme case that provides the performance ceiling.
Here.
In linear search:
•	Best case: O(1)O(1)O(1) (if the element is at the first position).
•	Worst case: O(n)O(n)O(n) (i.e., if the element does not exist or exists at the last
1.5. Multiplication Rule
If an algorithm has two loops sequentially, their complexities are added. If they are nested, the complexities are multiplied.
Sample:
•	Consecutive loops
C++
Copyedit
for(int i = 0; i <= n; i++) // O(n)
for(int j = 0; j < n; j++)  // O(n)
Its overall time complexity is O(n²).
2. Linked Lists vs Arrays
Memory Allocation
•	Arrays: Fixed consecutive memory allocation.
•	Linked Lists: Non-contiguous (dynamic memory allocation).
Performance
•	Arrays: Faster access by index O(1)O(1)
•	Linked lists: O(n) access because you have to traverse.
Insertion
•	Arrays: Time-consuming (O(n)O(n)O(n)) because
•	Linked Lists: Efficient (O(1)O(1)O(1) at the head,
Example:
Added the word
-	Array: To add an element in the middle, other elements must be shifted, so it's O(n)
-	Linked List: It is O(1) if the node pointer is given.
