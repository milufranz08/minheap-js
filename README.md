# MinHeap (JS)

While studying and prepping for interviews, I've found JavaScript to be one of the easiest and most flexible languages to use when implementing fast solutions. However, JavaScript does not have all the data structures out of the box as other languages such as Java and Python. This is the case for a min heap or a priority queue.

This repo contains a simple implementation of a min heap in JavaScript using an array as the data structure under the hood.

Resources: [AlgoMonster](https://algo.monster/problems/heap_intro)

## How to use it?

1. **Initialize it**
```
    const heap = new MinHeap();
```

2. **Insert values**
The MinHeap class expects a HeapItem node. The HeapItem expects two values on initialization, item and priority. The latter being optional.
```
    heap.push(new HeapItem(val)
```

> **Note:** If you enter an item that is not a number (i.e. an array of values), make sure to provide a priority value so the heap is able to sort.
```
    heap.push(new HeapItem([val, i, 0], val))
```

3. **Get smallest value**
```
    const item = heap.pop().element
```

4. **Take a look at smallest value**
This option allows you to see the min value but keep it in place.
```
    const item = heap.peek().element
```

5. **Get size**
```
    const n = heap.size()
```