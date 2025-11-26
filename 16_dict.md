# Python Dictionaries — Complete Guide

This guide explains Python dictionaries with clear examples and real-world patterns.

## 1. What Is a Dictionary?
A dictionary is a key–value data structure.

```python
person = {"name": "Ahmed", "age": 30, "city": "Cairo"}
```

## 2. Access, Add, Update, Delete
```python
person["name"]       # access
person["age"] = 31   # update
person["country"] = "Egypt"  # add
del person["city"]   # delete
```

## 3. dict.get()
```python
person.get("job")            # None
person.get("job", "unknown") # 'unknown'
```

## 4. keys(), values(), items()
```python
person.keys()
person.values()
person.items()
```

## 5. Looping
```python
for k in person:
    print(k, person[k])

for v in person.values():
    print(v)

for k, v in person.items():
    print(k, v)
```

## 6. Sorting a Dictionary
```python
scores = {"Ali": 85, "Sara": 92, "Omar": 78}

sorted(scores.items())  # sort by key
sorted(scores.items(), key=lambda x: x[1])  # sort by value
```

## 7. Frequency Counting (Manual)
```python
a = "oisudhcjpoksdcm,weeocjm"
d = {}

for c in a:
    if c in d:
        d[c] += 1
    else:
        d[c] = 1
```

## 8. Frequency Counting (Using get)
```python
d = {}
for c in a:
    d[c] = d.get(c, 0) + 1
```

## 9. Count Specific Character (e.g., 'k')
```python
k_count = d.get("k", 0)
```
