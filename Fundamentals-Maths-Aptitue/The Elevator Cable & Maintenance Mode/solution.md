What are your variables?
3* of 100% cable health at every floor +, start at 0 - 20 = + 4, 20 => +2 floors, floor is my variable and cable_health, and trip 

What is your compound stopping condition ?
stopping condition floor >= 35 OR cable_health < 60%

code:
```
def lift():
    floor = 0
    cable_health = 100.0  # (floating value since we starting at 100%)
    trip = 0
    
    while floor < 35 and cable_health >= 60:
        if floor < 20:
            floor += 4
        else:
            floor += 2
            
        trip += 1
        cable_health -= cable_health * 0.03
        
    return trip, floor, cable_health
```
Result: It takes 13 trips to pass Floor 35 and cable health is at 67.7%, so floor limit was reached first
