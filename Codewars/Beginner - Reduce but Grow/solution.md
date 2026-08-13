```
def grow(arr):
    num = 1
    for i in arr:
        num*= i
    return num
```
simplest solution

second solution
```
import math
def grow(arr):
    return math.prod(arr)
```
One liner using `reduce`
```
from functools import reduce
def grow(arr):
    return reduce(lambda x, y: x*y, arr)
    ```
