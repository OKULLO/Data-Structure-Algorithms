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

- ## Mapping type (dict)
- ## Set

