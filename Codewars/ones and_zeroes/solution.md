# Try 1

At first my solution was 
with an approach of using enumerate to get the index
and apply exponent on it and further multiplying it with val for 1s and 0s
```
def binary_array_to_number(arr):
    num = 0
    for i, val in enumerate((arr)):
            num = sum((2**i)*val)
    return num        

```
But then I got  *int* obj is not iterable error which i should've saw coming from miles 
however upon reading carefully there's one more error that Iterating is from Left to Right

# Try 2
```
def binary_array_to_number(arr):
    num = 0
    for i, val in enumerate(reversed(arr)):
            num = sum((2**i)*val)
            
    return num
```
Upon searching on internet I find out about `reversed()`

But the first error still stands

I thought of using list then i have to convert it to `str` and use `.join` method which is well sounded like i m complicating it.

so i did it one liner

# Try 3
```
def binary_array_to_number(arr):         
    return sum((2**i)*val for i, val in enumerate(reversed(arr)))
```
# Bonus solution
So I was talking about .join method and i found the exact same solution in GeekforGeeks 

a = [1, 0, 1, 1]

n = int(''.join(map(str, a)), 2)
print(n)

and i felt like i didn't do good
