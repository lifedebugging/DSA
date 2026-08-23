```
def filter_numbers(string):
    return  "".join(x for x in string if x.isalpha())
```
OR
```
def filter_numbers(string):
    return  "".join(filter(str.isalpha, string))
```
"above two solution is wrong below are corrected one"
OR

```
import re

def filter_numbers(string):
    return re.sub(r'\d',"", string)
```
OR
```
def filter_numbers(string):
    return  "".join(x for x in string if x.isalpha() or x.isspace())
```
