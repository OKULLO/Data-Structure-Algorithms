An algorithm is a set of instructions for accomplishing a task

## Binary search
Binary search is an algorithm; its input is a sorted list of elements and an item.
If an element you’re looking for is in that list, binary search returns the position
where it’s located. Otherwise, binary search returns null.

With binary search, you guess the middle number and eliminate half the
remaining numbers every time.
Binary search compares the target value to the middle element of the array

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
