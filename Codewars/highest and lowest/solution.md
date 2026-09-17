```
def high_and_low(numbers: str):
    numbers = [int(x) for x in numbers.split()]
    return " ".join((str(max(numbers)), str(min(numbers))))
```

