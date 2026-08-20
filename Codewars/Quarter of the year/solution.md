```
def quarter_of(month):
    # your code here
    # less than 3 or 3 part of 1st quarter
    # 3-6 second quarter
    #6-9 third quarter
    #9-12 fourth quarter
    #so if 3 >= month
    if 3 >= month:
        return 1
    elif 6>= month:
        return 2
    elif 9 >= month:
        return 3
    else: 
        return 4
```
simplest solution

one line below:
```
def quarter_of(month):
    # your code here
    return (month -1) //3 +1
```

