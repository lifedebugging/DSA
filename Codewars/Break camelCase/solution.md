```
import re

def solution(s):
    result = re.sub(r"([A-Z])", r" \1", s)
    return result
```
for one liner just return the re expression directly.
