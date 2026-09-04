my first working solution:
```
from collections import Counter

def duplicate_encode(word):
    word = word.lower()

    if len(set(word)) == len(word):
        return len(word) * '('
    
    else:
        char_counts = Counter(word)
        
        result = []
        for char in word:
            if char_counts[char] > 1:
                result.append(")")
            else:
                result.append("(")
        
        return "".join(result)

```
