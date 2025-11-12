# ⚙️ Python Error Handling — Beginner Guide

This guide explains how to use **try / except** in Python to handle runtime errors safely and clearly.

---

## 🔹 1. What is Error Handling?

Error handling means writing code that can **detect and respond** to errors, instead of crashing your program.

Python uses `try`, `except`, `else`, and `finally` blocks to handle errors gracefully.

---

## 🔹 2. The Basic `try / except` Structure

```python
try:
    # code that may cause an error
except:
    # code that runs if an error occurs
```

Example:

```python
num = input("Enter a number: ")
try:
    num = int(num)
    print(num * 2)
except:
    print("That's not a number!")
```

**If input = 4 →** prints `8`  
**If input = hello →** prints `"That's not a number!"`

---

## 🔹 3. Handling Specific Error Types

You can catch specific errors like `ValueError`, `ZeroDivisionError`, etc.

```python
try:
    num = int(input("Enter a number: "))
    print(10 / num)
except ValueError:
    print("You must enter a valid number!")
except ZeroDivisionError:
    print("You can't divide by zero!")
```

This way you can handle **different kinds of problems separately**.

---

## 🔹 4. Using `else` and `finally`

- `else:` runs **only if no error** occurs.
- `finally:` runs **no matter what**, even if an error happens.

```python
try:
    num = int(input("Enter a number: "))
except ValueError:
    print("Invalid input.")
else:
    print(f"You entered {num}.")
finally:
    print("Program ended.")
```

Output examples:
```
Enter a number: 5
You entered 5.
Program ended.
```
or
```
Enter a number: hi
Invalid input.
Program ended.
```

---

## 🔹 5. Common Example — Handling Input Errors

```python
num = input("Enter your age: ")
try:
    num = int(num)
    num += 2
    print(num)
except ValueError:
    print("This is not an age")
```

**Input: 20 → Output: 22**  
**Input: hi → Output: This is not an age**

---

## 🔹 6. Repeating Until Valid Input (Loop + Try/Except)

You can use a loop to keep asking the user until valid input is given.

```python
while True:
    s = input("Enter a number: ")
    try:
        n = int(s)
        print(f"Thank you! Your number is {n}.")
        break
    except ValueError:
        print("That's not a number, try again.")
```

✅ Keeps looping until the user enters a valid number.

---

## 🔹 7. Using Conditions Instead of `while True`

```python
valid = False
while not valid:
    s = input("Enter a number: ")
    try:
        n = int(s)
        print(f"Thank you! Your number is {n}.")
        valid = True
    except ValueError:
        print("That's not a number, try again.")
```

Same behavior, but clearer logic — loop runs while `valid` is `False`.

---

## 🔹 8. Custom Break Conditions

```python
while True:
    name = input("Enter your name (or 'quit' to stop): ")
    if name.lower() == "quit":
        break
    print(f"Hello, {name}!")
```

**Stops** when the user types `"quit"`.

---

## 🧩 Practice Challenges

1. Ask for a number and print its square. If invalid, show an error message.  
2. Ask for a number and divide 100 by it. Handle both invalid and zero inputs.  
3. Keep asking for input until user enters `'stop'`.  
4. Combine `try/except` with `if` to validate both **data type** and **value range**.  

---


