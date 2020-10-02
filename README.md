# Data-Structures-and-algorithms
### Hello World! :wave:
This repository will be my documentation while I learn Data structures and algorithms.
I will add my solved problems here :smile:

## Binary Search
https://www.topcoder.com/community/competitive-programming/tutorials/binary-search/
### Beyond arrays: the discrete binary search <br>
This is where we start to abstract binary search. A sequence (array) is really just a function which associates integers (indices) with the corresponding values. However, there is no reason to restrict our usage of binary search to tangible sequences. In fact, we can use the same algorithm described above on any monotonic function f whose domain is the set of integers. The only difference is that we replace an array lookup with a function evaluation: we are now looking for some x such that f(x) is equal to the target value. The search space is now more formally a subinterval of the domain of the function, while the target value is an element of the codomain. The power of binary search begins to show now: not only do we need at most O(log N) comparisons to find the target value, but we also do not need to evaluate the function more than that many times. Additionally, in this case we aren’t restricted by practical quantities such as available memory, as was the case with arrays.
<br>

What we can call the main theorem states that binary search can be used if and only if for all x in S, p(x) implies p(y) for all y > x. This property is what we use when we discard the second half of the search space. It is equivalent to saying that ¬p(x) implies ¬p(y) for all y < x (the symbol ¬ denotes the logical not operator), which is what we use when we discard the first half of the search space. The theorem can easily be proven, although I’ll omit the proof here to reduce clutter. <br>

These two parts are most often interleaved: when we think a problem can be solved by binary search, we aim to design the predicate so that it satisfies the condition in the main theorem.

## Merge Sort
The principle aspect involved in merge sort is a merge function which merges two sorted arrays and forms a final array that contains elements from both the arrays in a sorted fashion. It is quite fascinating how a simple merge function can be used to solve one of the most sought-after problems in Computer Science i.e. sorting, in one of the most efficient ways possible. The time complexity of merge sort is O(n log n). It is a divide-and-conquer algorithm. Merge sort continuously breaks down an array into several subarrays until each subarray consists of a single element and merging those subarrays repeatedly forms a sorted array at the end. Merge sort can be used to solve several important problems with ease. Some of the most famous problems that can be solved using merge sort are counting the number of inversions and efficiently sorting large datasets on computers with small RAMs.
### Other Resources:
https://www.geeksforgeeks.org/merge-sort/
<br>
