An algorithm is a set of instructions for accomplishing a task

## Binary search
Binary search is an algorithm; its input is a sorted list of elements and an item.
If an element you’re looking for is in that list, binary search returns the position
where it’s located. Otherwise, binary search returns null.

With binary search, you guess the middle number and eliminate half the
remaining numbers every time.
Binary search compares the target value to the middle element of the array

In general, for any list of n, binary search will take log<sub>2</sub> <sup>n</sup> steps to run 
To search through an list that contains 500 items

|             | Number |
| ----------- | ----------- |
| 2      | 500 r 0      |
| 2      | 125 r 0       |
| 2      | 62 r 1       |
| 2      | 31 r 0        |
| 2      | 15 r 1      |
| 2      | 7 r 1        |
| 2      | 3 r 1       |
| 2      | 1 r 1        |
| 2      | 0 r 1        |

which would give us 

log<sub>2</sub> <sup>2</sup><sup>9</sup>, which is 9 steps it would require for binary search

```python
class BinarySearch():

  def search(self, list_item, item):
    #sort item
    list_item.sort()
    print(list_item)
    low = 0
    high = len(list_item) - 1

    while low <= high:

        # ... check the middle element
        mid = (low + high) // 2
        guess = list_item[mid]
        # Found the item.
        if guess == item:
            return mid
            
      # The guess was too high.
        elif guess > item:
            high = mid - 1
            print(f"printing..{high}")
        # The guess was too low.
        else:
            low = mid + 1
            print(f"printing..{low}")
    # Item doesn't exist
    return None


search_item = BinarySearch()
my_list=[6,2,1,0,9,13,34,67,90]
second_list =[81,5,7,9,10]
print(search_item.search(my_list, 9))
print(search_item.search(second_list, 3))

```
Output :
```shell
[0, 1, 2, 6, 9, 13, 34, 67, 90]
4
[5, 7, 9, 10, 81]
printing..1
printing..-1
None
```
