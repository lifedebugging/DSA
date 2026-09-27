```py
import unicodedata

def switch_it_up(number):
    for n in str(number):
        n_name = unicodedata.name(str(n)).replace('DIGIT ', '').lower().capitalize()
        return n_name
    
        #using unicodedata.name
        #since it return "DIGIT ONE", using .replace('DIGIT ') to swap with empty string.
        #lowercase the string then capitalize
```
