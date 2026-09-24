```py

import codecs 
def rot13(message):
    # if its non letter let it be unchanged
    #if its letter shift to 13
    cipher_txt = codecs.encode(message, 'rot_13')
    return cipher_txt

```
