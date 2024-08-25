# Capture

## Problem Description

- Find factorial of a number n
- Assumption :- n>=0

## Solution Description -1 
- Pseudo code
	- Int res =1
	- Iterate var i from 2 to n
	- Multiply res with i storing it in res until and unless i<=n condition fulfilled.
- Code #code1
```python
def fact(n):
	res = 1
	for i in range(2,n+1):
		res = res*i
	return res
```
-  Time Complexity of solution $$\theta(n) = 1$$

## Solution Description -2
- Assumption $$n>=0$$
- Pseudo Code
	- Recursively call *fact(n)* which return *n X fact(n-1)*
	- 
- Code #code2
```python 
def fact(n):
	if n==0:
		return 1
	return n * fact(n-1)

```
- Time complexity of the function
$$ T(n) = T(n-1) + \theta(1)$$
	1. Work done at each level = $$\theta(1)$$
	2. No. of levels = $$n+1$$
	3. Total  Work done = $$\theta(1) * n = \theta(n)$$
	4. Space taken = $$\theta(n)$$ auxillary Space.
	5. Causes extra overhead space.

# Process

## Problem Description
Find the factorial of a number (n) assuming n>=0

Two Solutions present
1. Iterative Solution #code1
2. Recursive Solution #code2 

Better one is iterative solution 
- Iterative one gives time complexity of $$\theta(n)$$
- Recursive also gives time complexity of $$\theta(n)$$ with auxilliary space taken $$\theta(n)$$ due to the presence of #functioncallstack
- #functioncallstack 
	- Due to function stack which calls the function on each recursion.


