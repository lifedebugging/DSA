```py
from collections import Counter

def is_valid_walk(walk):
    #so if the number of blocks walked equal its true
    #if the number of each direction is exactly two also true
    if len(walk) != 10:
        return False
    counts = Counter(walk)
    return counts['n'] == counts['s'] and counts['e'] == counts['w']

```
or GRID simulation
```py
def is_valid_walk(walk):
    if len(walk) != 10:
        return False
    
    x, y = 0,0
    for move in walk:
        if move == "n" : y +=1
        if move == "s" : y -=1
        if move == "e" : x +=1
        if move == "w" : x -=1
    return x == 0 and y == 0
    

```
