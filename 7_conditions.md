# 🐍 Python Conditional Statements — if, elif, else & Logical Combinations

Conditional statements in Python allow your program to make decisions based on certain conditions.  
They use **if**, **elif**, and **else** blocks to control the flow of execution.

---

## 1️⃣ Basic `if` Statement

The `if` statement executes a block of code **only if** the condition is `True`.

```python
age = 20

if age >= 18:
    print("You are an adult.")
```

### ▶️ Output
```
You are an adult.
```

---

## 2️⃣ The `if...else` Statement

Use `else` to define an alternative block of code that runs when the condition is `False`.

```python
age = 15

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
```

### ▶️ Output
```
You are a minor.
```

---

## 3️⃣ The `if...elif...else` Ladder

Use `elif` (short for *else if*) to check multiple conditions in sequence.

```python
marks = 85

if marks >= 90:
    print("Grade: A")
elif marks >= 75:
    print("Grade: B")
elif marks >= 60:
    print("Grade: C")
else:
    print("Grade: F")
```

### ▶️ Output
```
Grade: B
```

> 💡 Python executes only the first matching condition and skips the rest.

---

## 4️⃣ Nested `if` Statements

You can place one `if` statement inside another to check multiple levels of conditions.

```python
age = 25
citizen = True

if age >= 18:
    if citizen:
        print("Eligible to vote.")
    else:
        print("Not a citizen.")
else:
    print("Underage.")
```

### ▶️ Output
```
Eligible to vote.
```

> 🧠 **Tip:** Try to avoid deep nesting by combining conditions with logical operators (`and`, `or`).

---

## 5️⃣ Combining `if` with Logical Operators

You can combine multiple conditions in a single `if` statement using `and`, `or`, and `not`.

### Using `and`

```python
age = 22
citizen = True

if age >= 18 and citizen:
    print("Eligible to vote.")
else:
    print("Not eligible.")
```

### ▶️ Output
```
Eligible to vote.
```

### Using `or`

```python
has_pass = True
has_permission = False

if has_pass or has_permission:
    print("Access granted.")
else:
    print("Access denied.")
```

### ▶️ Output
```
Access granted.
```

### Using `not`

```python
is_banned = False

if not is_banned:
    print("Welcome!")
else:
    print("Access denied.")
```

### ▶️ Output
```
Welcome!
```

---

## 6️⃣ Combining `if`, `elif`, `else` with Logical Operators

You can use logical operators inside complex decision-making structures.

```python
marks = 72
attendance = 85

if marks >= 90 and attendance >= 90:
    print("Excellent performance!")
elif marks >= 70 and attendance >= 75:
    print("Good performance!")
elif marks >= 50 and attendance >= 60:
    print("Needs improvement.")
else:
    print("Failed.")
```

### ▶️ Output
```
Good performance!
```

---

## 7️⃣ Short-Hand `if` and `if...else`

Python allows short-hand versions of simple conditions.

### One-line `if`

```python
x = 10
if x > 5: print("x is greater than 5")
```

### ▶️ Output
```
x is greater than 5
```

### One-line `if...else`

```python
age = 18
print("Adult") if age >= 18 else print("Minor")
```

### ▶️ Output
```
Adult
```

---

## 8️⃣ Conditional Expressions in Real Use

You can combine user input, arithmetic, and logical operators inside conditions.

```python
age = int(input("Enter your age: "))
country = input("Enter your country: ")

if age >= 18 and country.lower() == "usa":
    print("Eligible to vote in the USA.")
else:
    print("Not eligible to vote in the USA.")
```

### ▶️ Example Output
```
Enter your age: 20
Enter your country: USA
Eligible to vote in the USA.
```

---

## ✅ Summary

| Statement | Syntax Example | Description |
|------------|----------------|-------------|
| `if` | `if condition:` | Executes a block if condition is True |
| `if...else` | `if cond: ... else: ...` | Adds an alternative path |
| `if...elif...else` | Multiple conditions | Tests several cases in order |
| `and` | `if a > 5 and b < 10:` | Both conditions must be True |
| `or` | `if a > 5 or b < 10:` | At least one condition True |
| `not` | `if not banned:` | Reverses the condition |

---

## 💻 Example Script

Save this as **`if_else_demo.py`**:

```python
# if_else_demo.py

age = 20
citizen = True

if age >= 18 and citizen:
    print("Eligible to vote.")
elif age >= 16:
    print("Almost eligible.")
else:
    print("Not eligible.")

marks = 85
attendance = 90

if marks >= 90 and attendance >= 90:
    print("Excellent!")
elif marks >= 70 and attendance >= 75:
    print("Good performance.")
else:
    print("Needs improvement.")
```

### ▶️ Output
```
Eligible to vote.
Good performance.
```

---

**End of File — Python If, Else, Elif & Logical Operators Guide**
