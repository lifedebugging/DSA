```
def xo(s):
    return True if s.lower().count("x") == s.lower().count("o") or "x" and "o" not in s else False
```

I don't know something weird happened at first attempt 1 test case fialed
second 2 test case failed
third attempt all passed

upon searching I believe its the operator preceeding

`s.lower().count("x") == s.lower().count("o") is already Enough`

when no 'x' and no 'o' are in the string (like "zpzpzpp"):

    s.lower().count("x") gives 0

    s.lower().count("o") gives 0

    0 == 0 evaluates to True!

Because 0 == 0 is already True, you don't need any special check for missing letters. 
The equality test naturally handles strings with no 'x' or 'o'
so i changed my solution to

```
def xo(s):
    s = s.lower()
    return s.count("x") == s.count("o")
```

Rule I forgot: Expressions with == return `booleans` directly




