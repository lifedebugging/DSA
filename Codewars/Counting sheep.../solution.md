first solution
```
def count_sheeps(sheep):
    count = 0
    for s in sheep:
        if ((True in sheep) and s):
            count +=1
    return count
        
```
one liner using .count()
```
def count_sheeps(sheep):
    return sheep.count(True)
```
