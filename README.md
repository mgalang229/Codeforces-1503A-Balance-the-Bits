# Codeforces-1503A-Balance-the-Bits
Link: https://codeforces.com/problemset/problem/1503/A
### Test Case
<b>Sample Input:</b>
```
1
18
100110011000110001
```
<b>Sample Output:</b>
```
YES
()((()(())()))()()
(()((()()()()))())
```
### Explanation
```
1 0 0 1 1 0 0 1 1 0 0 0 1 1 0 0 0 1
? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? => a
? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? => b

"if" part in the code: 
1 0 0 1 1 0 0 1 1 0 0 0 1 1 0 0 0 1
( ? ? ( ( ? ? ( ) ? ? ? ) ) ? ? ? ) => a
( ? ? ( ( ? ? ( ) ? ? ? ) ) ? ? ? ) => b

note: there are 8 "1"s so 4 must be open brackets and the remaining must be closing brackets

"else" part in the code:
1 0 0 1 1 0 0 1 1 0 0 0 1 1 0 0 0 1
( ) ( ( ( ) ( ( ) ) ( ) ) ) ( ) ( ) => a
( ( ) ( ( ( ) ( ) ( ) ( ) ) ) ( ) ) => b

string "a" should be alternating ), (, ), (, ...
string "b" should be alternating (, ), (, ), ...
```
