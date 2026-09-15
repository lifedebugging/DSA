```
def make_negative( number ):
    return number if not number > 0 else -number
```
OR
```
def make_negative(number):
    return (number, -number)[number > 0]
```
