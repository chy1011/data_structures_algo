# Python Data Structures
### Lists
- General Purpose
- Most widely used data structures
- Grow and shrink size as needed
- Sequence type
- Sortable
<em>constructors</em> -> Creating a new list
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
<em>delete</em> -> delete a list or an item in a list
```
x = [5, 3, 8, 6]
del(x[1]) # deletes index 1 of x which is 3
print(x)
del(x) # deletes the entire list 
```

<em>append</em> -> append an item to a list
```
x = [5, 3, 8, 6]
x.append(7)
print(x)
```

<em>extend</em> -> append a sequence to a list
```
x = [5, 3, 8, 6]
y = [12, 13]
x.extend(y)
print(x) # "adds" list y to list x
```

<em>insert</em> -> insert an item at a given index
```
x = [5, 3, 8, 6]
x.insert(1, 7)
print(x)
x.insert(1, ['a', 'm']
print(x)
```
