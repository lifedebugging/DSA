# To count distinct letters or objects use `Counter`

```
from collections import Counter

def count(s):
    if not s:
        return {}
    return Counter(s)
```
