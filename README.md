## 📊 Java Collections – Big O Performance

Below are the **Big O performance** metrics of common functions for different Java Collections.

---

### 📝 **List**

| List                 | Add  | Remove | Get  | Contains | Next | Data Structure |
|-----------------------|------|--------|------|----------|------|----------------|
| `ArrayList`            | O(1) | O(n)  | O(1) | O(n)    | O(1) | Array |
| `LinkedList`           | O(1) | O(1)  | O(n) | O(n)    | O(1) | Linked List |
| `CopyOnWriteArrayList` | O(n) | O(n)  | O(1) | O(n)    | O(1) | Array |

---

### 🔢 **Set**

| Set                    | Add    | Remove | Contains | Next   | Size | Data Structure           |
|-------------------------|--------|--------|----------|--------|------|---------------------------|
| `HashSet`               | O(1)  | O(1)  | O(1)    | O(h/n) | O(1) | Hash Table |
| `LinkedHashSet`         | O(1)  | O(1)  | O(1)    | O(1)   | O(1) | Hash Table + Linked List |
| `EnumSet`               | O(1)  | O(1)  | O(1)    | O(1)   | O(1) | Bit Vector |
| `TreeSet`               | O(log n) | O(log n) | O(log n) | O(log n) | O(1) | Red-black Tree |
| `CopyOnWriteArraySet`   | O(n)  | O(n)  | O(n)    | O(1)   | O(1) | Array |
| `ConcurrentSkipListSet` | O(log n) | O(log n) | O(log n) | O(1)   | O(n) | Skip List |

---

### 🛠️ **Queue**

| Queue                   | Offer   | Peek | Poll   | Remove | Size | Data Structure |
|--------------------------|---------|------|--------|--------|------|----------------|
| `PriorityQueue`           | O(log n) | O(1) | O(log n) | O(n)  | O(1) | Priority Heap |
| `LinkedList`              | O(1)   | O(1) | O(1)   | O(1)  | O(1) | Linked List |
| `ArrayDeque`              | O(1)   | O(1) | O(1)   | O(n)  | O(1) | Array |
| `ConcurrentLinkedQueue`   | O(1)   | O(1) | O(1)   | O(n)  | O(n) | Linked List |
| `ArrayBlockingQueue`      | O(1)   | O(1) | O(1)   | O(n)  | O(1) | Array |
| `PriorityBlockingQueue`   | O(log n) | O(1) | O(log n) | O(n) | O(1) | Priority Heap |
| `SynchronousQueue`        | O(1)   | O(1) | O(1)   | O(n)  | O(1) | None |
| `DelayQueue`              | O(log n) | O(1) | O(log n) | O(n) | O(1) | Priority Heap |
| `LinkedBlockingQueue`     | O(1)   | O(1) | O(1)   | O(n)  | O(1) | Linked List |

---

### 🗂️ **Map**

| Map                     | Get    | ContainsKey | Next   | Data Structure           |
|--------------------------|--------|-------------|--------|---------------------------|
| `HashMap`               | O(1)  | O(1)        | O(h/n) | Hash Table |
| `LinkedHashMap`         | O(1)  | O(1)        | O(1)   | Hash Table + Linked List |
| `IdentityHashMap`       | O(1)  | O(1)        | O(h/n) | Array |
| `WeakHashMap`           | O(1)  | O(1)        | O(h/n) | Hash Table |
| `EnumMap`               | O(1)  | O(1)        | O(1)   | Array |
| `TreeMap`               | O(log n) | O(log n) | O(log n) | Red-black Tree |
| `ConcurrentHashMap`     | O(1)  | O(1)        | O(h/n) | Hash Table |
| `ConcurrentSkipListMap` | O(log n) | O(log n) | O(1)   | Skip List |

---

✅ **Notes:**

- **h:** Hash collisions.
- `O(h/n)`: Depends on the load factor and number of collisions.
- Use **appropriate data structures** based on your performance needs for `Add`, `Remove`, `Get`, and concurrent operations.
