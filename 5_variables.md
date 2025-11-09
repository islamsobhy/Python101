# 🐍 Python Variables

Variables are used to **store data values** in Python.  
They act as containers that hold information which can be used and changed throughout your program.

Python is **dynamically typed**, meaning you don’t have to declare variable types — they’re determined automatically at runtime.

---

## 1️⃣ Creating and Using Variables

To create a variable, simply assign a value to a name using the `=` operator.

```python
name = "Alice"
age = 25
country = "USA"

print(name)
print(age)
print(country)
```

### ▶️ Output
```
Alice
25
USA
```

> 💡 Variable names must start with a letter or underscore (`_`), and can contain letters, numbers, and underscores.

---

## 2️⃣ Variable Naming Rules

Variable names in Python must follow these rules:

✅ **Valid names**
```python
first_name = "John"
_age = 30
user123 = "Mike"
```

❌ **Invalid names**
```python
2user = "Tom"        # Cannot start with a number
user-name = "Sam"    # Hyphen not allowed
my var = "Bob"       # Spaces not allowed
```

> 🧠 Use **snake_case** naming style for readability (e.g., `user_name`, `student_age`).

---

## 3️⃣ Variable Data Types

Variables can store different data types such as strings, numbers, booleans, lists, etc.

```python
name = "Alice"          # string
age = 25                # integer
height = 5.6            # float
is_student = True       # boolean
fruits = ["apple", "banana", "mango"]  # list
```

### ▶️ Output
```
Alice
25
5.6
True
['apple', 'banana', 'mango']
```

You can use the `type()` function to check the data type of a variable:

```python
print(type(name))
print(type(age))
print(type(height))
print(type(is_student))
print(type(fruits))
```

### ▶️ Output
```
<class 'str'>
<class 'int'>
<class 'float'>
<class 'bool'>
<class 'list'>
```

---

## 4️⃣ Multiple Assignments

You can assign values to multiple variables in one line.

```python
x, y, z = 10, 20, 30
print(x, y, z)
```

### ▶️ Output
```
10 20 30
```

You can also assign the same value to multiple variables:

```python
a = b = c = "Python"
print(a, b, c)
```

### ▶️ Output
```
Python Python Python
```

---

## 5️⃣ Variable Reassignment and Updating

You can change a variable’s value at any time — Python will automatically update its type.

```python
x = 10
print(x)

x = "Now I'm a string!"
print(x)
```

### ▶️ Output
```
10
Now I'm a string!
```

> 💡 This is possible because Python is **dynamically typed**.

---

## 6️⃣ Constants (Convention)

Python does not have true constants, but by convention,  
variables written in **ALL_CAPS** are treated as constants.

```python
PI = 3.14159
APP_NAME = "MyApp"

print(PI)
print(APP_NAME)
```

### ▶️ Output
```
3.14159
MyApp
```

> 🔒 Constants are **not enforced** by Python — they’re just a developer convention.

---

## ✅ Summary

| Concept | Example | Description |
|----------|----------|-------------|
| Variable creation | `x = 10` | Assigns value 10 to `x` |
| Data type | `type(x)` | Returns variable type |
| Multiple assignment | `a, b = 1, 2` | Assigns multiple values |
| Same value | `a = b = "Hi"` | Assigns one value to many |
| Reassignment | `x = "text"` | Changes type dynamically |
| Constant (convention) | `PI = 3.14` | Treated as fixed value |

---

## 💡 Best Practices

✅ Use descriptive variable names  
✅ Follow **snake_case** naming style  
✅ Avoid reusing built-in names (e.g., `list`, `sum`, `str`)  
✅ Use **ALL_CAPS** for constants  

---

## 💻 Example Script

Save this file as **`variables_demo.py`**:

```python
# variables_demo.py

# Basic variables
name = "Alice"
age = 25
height = 5.6
is_student = True

# Display values
print(name, age, height, is_student)

# Check types
print(type(name), type(age), type(height), type(is_student))

# Multiple assignment
x, y, z = 1, 2, 3
print(x, y, z)

# Same value
a = b = c = "Python"
print(a, b, c)

# Constant (convention)
PI = 3.14159
print("Value of PI:", PI)
```

### ▶️ Output
```
Alice 25 5.6 True
<class 'str'> <class 'int'> <class 'float'> <class 'bool'>
1 2 3
Python Python Python
Value of PI: 3.14159
```

---

**End of File — Python Variables Guide**
