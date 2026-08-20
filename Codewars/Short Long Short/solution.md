```
def solution(a, b):
    return "".join(b+a+b if len(a) > len(b) else a+b+a)
```
