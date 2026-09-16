```py

def validate_pin(pin):
    return pin.isdigit() and len(pin) in (4,6)
    # return true or false
```
OR
```py
import re

def validate_pin(pin):
    # ^ = start, $ = end, | = OR inside parentheses
    pattern = r"^([0-9]{4}|[0-9]{6})$"
    return bool(re.fullmatch(pattern, pin))
```
