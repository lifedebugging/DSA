my first solution:

```
def correct(s):
    return s.replace('5','S').replace('0', 'O').replace('1', 'I')
```

but upon finding out about trans built in function:

```
def correct(s):
    return s.translate(str.maketrans("501", "SOI"))
```
or attempt dict look up
```
"".join({'5':'S', '0':'O', '1':'I'}.get(c, c) for c in s)
```
