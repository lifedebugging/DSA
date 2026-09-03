```
def add_binary(a,b):
    c= a+b
    return str(bin(c)[2:])
    #your code here
```

    #here i m using bin() ~ in-built function 
    # but Built-in way (includes '0b' prefix)
    # Clean way (removes the '0b' prefix using string slicing)
or
```
def add_binary(a,b):
    return f"{a + b:b}"v
```
