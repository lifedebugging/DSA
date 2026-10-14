```py
def nb_dig(n, d):
    #obv first step in range n square them all but since integer there is a possibility of being negative but result will be always pos
    #store the occurance in list
    #then check if d is present in each number 
    #since we are checking each number inside a list we need a nested loop
    #or you can convert to string and use .count()
    #and then a simple counter +1 to count all the occurance of d
    
    count = 0
    for k in range(n+1):
        squared = k**2
        
        count += str(squared).count(str(d))
    return count
```
