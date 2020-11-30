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

### Tuples
- Immutable (can't add/change)
- Useful fixed data
- Faster than Lists
- Sequence type

**constructors** -> creating new tuples.
```
x = ()
x = (1, 2, 3)
x = 1, 2, 3
x = 2, # comma tells Python its a tuple.
print(x, type(x))

list1 = [2, 4, 6]
x = tuple(list1)
print(x, type(x))
```

**tuples are immutable**, but member objects may be mutable.
```
x = (1, 2, 3)
# del(x[1]) # fails
# x[1] = 8  # fails
print(x)

y = ([1, 2], 3)   # a tubple where the first item is a list
del(y[0][1])      # deletes the 2
print(y)          # the list within the tuple is mutable

y += (4, )        # concatenating two tuples works
print(y)
```

### Sets
- Store non-duplicate items
- Very fast access vs Lists
- Math Set ops (union, intersect)
- Sets are unordered

**constructors** -> creating new sets
```
x = {3, 5, 3, 5}
print(x)

y = set()
print(y)

list1 = [2, 3, 4]
z = set(list1)
print(z)
```
**set operations**
```
x = {3, 8, 5}
print(x)
x.add(7)
print(x)

x.remove(3)
print(x)

# get length of set x
print(len(x))

# check membership in x
print(5 in x)

# pop random item from set x
print(x.pop(), x)

# delete all items from set x
x.clear()
print(x)
```

**Mathematical set operations**  
intersection (AND): set1 & set2  
union (OR): set1 | set2  
symmetric difference (XOR): set1 ^ set2 differencee (in set1 but not set 2): set1 - set2  
subset (set2 contains set1): set1 <= set2  
superset (set1 contains set2): set1 >= set2
```
s1 = {1, 2, 3}
s2 = {3, 4, 5}
print(s1 & s2}
print(s1 | s2)
print(s1 ^ s2)
print(s1 - s2)
print(s1 <= s2)
print(s1 >= s2)
```
**Dictionaries (dict)**
- Key/Value pairs
- Associative array, like Java HashMap
- Dicts are Unordered
```
x = {
     'pork': 25.3,
     'beef': 33.8,
     'chicken': 22.7
    }
print(x)
x = dict([
          ('pork', 25.3),
          ('beef', 33.8),
          ('chicken': 22.7)
        ])
print(x)
x = dict(pork=25.3, beef=33.8, chicken=22.7)
print(x)
```

**dict operations**
```
x['shrimp'] = 38.2    # add or update
print(x)

# delete an item
del(x['shrimp'])
print(x)

# get length of dict x
print(len(x))

# delete all items from dict x
x.clear()
print(x)

# delete dict x
del(x)
```

**accessing keys and values in a dict**  
Not compatible withj Python 2.
```
y = {'pork': 25.3, 'beef': 33.8, 'chicken': 22.7}
print(y.keys())
print(y.values())
print(y.items())    # key-value pairs

# check membership in y_keys (only looks in keys, not values)
print('beef' in y)

# check membership in y_values
print('clams' in y.values())
```

**iterating a dict** -> note, items are in random order.
```
for key in y:
  print(key, y[key])

for k, v in y.items():
  print(k, v)
```
