```
def fake_bin(num_string):
    counter = []
    for x in num_string:
        if int(x) >= 5:
            counter.append(1)
        else:
            counter.append(0)

    return "".join(str(c) for c in counter)

```
the better one:
```
