```py
def pipe_fix(nums):
    #I have to return a list with ascending number
    #the number starting and end point will be nums starting and end point
    #and it will only count by 1
    start, end = nums[0], nums[-1]
    counter = []
    for i in range(start,end+1):
        counter.append(i)
    return counter
```
OR
```py
def pipe_fix(nums):
	return list(range(nums[0], nums[-1] + 1))
```
