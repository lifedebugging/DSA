```
import re
def array(string):
    # first string index count should be more than two use if else?
    # only the last and first one would be cut off in new string, use index slicing?
    #your code here
    items = string.split(",")
    middle_items = items[1:-1]
    return  " ".join(middle_items) if middle_items else None

#Whenever a problem mentions items "separated by commas", always use string.split(",") to turn it into a list of items first, before doing any slicing or removal
```
