# 🐍 Python Functions — Built-in, Module, and User-Defined Functions

This guide covers **Python functions**: built-in functions (like `print`, `max`, `min`), module functions (like `math.sqrt`), and user-defined functions.

---

## 🔹 1. What is a Function?

A **function** is a reusable block of code that performs a specific task.  
It can take **inputs** (parameters) and may return an **output** (value).

Syntax:
```python
def function_name(parameters):
    # Code block
    return value  # optional
```

Example:
```python
def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))
```
Output:
```
Hello, Alice!
```

---

## 🔹 2. Built-in Functions

Python comes with many built-in functions you can use without importing any modules.

```python
print("Hello")          # prints a message
len([1, 2, 3])          # returns 3
max([4, 10, 2])         # returns 10
min([4, 10, 2])         # returns 2
sum([1, 2, 3, 4])       # returns 10
type("Hi")              # returns <class 'str'>
round(3.14159, 2)       # returns 3.14
abs(-5)                 # returns 5
```

---

## 🔹 3. Functions in Modules

Python modules (like `math`, `random`, `datetime`) contain extra functions you can import.

### Example with `math`:
```python
import math

print(math.sqrt(16))   # 4.0
print(math.pow(2, 3))  # 8.0
print(math.pi)         # 3.141592653589793
```

Or import a single function:
```python
from math import sqrt
print(sqrt(25))  # 5.0
```

### Example with `random`:
```python
import random
print(random.randint(1, 6))  # random number between 1 and 6
```

### Example with `datetime`:
```python
import datetime
print(datetime.datetime.now())  # prints current date and time
```

---

## 🔹 4. Defining Your Own Function

Example:
```python
def add_numbers(a, b):
    return a + b

result = add_numbers(5, 7)
print("Sum:", result)
```
Output:
```
Sum: 12
```

---

## 🔹 5. Default Parameters

You can give parameters default values.

```python
def greet(name="Guest"):
    print(f"Hello, {name}!")

greet()        # Hello, Guest!
greet("Bob")   # Hello, Bob!
```

---

## 🔹 6. Returning Multiple Values

Functions can return multiple results as a tuple.

```python
def divide(a, b):
    quotient = a // b
    remainder = a % b
    return quotient, remainder

q, r = divide(10, 3)
print(q, r)  # 3 1
```

---

## 🔹 7. Variable Arguments

Use `*args` for multiple positional arguments, and `**kwargs` for keyword arguments.

```python
def total_sum(*nums):
    return sum(nums)

print(total_sum(1, 2, 3, 4))  # 10

def show_info(**info):
    for key, value in info.items():
        print(key, "=", value)

show_info(name="Alex", age=25)
```
Output:
```
name = Alex
age = 25
```

---

## 🔹 8. Lambda (Anonymous) Functions

Short, one-line functions created using `lambda`.

```python
square = lambda x: x ** 2
print(square(5))  # 25
```

Commonly used with `map()` or `filter()`:
```python
nums = [1, 2, 3, 4]
squares = list(map(lambda x: x**2, nums))
print(squares)  # [1, 4, 9, 16]
```

---

## 🔹 9. Methods vs Functions

- **Function** — standalone (e.g., `len(list)` or `math.sqrt(9)`)
- **Method** — tied to an object (e.g., `"text".upper()`)

Example:
```python
"hello".upper()   # "HELLO"
[1, 2, 3].append(4)
```

---

## 🔹 10. Error Handling Inside Functions

```python
def safe_divide(a, b):
    try:
        return a / b
    except ZeroDivisionError:
        return "Cannot divide by zero"

print(safe_divide(10, 0))  # Cannot divide by zero
```

---

## 🔹 11. Docstrings and `help()`

Document your functions properly using docstrings.

```python
def multiply(a, b):
    """Return the product of two numbers."""
    return a * b

help(multiply)
```

---

## 🧩 Practice Challenges

1. Write a function `is_even(n)` that returns True if n is even.  
2. Write `find_max(a, b, c)` using `if` statements (no `max()`).  
3. Create a function `square_root(x)` that uses `math.sqrt` and handles negative input gracefully.  
4. Write a function `reverse_string(s)` that returns the reversed string.  
5. Use `map()` with a lambda to cube all numbers in a list.  

---

💾 Created by ChatGPT — Python Functions Guide
