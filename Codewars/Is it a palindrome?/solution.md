```py
def is_palindrome(s):
    #to check for palindrome you have to check if the reverse is equal to the word
    #you can reverse by s[::-1]
    #can it work with simple if check
    #however since its case insensitive convert it all to lower case will help
    s = s.lower()
    if not s == s[::-1]:
        return False
    return True
```
