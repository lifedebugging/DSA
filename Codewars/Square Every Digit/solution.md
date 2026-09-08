first solution 
```
def square_digits(num):
    p = ""
    for n in str(num):
        p += str(int(n) ** 2)
    return int(p)
        
    # Your code here
```
one liner
```
def square_digits(num):
    return int("".join(str(int(n)** 2) for n in str(num)))
```
def square_digits(num):
    if num == 0:
        return 0
    
    result = 0
    place_value = 1 
    
    while num> 0:
        digit = num % 10
        squared = digit ** 2
        
        result += squared * place_value
        
        if squared >= 10:
            place_value *= 100
        else:
            place_value *=10
            
        num //= 10
        
    return result
 ```  
