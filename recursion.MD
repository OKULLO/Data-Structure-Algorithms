Recursion is a process by which a function calls itself directly or indirectly. 

Every recursive function has two parts: 
1. the base : is when the function doesn’t call itself again so it doesn’t go into an infinite loop, the role of the base is to stop a recursive function from executing endlessly – once a pre-specified base condition is met, the function knows it’s time to exit.
2. the recursive case. The recursive case is when the function calls itself

```python

def fun(a, b):
    if (b == 0):  #base case
        return 0
    if (b % 2 == 0):
        return fun(a * a, b//2)
     
    return fun(a * a, b//2) + a #recursive case

print(fun(4, 7))
print(fun(4, 8))
 
```
Output
```shell
276
65536

```
 