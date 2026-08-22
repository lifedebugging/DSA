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

However this solution is already O(1) time complexity (constant time) so the best i can do is make it more cleaner.

Using `sorted` built-in which **takes a list of number** and sort them from smallest to largest.
```
def wrap(height, width, length):
    short, med, long = sorted([height, width, length])
    return (short*4) + (med*2) + (long*2) + 20
```
