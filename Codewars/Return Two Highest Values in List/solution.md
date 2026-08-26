my first solution:
```
def two_highest(arg1):
    if len(arg1) > 2:
        arg = list(set(arg1))
        arg.sort(reverse=True)
        return arg[:2]
    else:
        arg = list(set(arg1))
        arg.sort(reverse=True)
        return arg
        
    pass
```

more efficient:

```
def two_highest(arg1):
    arg = list(set(arg1))
    arg.sort(reverse=True)
    return arg[:2] if len(arg1) > 2 else arg
        
    pass
```
OR
```
def two_highest(arg1):
    return sorted(set(arg1), reverse=True)[:2]
```
set(arg1) Removes duplicates

.sorted(..., reverse=True) Sorts unique numbers from highest to lowest and returns a new 

list.[:2] Safely slices the top 2 (or fewer if less than 2 exist).
