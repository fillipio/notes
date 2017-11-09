## General
- Swapping need caching of one of the items, even in recursion
- Think of objects to cache stuff for later, O(c) lookup

## Leetcode
#### Intersection of two arrays:
- Learnt about Set ( list of values, unique )
- came up with O(n^2) with forEach / Map / indexOf
- O(n) solution with Set
#### Backtracking
- choose, explore and unchoose (draw parallels to depth first search)
- problems like permute, anagrams, dice roll can be solved
- permute: length l and options o => O(options ^ length)
- for example
  - anagram of a string of length n => options n, length n => O(n^n) ? or O( n * n! ) ?
  - rolling a dice O( 6 ^ n ) ?

