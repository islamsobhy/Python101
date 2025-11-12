# 🧩 Python Type Hinting

Type hinting in Python helps specify **the expected data types** for function parameters and return values.  
It improves readability, helps detect errors, and works well with tools like `mypy`, `pylance`, or IDEs.

---

## 🔹 1. What Are Type Hints?

Type hints (also called *type annotations*) show what types a function expects and what it returns.

Example:
```python
def sum(x: int, y: int) -> int:
    return x + y

print(sum(5, 4))
```
**Output:**
```
9
```

Here:
- `x: int` → the variable `x` must be an integer.  
- `y: int` → the variable `y` must be an integer.  
- `-> int` → the function will return an integer.

🧠 Type hints **don’t enforce** types at runtime — they are for static analysis and clarity.

---

## 🔹 2. Type Hints with Docstrings

You can include type hints and docstrings together for best readability.

```python
def sum(x: int, y: int) -> int:
    """
    Add two integers together.

    :param x: The first integer
    :param y: The second integer
    :return: The sum of x and y
    """
    return x + y

print(sum(5, 4))
```
Output:
```
9
```

---

## 🔹 3. Why Use Type Hints?

✅ Improves code readability  
✅ Helps IDEs with autocompletion and debugging  
✅ Allows static type checking (`mypy`, VS Code, etc.)  
✅ Makes code easier to maintain in large projects

Example with type checking using `mypy` in terminal:
```
mypy my_script.py
```

---

## 🔹 4. Basic Type Hint Examples

| Type | Example | Description |
|------|----------|-------------|
| `int` | `x: int` | Integer values |
| `float` | `x: float` | Decimal numbers |
| `str` | `name: str` | Text strings |
| `bool` | `flag: bool` | True or False |
| `list` | `nums: list` | List of any values |
| `dict` | `data: dict` | Dictionary |
| `tuple` | `coords: tuple` | Tuple |
| `Any` | `value: Any` | Any type allowed |

Example:
```python
def greet(name: str, age: int) -> str:
    return f"Hello {name}, you are {age} years old."
```

---

## 🔹 5. Type Hints with `typing` Module

Use the `typing` module for advanced hints.

```python
from typing import List, Dict, Tuple, Optional, Any

def total(values: List[int]) -> int:
    return sum(values)

def get_user() -> Dict[str, Any]:
    return {"name": "Alex", "age": 30}

def find_user(id: int) -> Optional[str]:
    if id == 1:
        return "Alice"
    return None

def coordinates() -> Tuple[int, int]:
    return (10, 20)
```

---

## 🔹 6. Type Hint for Functions Without Return

If your function doesn’t return anything, use `-> None`.

```python
def show_message(msg: str) -> None:
    print(msg)
```

---

## 🔹 7. Combining Type Hints with Default Parameters

```python
def power(base: int, exponent: int = 2) -> int:
    return base ** exponent
```

---

## 🔹 8. Lambda Functions and `Callable`

```python
from typing import Callable

add: Callable[[int, int], int] = lambda x, y: x + y
print(add(3, 4))  # 7
```

---

## 🔹 9. Real Example with Type Hints and Error Handling

```python
from typing import List

def average(scores: List[int]) -> float:
    """
    Calculate the average of a list of numbers.

    :param scores: List of integer scores
    :return: Average score as float
    """
    return sum(scores) / len(scores)

print(average([80, 90, 100]))  # 90.0
```

---

## 🧩 10. Practice Challenges

1. Write a function `multiply(x: int, y: int) -> int` that multiplies two numbers.  
2. Write a function `greet(name: str, age: int) -> str` that returns a greeting.  
3. Write `safe_divide(a: float, b: float) -> Optional[float]` that returns `None` if `b == 0`.  
4. Write `combine_names(first: str, last: str) -> str` that joins two strings.  
5. Write `get_max(values: List[int]) -> int` that returns the largest number in a list.

---

