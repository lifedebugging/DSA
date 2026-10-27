```py
def two_sort(array):
    # your code here
    #use sorted() to sort the list alphabatically
    #loop over first elem list[0]
    #use join to add concatenate star as separator in word
    sorted_arr = sorted(array)
    return "***".join(char for char in sorted_arr[0])
```
