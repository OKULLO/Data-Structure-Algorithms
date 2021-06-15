# Python contains various built-in data types. These include 
- ## Numeric types (int, float, complex, bool)
- ## Sequence types (str, list, tuple, range)
#### Common string methods 
| Syntax              | Description                   |
| -------------------- | ----------------------------  |                                    
| string.capitalize | Returns a string with only the first character capitalized |  
| string.endswith(substring,[start, end] |Returns True if a string ends with a specified substring |
| string.isalpha() | Returns True if all chars are alphabetic |
| string.replace(old,new[maxreplace]) | Replaces old substring with a new substring.|
| s.strip([characters])  | Removes whitespace or optional characters |

Strings, like all sequence types, support indexing and slicing.We can retrieve any character from a string by using its index
```python
name = "New York"
for i in enumerate (name[0 :6]) :
    print (i)
```
Output
```shell
(0, 'N')
(1, 'e')
(2, 'w')
(3, ' ')
(4, 'Y')
(5, 'o')
```
In Python, a string is immutable. You cannot overwrite the values of immutable objects. However, you can assign the variable again.
```python
print(name + " City")
```
Output
```shell
New York City
```
#### Common List methods 
List  can store any number of different data types. They are simple representations of objects and are indexed by integers
starting from zero
| Syntax              | Description                   |
| -------------------- | ----------------------------  | 
| li.append(x) | Appends element x at the end of list |
|li.count(x) | Returns the count of the occurrence of x in list |
| li.pop(i) |  Returns the element and Removes i  from the list, note i is index of object |
| li.sort(key,[reverse]) | Sorts list with optional key and reverses it.|

List can contain other nested list items
```python
for user_info in user_data:
    print (f"Name:{user_info[0]}, Age : {user_info[1]}")
```
Output:
```shell
Name:Ruth, Age : 60
Name:Max, Age : 90
Name:Joy, Age : 45
```
#### List comprehensions
List comprehension offers a shorter syntax when you want to create a new list based on the values of an existing list.
```python

name = "New York City".split()
print (name)
print ([i.lower() for i in name])
```
Output
```shell
['New', 'York', 'City']
['new', 'york', 'city']
```
- ## Mapping type (dict)
- ## Set

