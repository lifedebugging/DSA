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
the better one with `join`:
```
def fake_bin(num_string):
    return "".join("1" if (x >= "5") else "0" for x in num_string)
```
