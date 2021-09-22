Mapreduce is a parallel algorithm .

### The map function
The map function is simple: it takes an array and applies the same
function to each item in the array. 

```python
names = ['Anne', 'Amy', 'Bob', 'David', 'Carrie', 'Barbara', 'Zach']
lengths = map(len, names)
print (list(lengths))


arr1 = [1, 2, 3, 4, 5]
arr2 = map(lambda x: x**3, arr1)
print(list(arr2))
``` 
Output 
```shell
[4, 3, 3, 5, 6, 7, 4]
[1, 8, 27, 64, 125]
```

### The reduce function
With reduce,it reduces a whole list of items down to one item. With map, you go from
one array to another.
```python
from functools import reduce
lists= [1, 2, 3, 4, 5]
r = reduce(lambda x,y: x+y, lists)
print(r)
```

Output
```shell
15
```
