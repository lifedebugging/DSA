first
```
def points(games):
    score = 0
    for g in games:
        x, y = map(int,g.split(':'))
        if x < y:
            score +=0
        elif x == y:
            score +=1
        else:
            score +=3
            
    return score
```
one liner (not recommended)
```
 return sum(3 if x > y else 1 if x==y else 0  for g in games for x,y in [map(int, g.split(':'))])
```
