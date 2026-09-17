```py
import string

def high(x):
    # Code here
    # associate each letter with number
    matches = {
        "a": 1,
        "b": 2,
        "c": 3,
        "d": 4,
        "e": 5,
        "f": 6,
        "g": 7,
        "h": 8,
        "i": 9,
        "j": 10,
        "k": 11,
        "l": 12,
        "m": 13,
        "n": 14,
        "o": 15,
        "p": 16,
        "q": 17,
        "r": 18,
        "s": 19,
        "t": 20,
        "u": 21,
        "v": 22,
        "w": 23,
        "x": 24,
        "y": 25,
        "z": 26
       }
    x = x.split()
    
    return max(x, key=lambda word: sum(matches[char] for char in word))
```

OR
```py
import string

def high(x):
    
    # Code here
    words = x.split()
    return max(words, key = lambda word : sum(ord(char) - 96 for char in word))
```
