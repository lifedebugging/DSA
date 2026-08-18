```
def filter_numbers(string):
    return  "".join(x for x in string if x.isalpha())
```
OR
```
def filter_numbers(string):
    return  "".join(filter(str.isalpha, string))
```
