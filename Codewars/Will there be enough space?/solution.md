```py
def enough(cap, on, wait):
    if (on + wait) <= cap:
        return 0
    else:
        return ((on + wait) - cap) 
    # Your code here
```
and
```py
def enough(cap, on, wait):
    if  not (on + wait) <= cap:
        return ((on + wait) - cap)
    return 0
    # Your code here
```
and
```py
def enough(cap, on, wait):
    return max(0, wait-(cap-on))
```
