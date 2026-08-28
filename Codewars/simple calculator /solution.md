my first easy solution:
```
def calculator(x, y, op):
    if isinstance(x, int) and isinstance(y,int):
        if op == "+":
            return x + y
        elif op == "-":
            return x - y
        elif op == "*":
            return x * y
        elif op == "/":
            return x / y
        else:
            return "unknown value"
    else:
        return "unknown value"
    
    pass
```

second solutoin
```
def calculator(x, y, op):
# de morgan's law
    if not isinstance(x, int) or not isinstance(y,int):
        return "unknown value"
    match op:
        case "+":
            return x + y
        case "-":
            return x - y
        case "*":
            return x * y
        case "/":
            return x / y
        case _:  # Underscore '_' acts as the catch-all / default case
            return "unknown value"
```
