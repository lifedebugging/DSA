first working solution:
```
def longest(a1, a2):
    new = (a1,a2)
    joined = "".join(new)
    return "".join(sorted(set(joined)))
    # your code
```
better solution:
```
def longest(a1, a2):
    return "".join(sorted(set(a1+a2)))
```
