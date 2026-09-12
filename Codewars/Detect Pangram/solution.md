```
def is_pangram(string):
    alp = 'abcdefghijklmnopqrstuvwxyz'
    string = string.lower()
    for letter in alp:
        if letter not in string:
            return False
    return True
```
Above is a hardcoded version just hard code the alphabets and check against them one by one over the `for` loop.

Upon searching you can `import string` to import `string.ascii_lowercase`
it contains all the 26 letters and use `set` to it.

```
import string

def is_pangram(text):
    text = text.lower()
    return all(letter in text for letter in string.ascii_lowercase)
```
OR
```
import string

def is_pangram(text):
    text = set(text.lower())
    ascii_ = set(string.ascii_lowercase)
    
    return ascii_.issubset(text)
```
