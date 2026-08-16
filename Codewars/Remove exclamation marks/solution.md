my first solution
```
def remove_exclamation_marks(s):
    return s.replace('!', '')
```
can also be done with 
```
s.translate(str.maketrans("!", ''))
```
better for multi replacement/removal
