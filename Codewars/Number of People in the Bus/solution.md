Well this one actually scared me I m not gonna lie I thought I will have to look at the solution
You should know that I have no experience in DSA 

So anyways I decided to not give up, I gave it a try

I wrote a pseudo code of my own understanding that's what i do when i m really not understanding what's going on help me clear up

```
# nested list
# iterate over at last [nth index]
# subtract the total number of people get on the bus - total number of people get off the bus
# return list[nth][0]
```

```
def number(bus_stops):
    last_psg = []
    for i in bus_stops:
        sub = i[0] - i[1]
        last_psg.append(sub)
    return last_psg
```
This gave me  subtract the total number of people get on the bus - total number of people get off the bus but a list of it 
that's it then i just sum it all up

```
total = sum(k for k in last_psg)
```
and it worked however i don't know how efficient this is and i definitely think the question could be frame a little better the words are poor.
