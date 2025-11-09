# 🐍 Python Operators, Input, Boolean, and Logical Operators

This guide explains **Python operators**, **input handling**, **boolean expressions**, and **logical operators**, all in one place.

---

## 1️⃣ Python Operators Overview

Operators are symbols used to perform operations on variables and values.

### 🔹 Types of Operators in Python

| Type | Description | Example |
|------|--------------|----------|
| Arithmetic Operators | Perform mathematical operations | `+`, `-`, `*`, `/`, `//`, `%`, `**` |
| Assignment Operators | Assign values to variables | `=`, `+=`, `-=`, `*=`, `/=`, `%=` |
| Comparison Operators | Compare two values | `==`, `!=`, `>`, `<`, `>=`, `<=` |
| Logical Operators | Combine conditional statements | `and`, `or`, `not` |
| Identity Operators | Compare memory locations | `is`, `is not` |
| Membership Operators | Test for sequence membership | `in`, `not in` |
| Bitwise Operators | Operate on bits | `&`, `|`, `^`, `~`, `<<`, `>>` |

---

## 2️⃣ Arithmetic Operators

Arithmetic operators are used for mathematical calculations.

```python
a = 10
b = 3

print(a + b)   # Addition
print(a - b)   # Subtraction
print(a * b)   # Multiplication
print(a / b)   # Division
print(a // b)  # Floor Division
print(a % b)   # Modulus
print(a ** b)  # Exponentiation
```

### ▶️ Output
```
13
7
30
3.3333333333333335
3
1
1000
```

---

## 3️⃣ Assignment Operators

Assignment operators are used to assign values to variables.

```python
x = 5
x += 3   # x = x + 3
x -= 2   # x = x - 2
x *= 4   # x = x * 4
x /= 2   # x = x / 2
print(x)
```

### ▶️ Output
```
12.0
```

---

## 4️⃣ Comparison Operators

Comparison operators are used to compare values.

```python
a = 10
b = 5

print(a == b)
print(a != b)
print(a > b)
print(a < b)
print(a >= b)
print(a <= b)
```

### ▶️ Output
```
False
True
True
False
True
False
```

---

## 5️⃣ Taking User Input

You can take input from the user using the `input()` function.  
All inputs are stored as **strings** by default.

```python
name = input("Enter your name: ")
age = input("Enter your age: ")
print("Hello", name, "! You are", age, "years old.")
```

### ▶️ Example Output
```
Enter your name: Alice
Enter your age: 25
Hello Alice ! You are 25 years old.
```

To convert input to another type (e.g., integer or float):

```python
age = int(input("Enter your age: "))
height = float(input("Enter your height: "))
print("Age:", age, "Height:", height)
```

---

## 6️⃣ Boolean Data Type

A **Boolean** represents one of two values: `True` or `False`.

```python
is_active = True
is_logged_in = False

print(is_active)
print(type(is_logged_in))
```

### ▶️ Output
```
True
<class 'bool'>
```

Booleans often appear as the result of comparisons:

```python
x = 10
y = 5

print(x > y)
print(x == y)
```

### ▶️ Output
```
True
False
```

---

## 7️⃣ Logical Operators

Logical operators are used to combine conditional expressions.

| Operator | Description | Example | Result |
|-----------|--------------|----------|---------|
| `and` | Returns True if **both** statements are true | `x > 5 and x < 15` | True |
| `or` | Returns True if **any one** statement is true | `x > 5 or x < 3` | True |
| `not` | Reverses the result | `not(x > 5)` | False |

```python
x = 10

print(x > 5 and x < 15)   # True
print(x > 5 or x < 3)     # True
print(not(x > 5 and x < 15))  # False
```

### ▶️ Output
```
True
True
False
```

---

## 8️⃣ Combining Conditions

You can mix comparison and logical operators in a single expression.

```python
age = 20
country = "USA"

if age >= 18 and country == "USA":
    print("Eligible to vote")
else:
    print("Not eligible")
```

### ▶️ Output
```
Eligible to vote
```

---

## ✅ Summary

| Category | Operators | Example | Description |
|-----------|------------|----------|-------------|
| Arithmetic | `+ - * / // % **` | `a + b` | Math operations |
| Assignment | `= += -= *= /=` | `x += 1` | Update variables |
| Comparison | `== != > < >= <=` | `a > b` | Compare values |
| Logical | `and or not` | `a > 5 and b < 10` | Combine conditions |
| Boolean | `True, False` | `is_active = True` | Binary outcomes |
| Input | `input()` | `name = input("Enter: ")` | Take user input |

---

## 💻 Example Script

Save this file as **`operators_demo.py`**:

```python
# operators_demo.py

# Arithmetic operators
a = 10
b = 3
print(a + b, a - b, a * b, a / b, a // b, a % b, a ** b)

# Assignment
x = 5
x += 3
print("x after addition:", x)

# Comparison
print(a > b, a == b, a != b)

# Boolean and logical operators
is_active = True
is_admin = False
print(is_active and is_admin)
print(is_active or is_admin)
print(not is_admin)

# User input example
name = input("Enter your name: ")
print("Hello", name)
```

### ▶️ Example Output
```
13 7 30 3.3333333333333335 3 1 1000
x after addition: 8
True False True
False
True
True
Enter your name: Alice
Hello Alice
```

---

**End of File — Python Operators, Input, and Logical Operators Guide**
