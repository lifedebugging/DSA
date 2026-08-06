Before writing any code i m answering

What are the variables?
variables 500 litres tank current water, 8% loss every 60 minute + 15 litres water back 

Where is the equals / stopping condition?
"back into" and "lose" and stopping condition when water < 200 litres 

Which category does this belong to?
Accumilator/ Growth category

How would you model it?
 8% of 500 litres = 40 litres
so every 60 minutes (500-40)+15
just guessing since only 25 litres losing every hour which roughly 8 hours 

*which was my mistake* because every hour the current total is getting down as well

code:
```
hours = 0
def tank(litres: int=500):
  while litres >= 200:
     litres = litres - (litres * 0.08) + 15
     hours +=1
  return hours
```
Lesson: percentages change as the total changes.
Whenever you see "X% of current amount," multiply the percentage by the variable inside the loop
