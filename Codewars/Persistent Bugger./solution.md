first solution
```py
import math
def persistence(n):
    # split n
    #multiply the splitted n
    #grab the result from n and split again
    #keep doing it until only x a single digit is left
    
    result = list(map(int, str(n)))
    counter = 0
    while len(result) >= 2:
            result = math.prod(result)
            result =  list(map(int, str(result)))
            counter += 1
    return counter
```
