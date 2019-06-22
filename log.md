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
TEMPLATE
### Day X: 11/06/2019 Tuesday

**Today's Progress**:

**Link(s) to work**
