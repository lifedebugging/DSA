```
def get_middle(s):
    # simply find the strin length
    length = len(s)
    #finding even is easy by ( num % 2 check its result 0)
    #if true return s[floor divide by 2 - 1 :floor divide by 2 + 1]
    #say string length is 4
    # s[4/2 - 1 : 4/2 +1] -> s[1:3]
    # this will give two middle value because for length of 4 integer the indexing is:
    # [0,1,2,3]
    #and when we do s[1:3] it always return 1 and 2 indexing skipping the 3 (thats how it works in index slicing)
    
    return s[length // 2 - 1 : length // 2 + 1] if length % 2 == 0 else s[length // 2]
```
