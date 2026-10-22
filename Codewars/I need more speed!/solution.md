```py
import numpy as np
def reverse(seq): 
    # your code here
    #reverse the sequence but i cannot use builtins amd slicing
    #and it has to be fast
    #i can create new empty list but i cannot use empty list as well, take an elem out using //10
    #append in new empty list
    #and discard using %10
    # not working
    # trying np.fliplr
    # not working
    #trying while loop with replacing left and right and incrementing 1 to left and decrementing 1 to right
    left, right = 0, len(seq) - 1
    while left < right:
        seq[left], seq[right] = seq[right], seq[left]
        left += 1
        right -= 1
```
