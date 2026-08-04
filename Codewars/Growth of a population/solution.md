MY pseudo code first

```
 def nb_year(p0, percent, aug, p):
    num = []
     while p0 + percent * 0.2 + aug is not equal to p
num.append( p0 + percent * 0.2 + aug)
stop when num >= p
return leng(num)
```

solution is rather easy
just increment year and add p0 until it matches p
```
def nb_year(p0, percent, aug, p):
    year = 0
    while p0 < p:
        #simply calculate new p0
        p0 += int(p0 * (percent / 100)) + aug
        year +=1
    return year
    # your code
```
