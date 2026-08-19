```
def count_min_rotations(dice):
    if not dice:
        return 0
    min_rotations = float('inf')
    
    for target in range(1,7):
        current_rotation = 0
        
        for die in dice:
            if target == die:
                continue
            elif target+die == 7:
                current_rotation+=2
            else:
                current_rotation+=1
        if current_rotation < min_rotations:
            min_rotations = current_rotation
    return min_rotations
```

few things to notice:
```
# Standard "Find Minimum Element" pattern
lowest = float('inf')
```

unfortunately i had to look it up solution in google because i wasn't getting anywhere to get the `min_rotation`

