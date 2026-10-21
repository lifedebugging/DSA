```py
def solution(text, ending):
    # your code here...
    #if two or more last char match the 'ending' its true
    if text[-len(ending):] == ending:
        return True
    return False
```
