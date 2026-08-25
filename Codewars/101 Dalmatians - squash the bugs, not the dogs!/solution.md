correct code:
```
def how_many_dalmatians(number):
    dogs =  ["Hardly any", "More than a handful!", "Woah that's a lot of dogs!", "101 DALMATIANS!!!"]
    
    respond = dogs[0] if number <= 10 else dogs[1] if number <= 50 else dogs[2] if number <= 100 else dogs[3] 
    
    return respond
```
However this question and its test case has a bug 

101 DALMATIANS is the correct spelling but in test case it's *DALMATIONS* since i cannot access author test case
I leave it to DALMATIONS in my code.


the code with errors:
```
def how_many_dalmatians(n):
  dogs ["Hardly any", "More than a handful!", "Woah that's a lot of dogs!", "101 DALMATIONS!!!"];
  
  respond = if number <= 10 then dogs[0] else if (number <= 50 then dogs[1] else (number = 101  dogs[3] else dogs[2]
  
return respond
```
