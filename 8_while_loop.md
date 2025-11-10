
# 🐍 Python `while` Loops — Complete Guide + Practice

This document walks you through everything you need to know about **`while` loops in Python**, from syntax to advanced exercises.

---

## 📘 1. What is a `while` Loop?

A **`while` loop** runs a block of code **as long as a condition is `True`**.

### 🧩 Syntax:
```python
while condition:
    # code block
```

### Example:
```python
count = 1
while count <= 5:
    print(count)
    count += 1
```

---

## ⚙️ 2. How It Works

1. Check the **condition** → if True, run the code inside.
2. After running the block, check again.
3. Stop when the condition becomes **False**.

---

## ⚠️ 3. Infinite Loops

If the condition never becomes False, the loop never stops.

```python
i = 1
while i <= 5:
    print(i)
    # forgot i += 1 → infinite loop!
```

---

## 🪄 4. Optional `else` Block

You can attach an `else` block to a `while` loop.
It runs **only if the loop finished normally** (no `break`).

```python
x = 1
while x <= 3:
    print(x)
    x += 1
else:
    print("Loop finished!")
```

---

## 🔄 5. Loop Control: `break` and `continue`

### `break` — stop the loop immediately
```python
i = 1
while i <= 5:
    if i == 3:
        break
    print(i)
    i += 1
```

### `continue` — skip current iteration
```python
i = 0
while i < 5:
    i += 1
    if i == 3:
        continue
    print(i)
```

---

## 💡 6. Practice Exercises

### 🟢 Beginner

#### 1️⃣ Counting from 1 to 10
```python
i = 1
while i <= 10:
    print(i)
    i += 1
```

#### 2️⃣ Counting Down from 10
```python
i = 10
while i >= 1:
    print(i)
    i -= 1
```

#### 3️⃣ Sum of First N Numbers
```python
n = int(input("Enter a number: "))
total = 0
i = 1
while i <= n:
    total += i
    i += 1
print("Sum =", total)
```

---

### 🟡 Intermediate

#### 4️⃣ Even Numbers from 1–20
```python
i = 1
while i <= 20:
    if i % 2 == 0:
        print(i)
    i += 1
```

#### 5️⃣ Guess the Number Game
```python
secret = 7
guess = None

while guess != secret:
    guess = int(input("Guess the number: "))
    if guess < secret:
        print("Too low!")
    elif guess > secret:
        print("Too high!")
    else:
        print("Correct!")
```

#### 6️⃣ Reverse Digits of a Number
```python
num = int(input("Enter a number: "))
rev = 0

while num > 0:
    digit = num % 10
    rev = rev * 10 + digit
    num //= 10

print("Reversed number:", rev)
```

---

### 🔵 Advanced

#### 7️⃣ Check Palindrome Number
```python
num = int(input("Enter a number: "))
temp = num
rev = 0

while num > 0:
    rev = rev * 10 + num % 10
    num //= 10

if temp == rev:
    print("Palindrome")
else:
    print("Not palindrome")
```

#### 8️⃣ Collatz Sequence
```python
n = int(input("Enter a number: "))
while n != 1:
    print(n, end=" → ")
    if n % 2 == 0:
        n //= 2
    else:
        n = 3 * n + 1
print(1)
```

#### 9️⃣ Pattern Printing
```python
rows = 5
i = 1
while i <= rows:
    print("*" * i)
    i += 1
```

#### 🔟 ATM Simulation
```python
balance = 1000

while True:
    print("\n1. Check Balance\n2. Withdraw\n3. Exit")
    choice = input("Choose an option: ")

    if choice == '1':
        print("Balance:", balance)
    elif choice == '2':
        amt = int(input("Enter amount: "))
        if amt <= balance:
            balance -= amt
            print("Withdrawn:", amt)
        else:
            print("Insufficient funds!")
    elif choice == '3':
        print("Goodbye!")
        break
    else:
        print("Invalid option.")
```

---

## 🧠 Summary Table

| Keyword | Purpose |
|----------|----------|
| `while condition:` | Loop as long as condition is True |
| `break` | Stop the loop immediately |
| `continue` | Skip current iteration |
| `else` | Run if loop ends normally |

---

🎯 **Next Step:**  
Try modifying each program — add user input, change conditions, or introduce counters.  
Practicing by tweaking loops builds real logic fluency.
