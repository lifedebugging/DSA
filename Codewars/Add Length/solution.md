my first working code:
```
def add_length(str_):
    splitted = str.split(str_)
    new = []
    for s in splitted:
        new.append(f"{s} {len(s)}")
    
    return new
    #your code here
```
one liner:
```
def add_length(str_):
    return [f"{s} {len(s)}" for s in str_.split()]
```
