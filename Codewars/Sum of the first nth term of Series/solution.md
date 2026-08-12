The solution is 
```
def series_sum(n):
    # Happy Coding ^_^
    s = []
    for i in range(0, n):
        s.append(1/(i*3+1)) 
    return '{:.2f}'.format(sum(s))
```

If u can't figure out just look up the math formula and apply the logic

Error resolved: `TypeError: 'float' object is not iterable`
which is basically converting s to an empty list 
