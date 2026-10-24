```py
def how_much_i_love_you(nb_petals):
    #first i need a list of all the letters
    #and use modulo operator
    petals = ["I love you",
              "a little",
              "a lot",
              "passionately",
              "madly",
              "not at all"]
    
    len_of_petals = len(petals)
    return petals[(nb_petals - 1) % len_of_petals]
```
