```py
def alphabet_position(text):
    words = text.lower().split()
    
    return " ".join(str(ord(char)- 96) for word in words for char in word if char.isalpha())

```
