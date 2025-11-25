# Python Lists — Complete Guide

## 📌 What Is a List?
A **list** in Python is an ordered, mutable collection of items.  
Lists allow:
- Mixed data types
- Indexing
- Slicing
- Updating elements
- Iteration
- Nesting (lists inside lists)

```python
fruits = ["apple", "banana", "cherry"]
numbers = [1, 2, 3, 4]
mixed = ["Ali", 30, True, 3.14]
```

---

## 📌 Creating Lists
```python
empty = []
nums = list(range(5))    # [0, 1, 2, 3, 4]
copy = fruits[:]         # shallow copy
```

---

## 📌 Indexing
Lists are 0‑indexed.

```python
fruits[0]      # "apple"
fruits[1]      # "banana"
fruits[-1]     # "cherry"
```

---

## 📌 Slicing
```python
fruits[0:2]    # ['apple', 'banana']
fruits[1:]     # ['banana', 'cherry']
fruits[:]      # full copy
```

---

## 📌 Mutability
Lists **can change** after creation.

```python
fruits[1] = "blueberry"
fruits.append("date")
fruits.insert(1, "kiwi")
fruits.remove("apple")
last = fruits.pop()       # removes last
```

---

## 📌 Common List Methods

| Method | Description |
|--------|-------------|
| append(x) | Add x to end |
| extend(iter) | Add elements from another list |
| insert(i,x) | Insert at index |
| remove(x) | Remove first matching value |
| pop([i]) | Remove + return item |
| clear() | Empty list |
| sort() | Sort in place |
| reverse() | Reverse order |
| count(x) | Count occurrences |
| index(x) | Find index of x |

Example:
```python
nums = [3,1,4,1,5]
nums.count(1)      # 2
nums.index(4)      # 2
nums.sort()        # [1,1,3,4,5]
```

---

## 📌 List Comprehension
Short, powerful syntax.

```python
squares = [x*x for x in range(10)]
evens = [x for x in range(10) if x % 2 == 0]
matrix = [[1,2],[3,4],[5]]
flat = [n for row in matrix for n in row]  # flatten
```

---

## 📌 Iterating Lists
```python
for item in fruits:
    print(item)

for i, item in enumerate(fruits):
    print(i, item)
```

---

## 📌 Copying Lists
```python
a = [1,2,3]
b = a          # alias (same object)
c = a.copy()   # shallow copy
```

Deep copy:
```python
import copy
deep = copy.deepcopy([[1],[2]])
```

---

## 📌 Useful Patterns
```python
" ".join(["hello", "world"])   # "hello world"
"one,two".split(",")           # ['one','two']
3 in [1,2,3]                   # True
[0] * 5                        # [0,0,0,0,0]
```

---

## 📌 Practice Exercises

### 1️⃣ Sum of 1–10
```python
nums = list(range(1,11))
sum(nums)
```

### 2️⃣ Capitalize names
```python
names = ["alice","bob","charlie"]
cap = [n.title() for n in names]
```

### 3️⃣ Flatten list of lists
```python
nested = [[1,2],[3,4],[5]]
flat = [x for row in nested for x in row]
```

### 4️⃣ Sort fruits from string
```python
s = "apple,banana,orange"
lst = s.split(",")
lst.sort()
```

---

## ✅ Summary
- Lists are **ordered + mutable**
- Support indexing, slicing, updating
- Comprehension is powerful
- Know the difference between **shallow** and **deep** copy
 
