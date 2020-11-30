# Python List Comprehensions
basic format: new_list = [transform sequence [filter] ]
```
import random   # built-in python module
```

**get values within a range**
```
under_10 = [x for x in range(10)]
print('under_10: ' + str(under_10))
```
**get squared values**
```
squares = [x**2 for x in under_10]
print('squares: ' + str(squares))
```
