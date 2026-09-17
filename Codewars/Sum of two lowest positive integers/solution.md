```
def sum_two_smallest_numbers(numbers):
    sorted_sum = sorted(numbers)
    if not sorted_sum and not sorted_sum > 2:
        return "Not enough numbers"
    return sum(sorted_sum[:2])
```
