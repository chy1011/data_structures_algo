# MaxHeap

![MaxHeap Ref Img](max_heap.png)

### What is a MaxHeap?
- Complete Binary Tree
- Every node <= its parent

# MaxHeap Time Complexity!

![MaxHeap Ref Img](max_heap_speed.png)

### MaxHeap is FAST!
- Insert in O(log n)
- Get max in O(1)
- Remove Max in O(log n)

![MaxHeap Ref Img](max_heap_implement_list.png)

### MaxHeap Operations
- Push (insert)
- Peek (get max)
- Pop (remove max)

### Push
- Add value to the end of array
- Float it up to its proper position

![MaxHeap Ref Img](max_heap_push_example.png)
![MaxHeap Ref Img](max_heaps_compare.png)
![MaxHeap Ref Img](max_heaps_compare_2.png)

### Peek
- Returns the value at heap[1]

![MaxHeap Ref Img](max_heaps_peek.png)

### Pop
- Move max to end of array
- Delete it
- Bubble down the item at index to its proper position
- Return max

![MaxHeap Ref Img](max_heaps_pop.png)

### Python MaxHeap
A MaxHeap always bubbles the highest value to the top, so it can be remove instantly.  
Public functions: push, peek, pop  
Private functions: swap, __floatUp, __bubbleDown, __str.

```
class MaxHeap:
    def __init__(self, items=[]):

```
