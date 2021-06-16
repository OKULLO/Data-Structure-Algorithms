Big O notation
Big O notation is special notation that tells you how fast an algorithm is

O<sub>n</sub> 
where
```
O is big Notation
n is number of operations( your algorithms)

```

Here are five Big O run times that you’ll encounter a lot, sorted from
fastest to slowest:
|    O notatation | Explantion |
| ----------- | ----------- |
| O(log n)| Binary search|
|O n |Simple search known as linear time|
|O (n * log n) | Quicksort (fast sorting)|
|O n<sup>2</sup>|selection sort (slow sorting)|
|O (n !) |traveling salesperson (the slowest)|

Let me explain with a simple example, you want to carry out a task that requires 32 steps , let's see which would be the fastest
|             | Number |
| ----------- | ----------- |
| 2      | 32 r 0           |
| 2      | 16 r 0           |
| 2      | 8 r 0            |     
| 2      | 4 r 0            |
| 2      | 2 r 0            |
|        | 1 r 0             |

log<sub>2</sub> 32<sup> = log<sub><del>2</del></sub> <del>2</del><sup>5</sup>


|Number of steps | O(log n) |O n |O (n * log n) | O n<sup>2</sup> | O (n !) |
| ----------- | ----------- |----------- | ----------- |----------- | ----------- |
|32|5 |    32 |32 * 5 = 160| 32<sup>2</sup> = 1024 |  32! = 32 * 32 * 31 * 30 * ...1 = 2.631308369 <sup>E+35 </sup> |

   
