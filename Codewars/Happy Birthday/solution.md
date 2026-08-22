My first simple solution:

```
def wrap(height, width, length):
    print(f"{height}, {width}, {length}")
    m = min(height, width, length)
    if m == height:
        return (length * 2 + width * 2 + height * 4) + 20
    elif m == width:
         return (length * 2 + height * 2 + width * 4) + 20
    else:
         return (height * 2 + width * 2 + length * 4) + 20
```

