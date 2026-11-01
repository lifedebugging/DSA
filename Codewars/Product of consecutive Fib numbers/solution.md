```py
def product_fib(_prod):
    a,b = 0, 1
    while a * b <= _prod:
        if a*b == _prod:
            return [a, b , True]
        a,b = b, a+b
        if a*b > _prod:
            return [a, b, False]
        
#     setup fibonacci chain:
#     starting with number 0 and 1 
#     while true i will use
#     where 0 + 1 then result will be stored in res
#     res will  be added to last number used so total of two  variable i will update 
#     last num and res
#     and every res check if res >= prod
#     if true break
#     and return the last num and res , true if == else false
```
