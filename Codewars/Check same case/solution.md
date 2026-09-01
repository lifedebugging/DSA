```
def same_case(a, b):
    if not (a.isalpha() and b.isalpha()):
        return -1
    elif a.islower() and b.islower() or a.isupper() and b.isupper():
        return 1
    else:
        return 0
        
        
    # your code here
    pass
```
one liner:
```
def same_case(a, b):
    return -1 if not (a.isalpha() and b.isalpha()) else 1 if a.islower() and b.islower() or a.isupper() and b.isupper() else 0
```
other solution:
```
def same_case(a, b):
    return a.isupper() == b.isupper() if a.isalpha() and b.isalpha() else -1
```
