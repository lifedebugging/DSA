```py
# write the function is_anagram
def is_anagram(test, original):
    #True if test chars are all in original
    #can i use all here?
    original, test = original.lower(), test.lower()
    return sorted(original) == sorted(test)
```
