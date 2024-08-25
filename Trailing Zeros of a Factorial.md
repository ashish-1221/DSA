# Capture

## Problem Description
1.  Find the number of trailing zeroes of a factorial of number(n.
e.g. for n=5. The factorial is 120. The number of consecutive zeros from the unit's place is 1.similarly, for n=10. the factorial is 362800. The number of consecutive zeros from the unit's place is 2.

## Solution Description -1

 1. Code 1 #code1 
```python 
def fact(n):
    res = 1
    count = 0
    for i in range(2,n+1):
        res = res * i
        if (i%5==0)and (i>=5):
            count = count + 1
    return count
if __name__=="__main__":
    print(fact(10))
```
2. Pseudo code
	1. First calculate the factorial of a function in a for loop
	2. Initialize count =0
	3. Check if division of  the factorial by 10 gives remainder as  0
	4. if 0 then increment count
	5. divide factorial by 10
	6. Run step 3 again
	7. Return count
3. Problems with the code
	1. Time complexity of the code $$\theta(n)$$
	2. 