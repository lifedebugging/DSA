```py
def sum_array(arr):
    if not arr:
        return 0
    
    new_arr = sorted(arr)[1 : -1]
    return sum(new_arr)
```    
