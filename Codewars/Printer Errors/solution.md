```py
def printer_error(color):
    error = sum(1 for c in color if c > 'm')
    return f"{error}/{len(color)}"
```
