my first solution:
```
def cookie(x):
    if type(x) is bool:
        return "Who ate the last cookie? It was the dog!"
    elif isinstance(x, str):
        return "Who ate the last cookie? It was Zach!"
    elif isinstance(x, (float,int)):
        return "Who ate the last cookie? It was Monica!"
    else:
        return "Who ate the last cookie? It was the dog!"
    pass #Good Luck
```
OR
```
def cookie(x):
    eater = {str : "Zach", int : "Monica", float : "Monica"}.get(type(x), "the dog")
    return f"Who ate the last cookie? It was {eater}!"
```

But we didn't check the **Bool** explicitly?

Works because type(x) check the **exact** class

When x = True, type(x) evaluates to <class 'bool'>.

The dictionary keys are {str, int, float}.

Because bool is not inside that dictionary, .get(type(x)) fails to find <class 'bool'>.

It immediately returns the default fallback: "the dog"
