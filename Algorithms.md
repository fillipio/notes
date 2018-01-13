## General
- Swapping need caching of one of the items, even in recursion
- Think of objects to cache stuff for later, O(c) lookup

## Topics
### Array

### Hash Table

Linked List,Math,Two Pointers,String,Binary Search,Divide and Conquer,Dynamic Programming,Backtracking,Stack,Heap,Greedy,Sort,Bit Manipulation,Tree,Depth-first Search,Breadth-first Search,Union Find,Graph,Design,Topological Sort,Trie,Binary Indexed Tree,Segment Tree,Binary Search Tree,Recursion,Brainteaser,Memoization,Queue,Minimax,Reservoir Sampling,Map,Geometry"

## Leetcode
#### Intersection of two arrays:
- Learnt about Set ( list of values, unique )
- came up with O(n^2) with forEach / Map / indexOf
- O(n) solution with Set
#### Median of two sorted arrays
- Median is based on count
- Simple O(n+m) solution is to merge the arrays (Merge sort merge step), then lookup the median
- O(log(n+m)) solution is required, so divide and conquer
- start at the center of both the arrays (depends on length of both arrays)
- get rid of array-length/2 input space on each step
- ** logic: find the point at which all items of [...left1, ...left2] are less than [...right1, ...right2]
  - check for: ...left1 < ...right2  and ...left2 < ...right1
  - if not, move the pointers by reducing the input size to half ( ~binary search )
#### Backtracking
- choose, explore and unchoose (draw parallels to depth first search)
- problems like permute, anagrams, dice roll can be solved
- permute: length l and options o => O(options ^ length)
- for example
  - anagram of a string of length n => options n, length n => O(n^n) ? or O( n * n! ) ?
  - rolling a dice O( 6 ^ n ) ?

