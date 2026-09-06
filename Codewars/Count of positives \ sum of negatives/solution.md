```
def count_positives_sum_negatives(arr):
    pos = sum(1 for a in arr if (a> 0))
    neg = sum(a for a in arr if (a<0))
    return [pos,neg] if arr else []
```
