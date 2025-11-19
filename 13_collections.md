# Python Collections Cheat Sheet

## 1. Strings (`str`)
- Ordered, immutable text.
```python
name = "Alice"
print(name[0])      # A
print(name[1:3])    # li
```

## 2. Lists (`list`)
- Ordered, mutable, allows duplicates.
```python
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")
print(fruits)
```

## 3. Tuples (`tuple`)
- Ordered, immutable.
```python
point = (10, 20)
print(point[0])
```

## 4. Sets (`set`)
- Unordered, mutable, unique items only.
```python
s = {1, 2, 3, 3}
print(s)   # {1, 2, 3}
```

## 5. Dictionaries (`dict`)
- Key-value pairs, mutable, keys unique.
```python
person = {"name": "Alice", "age": 25}
print(person["name"])
```

## Summary Table

| Type   | Ordered | Mutable | Allows Duplicates | Usage |
|--------|---------|---------|-------------------|-------|
| `str`  | Yes     | No      | Yes               | Text data |
| `list` | Yes     | Yes     | Yes               | General collections |
| `tuple`| Yes     | No      | Yes               | Fixed data |
| `set`  | No      | Yes     | No                | Unique items |
| `dict` | Yes*    | Yes     | Keys: No          | Key-value data |

*Dicts preserve insertion order in Python 3.7+.
