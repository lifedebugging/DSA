first solution 
```
def reverse_words(text):
    text = text.split(" ")
    print(text)
    return " ".join(t[::-1] for t in text)
    pass #go for it
```
trying with lambda function also known as anonymous function
```
def reverse_words(text):
    return " ".join(map(lambda x: x[::-1], text.split(" ")))
``` 
