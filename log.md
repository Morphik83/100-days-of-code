# 100 Days Of Code - Log

### Day 1: 10/06/2019 Monday
**Today's Progress**: 
1. Alg: Level Order Traversal 
- hints: add node to search queue, use levelsize + while within while (while search queue, while levelsize)
2. Alg: Merge Intervals
- hints: 6 cases, better to sort on start, use class Interval(start, end) 

**Thoughts**
Its my another attempt to complete 100 days of coding. This time I'd like to improve on coding-interview skills.  

**Link(s) to work**
1. [BST Level-Order Traversal](https://www.educative.io/collection/page/5668639101419520/5671464854355968/5726607939469312)
2. [BST Level-Order Traversal](https://www.hackerrank.com/challenges/30-binary-trees/problem)
3. [Merge Intervals](https://www.educative.io/collection/page/5668639101419520/5671464854355968/5652017242439680)

---
### Day 2: 11/06/2019 Tuesday
**Today's Progress**:
1. Abstract Base Classes: 
https://www.python-course.eu/python3_abstract_classes.php
2. Alg: Remove Duplicates from linked list
- hints: two pointers, as long as slow.data == fast.data, keep moving f = f.next, then s.next = f, two whiles (while s.next !=None, while f!=None and s.d == f.d)

**Link(s) to work**
1. [Abstrac Classes](https://www.hackerrank.com/challenges/30-abstract-classes/problem)
2. [Remove Duplicates from linked list](https://www.hackerrank.com/challenges/30-linked-list-deletion/problem)

---
### Day 3: 12/06/2019 Wednesday
**Today's Progress**:
1. review prev days 
2. Alg: Reverse Linked List
- hints: two pointers (prev, curr), use temp to store temp=curr.next
3. Prime numbers

**Link(s) to work**
1. [Reverse Linked List](https://www.educative.io/collection/page/5668639101419520/5671464854355968/4519653420302336)
2. [Prime Numbers](https://www.hackerrank.com/challenges/30-running-time-and-complexity/problem?isFullScreen=false)

---
### Day 4: 13/06/2019 Thursday
**Today's Progress**:
1. Nested Logic 
2. Max subarray of size k

**Link(s) to work**
1. [Nested Logic](https://www.hackerrank.com/challenges/30-nested-logic/problem)
2. [Max subarray of size k](https://www.educative.io/collection/page/5668639101419520/5671464854355968/5177043027230720)

---
### Day 5: 14/06/2019 Friday
**Today's Progress**:
1. Average of all subarrays of size K
2. Attempted to resolve 'Power of Thor - episode 1', but managed to resolve 
only 2/4 cases. 

**Link(s) to work**
1. [Average of all subarrays of size K](https://www.educative.io/collection/page/5668639101419520/5671464854355968/6658855733821440)
2. [Power of Thor - episode 1](https://www.codingame.com/ide/puzzle/power-of-thor-episode-1)

---
### Day 6: 15/06/2019 Saturday
**Today's Progress**:
1. Static methods vs. class methods
2. Testing
3. Max Sum Subarray of Size K
- hints: window_start=0, window_end=0, itarate over arr until we >= k-1, then
check curren_sum > max_sum, then subtract first element and add next element.

**Link(s) to work**
1. [static vs. class](https://stackoverflow.com/questions/12179271/meaning-of-classmethod-and-staticmethod-for-beginner?rq=1)
2. [static vs. class](https://www.programiz.com/python-programming/methods/built-in/staticmethod)
3. [testing](https://www.hackerrank.com/challenges/30-testing)
4. [Max Sum Subarray of Size K](https://www.educative.io/collection/page/5668639101419520/5671464854355968/5177043027230720)

---
### Day 7: 16/06/2019 Sunday
**Today's Progress**:
1. study bit operations (alg: bits_power_of_two, )
2. all_subsets_of_a_set
- hints: for n-len array, there are 2^n subsets. generate masks (for i in range(1<<n)) 
then check where 1's are in each mask (for i in range(n))  
(mask>>i)&1 and if true, add a[i] to subset. 
3. count set bits (x&(x-1))

**Link(s) to work**

---
### Day 8: 17/06/2019 Monday
**Today's Progress**:
1. Repeat all from last 7 days 
2. (Two pointers) Pair with Target Sum (in *sorted* array)
- hints:  two pointers, one at start, second at end. if arr[st] + arr[end] bigger
than target_sum, then decrease end pointer, otherwise, increment start pointer. 
- hints: hash table (store val:index and search for target-num == val)

**Link(s) to work**
1. [Pair with Target Sum](https://www.educative.io/collection/page/5668639101419520/5671464854355968/6618310940557312)

---
### Day 9: 18/06/2019 Tuesday
**Today's Progress**:
1. bitwise AND

**Thoughts**: I am stuck with this problem

**Link(s) to work**
1. [bit wise AND](https://www.hackerrank.com/challenges/30-bitwise-and/problem)

---
### Day 10: 19/06/2019 Wednesday
**Today's Progress**:
1. bitwise AND

**Thoughts**: 
Eventually I made it - stupid small mistake ... this throws Timeout! both ifs are evaluated in each iteration:
```python
if max_so_far < m < k:
  max_so_far = m
if max_so_far == k-1:
  return max_so_far
```

this works, as second 'if' is evaluated only when first 'if' is true, so number of operations here goes down by ~50% 
```python
if max_so_far < m < k:
  max_so_far = m
  if max_so_far == k-1:
    return max_so_far
```
**Link(s) to work**
1. [bit wise AND](https://www.hackerrank.com/challenges/30-bitwise-and/problem)

---
### Day 11: 20/06/2019 Thursday
**Today's Progress**:
1. Linked Lists: has_cycle(head), find_cycle_length(head)  
-hints: slow pointer, fast pointer - if has_cycle, they meet  
-hints: length: if has_cycle => save meet_node and count how many times slow pointer needs to move to reach meet_node again

**Link(s) to work**
1. [LinkedList: has_cycle and find_cycle_length](https://www.educative.io/collection/page/5668639101419520/5671464854355968/6556337280385024)

---
### Day 12: 22/06/2019 Saturday
**Today's Progress**:
1. Cyclic Sort

**Link(s) to work**
1. [Cyclic Sort](https://www.educative.io/collection/page/5668639101419520/5671464854355968/6003980930908160)

---
### Day 13: 23/06/2019 Sunday
**Today's Progress**:
1. Continue with Cyclic Sort 
-hints: 1. check if nums[i]==i-1 (assign j=nums[i]-1 and check if nums[i]==nums[j])
if not equal, then move swap swap(nums, i, j) - by swapping be put value in index j in the sorted position. At the same time we keep checking if nums[i]==i-1, if true, we move to the next i (while i < len(nums))
-hints: 2. keep two variables (x=nums[i] and temp=nums[i-1])

**Link(s) to work**
1. [Cyclic Sort - 3 solutions](https://www.educative.io/collection/page/5668639101419520/5671464854355968/6003980930908160)

---
### Day 14: 24/06/2019 Monday
**Today's Progress**:
1. Revise last 13 days  
2. Find the median of a number stream  

**Thoughts**
did not finish alg question - started to read about heap and how to use it

**Link(s) to work**
1. [find a median of a number stream](https://www.educative.io/collection/page/5668639101419520/5671464854355968/6308926461050880)

---
### Day 15: 25/06/2019 Tuesday
**Today's Progress**:
1. arr of strictly positive int - find indx where left_sum == right_sum  
2. subsets (powerSet)  
-hints: bitwise (see day 7) or BFS

**Link(s) to work**
2. [Subsets](https://www.educative.io/collection/page/5668639101419520/5671464854355968/5670249378611200)

---
### Day 16: 26/06/2019 Wednesday
**Today's Progress**:
1. subsets (powerSet)  
-hints: BFS. Iterate over num in nums -> check length (n) of results array so far -> iterate over 'so far' created subsets n-times -> create a copy of exisiting subset and append 'num' to a copy to create new subset -> append subset to results -> pick next num -> check length n of results -> iterate n-times over results and create new subsets ... etc.
2. BST: height (1+ max(height(root.left), height(root.right)))
3. Binary Tree Path Sum

**Link(s) to work**
1. [Subsets](https://www.educative.io/collection/page/5668639101419520/5671464854355968/5670249378611200)
2. [binary-search-trees](https://www.hackerrank.com/challenges/30-binary-search-trees/tutorial)
3. [Binary Tree Path Sum](https://www.educative.io/collection/page/5668639101419520/5671464854355968/5642684278505472)

---
### Day 17: 27/06/2019 Thursday
**Today's Progress**:
1. DFS: Binary Tree Path Sum  
-hints: recursively check if node is a leaf node and if its value == sum.  
At each call (if node is not a leaf), subtract from sum -= node.val,  
and go (has_path(node.left, sum - node.val) or has_path(node.right, sum - node.val))

**Link(s) to work**
1. [DFS: Binary Tree Path Sum](https://www.educative.io/collection/page/5668639101419520/5671464854355968/5642684278505472)

---
### Day 18: 28/06/2019 Friday
**Today's Progress**:
1. (only count) All paths for a sum  
-hints: keep track of variable count - if path found, increae count by 1. return count var from each (recursive) call. If root is None, return 0. No need to use backtracking.

**Link(s) to work**
1. [All paths for a sum](https://www.educative.io/collection/page/5668639101419520/5671464854355968/5675214360805376)

---
### Day 19: 29/06/2019 Saturday
**Today's Progress**:
1. (find actual paths) All paths for a sum  
-hints: not the same as yesterday, as today we keep track of the nodes that sum up to given sum. To do that we need to backtrack visited nodes. Function call has 4 args(currNode, sum, currPath, allNodes). currNode is either left or right child, sum is decreased with each recursive call by the node.val, currPath is updated with each function call (either append if going down the tree or del when going up the tree). allPaths is updated with currPath only when we find such path where all the node's values sum up to given sum.

**Link(s) to work**
1. [All paths for a sum](https://www.educative.io/collection/page/5668639101419520/5671464854355968/5714315743068160)

---
### Day 20: 30/06/2019 Sunday
**Today's Progress**:
1. Order-agnostic Binary Search 

**Link(s) to work**
1.[Order-agnostic Binary Search](https://www.educative.io/collection/page/5668639101419520/5671464854355968/6304110192099328)

---
### Day 21: 01/07/2019 Monday
**Today's Progress**:
1. Resolved problem from yesterday (Order-agnostic Binary Search )
2. started to read about heap in Python and related issues.

**Link(s) to work**
1. [Top K numbers](https://www.educative.io/collection/page/5668639101419520/5671464854355968/5728885882748928)

---
### Day 22: 02/07/2019 Tuesday
**Today's Progress**:
1. Revise algorithms studied so far.

---
### Day 23: 03/06/2019 Wednesday
**Today's Progress**:
1. Read about HEAPs in Python 
2. Merge K-sorted Linked Lists
-hints: brute force. add all elements of all linked lists to one list and sort it. 

** Thoughts  
Today I did brute force - tomorrow, rewrite with heapq

**Link(s) to work**
1. [Heap](https://www.tutorialspoint.com/python/python_heaps.htm)
2. [Merge k-sorted linked lists](https://www.educative.io/collection/page/5668639101419520/5671464854355968/4611799594827776)

---
### Day 24: 04/07/2019 Thursday
**Today's Progress**:
1. Heapq [heapify, heappush, heappop, heappushpop, heapreplace(first pop then push!), nlargest, nsmallest]
2. Rich comparisons in Python: Classes can define new special methods __lt__, __le__, __eq__, __ne__, __gt__, __ge__ to override the corresponding operators. (I.e., <, <=, ==, !=, >, >=)
3. Solved Merge K-sorted Linked Lists with heap

**Link(s) to work**
1. [Merge k-sorted linked lists](https://www.educative.io/collection/page/5668639101419520/5671464854355968/4611799594827776)

---
### Day 25: 06/07/2019 Saturday
**Today's Progress**:
1. Started to read about Knapsack problem 

**Link(s) to work**
1. [Knapsack](https://www.educative.io/collection/page/5668639101419520/5671464854355968/5008218180812800)

---
### Day 26: 07/07/2019 Sunday
**Today's Progress**:
1. Greedy alg: Set_covering_problem  
-hints: from book 'Grokking algorithms', p.146 (radio stations)
2. 0-1 Knapsack Problem with Memoization   

**Link(s) to work**
2. [Knapsack](https://www.educative.io/collection/page/5668639101419520/5671464854355968/5008218180812800)
2a. [good YT explanation of Knapsack with memoization](https://www.youtube.com/watch?v=xOlhR_2QCXY)




---
TEMPLATE
### Day X: 11/06/2019 Tuesday

**Today's Progress**:

**Link(s) to work**

