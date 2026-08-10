The problem is rather simple my first attempt was

My first attempt was using enumerate

`return [item for index, item in enumerate(my_list) if index % 2 != 0]`

But I got an error about `syntax expression` most likely wrong placement of `if` statement

But the solution is even simpler using [start:stop:step] in range or array slicing.

`del my_list[1::2]`


