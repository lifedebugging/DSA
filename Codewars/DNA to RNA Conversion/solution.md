```
def dna_to_rna(dna):
    rna=""
    for d in dna:
        res = d.replace("T", "U")
        rna += res
    return rna
```
At first I was stuck I thought how would you replace T and U 
I was going to use if/else but then I looked up the .replace method in string manipulation

Here's one liner as well
```
def dna_to_rna(dna):
      return "".join([d.replace("T", "U") for d in dna])
```

couldn't it do it more clean 
PS you can do it with just `dna.replace('T','U')`
