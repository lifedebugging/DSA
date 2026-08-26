```
def bmi(weight, height):
    print(weight, height)
    index = weight  / (height ** 2)
    print(index)
    return "Underweight" if index <= 18.5 else "Normal" if index <= 25.0 else "Overweight" if index <=30.0 else "Obese"
    #your code here
```
