first solution:
```
def quadrant(x, y):
    if x < 0 and y < 0:
        return 3
    elif x < 0:
        return 2
    elif y < 0:
        return 4
    else:
        return 1
    # Poveli!
    pass
```
Ternary expression:
```

def quadrant(x, y):
    return (3 if x<0 else 4) if y<0 else (2 if x<0 else 1)
```
