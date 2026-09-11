```
def area_or_perimeter(l , w):
    return (2*(l + w)) if l != w else l*w
    # return your answer
```
without if/else
```
area_or_perimeter = lambda x, y: (x!=y) * (2*(x +y)) + (x==y) *(x*x)
```
