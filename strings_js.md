# Javascript String notes
- Create: `const str1 = "This is a string primitive"; const str2 = new String("This is a string object"`
- Read: `const fifthLetter = str1.charAt(4); const fifthLetter = str1[4];`
  - array-like str1[n] format can only read, cannot update or delete
  - charAt can be negligibly faster but more unpredictable, Eg: `str1.charAt(undefined)` will return the first char
  - go with str[n] format for non IE6 / 7 environments
- Update: string primitives are immutable. use slice to create a new string
  - `str.slice(0, n) + "diff" + str.slice(n)`
- Delete: same as above 
  - Delete char at n: `str.slice(0, n) + str.slice(n+1)`
  
## Tips
- get int equivalent for characters:
   - str.charCodeAt(0) - 97 // a: 0, b: 1..
   - str.charCodeAT(0) - 65 / A: 0, B: 1 ..
