my first solution:
```
def stringy(size):
    bin = []
    for i in range(size):
        if i % 2 ==0:
            bin.append("1")
        else:
            bin.append("0")
    return "".join(bin)
    # Good Luck!
```
one liner:
```
def stringy(size):

    return "".join("1" if i % 2 == 0 else "0" for i in range(size))
    # Good Luck!
```

OR
string multiplication and slicing
```
def stringy(size):

    return (10 * size)[:size]

"""
"10" * 5 creates "1010101010" (length 10).

[:5] slices it down to the first 5 characters: "10101".
"""

