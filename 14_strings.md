# Deep Dive: Python Strings

## 1. What is a string?
A string (`str`) is an ordered, immutable sequence of characters.

```python
name = "Mohammed"
type(name)
len(name)
```

## 2. Indexing
```python
name[0]
name[-1]
name[-2]
```

## 3. Slicing
```python
name[1:3]
name[1:-1]
name[1:]
name[:4]
```

## 4. Immutability & Concatenation
```python
# name[1] = 'a'  # Error
name2 = name[0] + 'a' + name[2:]
```

## 5. Membership
```python
'o' in name
'o' in name2
```

## 6. Help and dir
```python
dir(str)
help(str.find)
```

## 7. Find
```python
name.find('mm')
```

## 8. Extract domain
```python
x = "From abc.xyz@companyname.com to amrqura@gmail.com "July invoice""

first_pos = x.find('@')
last_pos = x.find(' ', first_pos + 1)
domain = x[first_pos+1:last_pos]
domain
```
