```py
def duplicate_count(text):
    # Your code goes here
    #in this question we have to count the duplicate occurance of characters
    #it can be both lower and upper case bB is still one b duplicate
    #normalize all to lower case
    #can i use .count() here with ascii and set but nope
    #convert it to set
    #and simply loop over each character and use .count but since i have to count exactly one per char
    #i can use simple counter +1
    normalized = text.lower()
    unique = set(normalized)
    count = 0
    for char in unique:
        if normalized.count(char) > 1:
            count +=1
    return count
```
