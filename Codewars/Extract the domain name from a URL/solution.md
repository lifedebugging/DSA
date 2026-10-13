```py
import re
def domain_name(url):
    domain = re.findall(r"((?:https?://)?(?:www\.)?([\w-]+))", url)[0][1]
    return domain
```
