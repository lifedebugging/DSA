my first working solution ~ split, sort and join together
```
import re

def order(sentence):
    sentence = sentence.split()
    print(sentence)
    return " ".join(sorted(sentence, key=lambda x: re.search(r'\d+', x).group()))
```
Also:
```
def order(sentence):
  return " ".join(sorted(sentence.split(), key=min))
```
