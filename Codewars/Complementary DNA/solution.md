my first solution:
```
return dna.replace('A', 'T').replace('T','A').replace('G','C').replace('C','G')
```
BUt the problem is when it run A gets replaced by T then T get replaced by A again..

My thinking:

loop one by one over each string and replace it and so i did
however make sure you store *the string in new string* because well it won't work
```
def DNA_strand(dna):
    new_dna = ""
    for d in dna:
        if d == 'T':
            new_dna += d.replace('T', 'A')
        elif d== 'A':
            new_dna += d.replace('A', 'T')
            
        elif d =='C':
            new_dna += d.replace('C','G')
        else:
            new_dna += d.replace('G', "C")
            
    return new_dna
    # code here
```
better way:
```
def DNA_strand(dna):
    return dna.translate(str.maketrans({"A": "T", "T": "A", "G": "C", "C": "G"}))
    # code here
```
