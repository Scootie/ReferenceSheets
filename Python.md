Multidimensional array

```
class Vividict(dict):
    def __missing__(self, key):
        value = self[key] = type(self)()
        return value
```
For loops:
```
for k in dict: ... (implements tp_iter --> faster option than)
for k in dict.keys(): ...

for key in dict.iterkeys(): ...
for value in dict.itervalues(): ...
for key, value in dict.iteritems(): ...
```
