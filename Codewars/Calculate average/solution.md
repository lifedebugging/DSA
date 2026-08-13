```
def find_average(numbers):
    return sum(numbers)/ len(numbers) if len(numbers) > 0 else 0
    pass
```
ORRRR
```
import statistics
return statistics.mean(numbers) if len(numbers) > 0 else 0
```
