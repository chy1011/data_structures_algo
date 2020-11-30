# Python Data Structures
### Lists
- General Purpose
- Most widely used data structures
- Grow and shrink size as needed
- Sequence type
- Sortable
**constructors** -> Creating a new list
```
x = list()
y = ['a', 25, 'dog', 8,43]
tuple1 = (10, 20)
z = list(tuple1)

# List Comprehension
a = [m for m in range(8)]
print(a)
b = [i**2 for i in range(10) if i>4]
print(b)
```
**delete** -> delete a list or an item in a list
```
x = [5, 3, 8, 6]
del(x[1]) # deletes index 1 of x which is 3
print(x)
del(x) # deletes the entire list 
```

**append** -> append an item to a list
```
x = [5, 3, 8, 6]
x.append(7)
print(x)
```

**extend** -> append a sequence to a list
```
x = [5, 3, 8, 6]
y = [12, 13]
x.extend(y)
print(x) # "adds" list y to list x
```

**insert** -> insert an item at a given index
```
x = [5, 3, 8, 6]
x.insert(1, 7)
print(x)
x.insert(1, ['a', 'm']
print(x)
```

**pop** -> pops last item off list and returns item
```
x = [5, 3, 8, 6]
x.pop()
print(x)
print(x.pop())
```

**remove** -> remove first instance of an item
```
x = [5, 3, 8, 6, 3]
x.remove(3)
print(x)
```

**reverse** -> reverse the order of the list. It is an in-place sort, meaning it changes the original list.
```
x = [5, 3, 8, 6]
x.reverse()
print(x)
```

**sort** -> sort the list in place.
Note:
sorted(x) returns a new sorted list without changing the original list x.
x.sort() puts the items of x in sorted order (sorts in place).
```
x = [5, 3, 8, 6]
x.sort()
print(x)
```

**reverse sort** -> sort items descending.
Use reverse=True parameter to the sort function.
```
x = [5, 3, 8, 6]
x.sort(reverse=True)
print(x)
```
