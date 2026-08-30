my first working solution:
```
def human_years_cat_years_dog_years(human_years):
    cat_years = 0
    dog_years = 0
    if human_years == 1:
        cat_years += 15
        dog_years += 15
    elif human_years == 2:
        cat_years += 24
        dog_years += 24
    else:
        cat_years += 24 + (4 * (human_years - 2))
        dog_years += 24 + (5 * (human_years - 2))
            
    return [human_years, cat_years, dog_years]
    
    # Your code here
```
Its simple I know but that's the point first get to answer simple then do the pythonic way.

```
def human_years_cat_years_dog_years(human_years):
    if human_years == 1:
        return [1,15,15]
    elif human_years == 2:
        return [2,24,24]
    else:
         return [human_years, 
                 24 + (4 * (human_years - 2)),
                 24 + (5 * (human_years - 2))]
            
    return [human_years, cat_years, dog_years]
```
Returning final directly from branches, no state tracking.

```
def human_years_cat_years_dog_years(human_years):
    cat_first_two = 9 * min(human_years, 2) + 6
    cat_years = cat_first_two + 4 * max(0, human_years - 2)
    
    dog_first_two = 9 * min(human_years, 2) + 6
    dog_years = cat_first_two + 5 * max(0, human_years - 2)
    
    return [human_years, cat_years, dog_years]
    # Your code here
```
Pure math using  y = a(x) + b





