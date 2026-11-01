```py
import math
def cockroach_speed(s):
    # convert km/h to cm/second
    return math.floor(s * 100000 / 3600)
```
or 
```
def cockroach_speed(s):
    return s // 0.036
```
