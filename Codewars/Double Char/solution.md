```
def double_char(s):
    return "".join(i*2 for i in s)
```
OR do with zip
pain the string with itself

` return "".join(a + b for a,b in zip(s,s))`
