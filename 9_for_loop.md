# 🐍 Python For Loops — Beginner to Intermediate Guide

This guide explains how to use **for loops** in Python step-by-step, with examples and challenges.

---

## 🔹 1. Basic `for` Loop
A `for` loop repeats actions for each item in a sequence (like a list or string).

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```
**Output:**
```
apple
banana
cherry
```

---

## 🔹 2. Using `range()`
`range()` lets you loop through a sequence of numbers.

```python
for i in range(5):
    print(i)
```
**Output:**
```
0
1
2
3
4
```

Custom start and step:
```python
for i in range(2, 10, 2):
    print(i)
```
**Output:**
```
2
4
6
8
```

---

## 🔹 3. Looping with `enumerate()`
`enumerate()` gives both the **index** and **value** of each item.

```python
fruits = ["apple", "banana", "cherry"]
for index, fruit in enumerate(fruits, start=1):
    print(index, fruit)
```
**Output:**
```
1 apple
2 banana
3 cherry
```

---

## 🔹 4. Using `if` Conditions Inside Loops
You can add logic inside loops to filter values.

```python
temperatures = [12, 18, 25, 30, 22]
for t in temperatures:
    if t > 20:
        print(t)
```
**Output:**
```
25
30
22
```

---

## 🔹 5. Accumulation (Summing Values)
Use a variable to accumulate totals.

```python
numbers = [3, 5, 7, 9]
total = 0
for n in numbers:
    total += n
print("The total is", total)
```
**Output:**
```
The total is 24
```

---

## 🔹 6. Conditional Summation
```python
numbers = [4, 11, 7, 20, 3, 18]
total = 0
for n in numbers:
    if n > 10:
        total += n
print("The sum of numbers greater than 10 is", total)
```
**Output:**
```
The sum of numbers greater than 10 is 49
```

---

## 🔹 7. Combining `enumerate()` and Conditions
```python
ages = [12, 25, 17, 30, 19, 42]
for pos, age in enumerate(ages, start=1):
    if age >= 18:
        print(pos, age)
```
**Output:**
```
2 25
4 30
5 19
6 42
```

---

## 🔹 8. Average of Filtered Values
```python
ages = [12, 25, 17, 30, 19, 42]
total = 0
count = 0

for age in ages:
    if age >= 18:
        total += age
        count += 1

print("Average of adults is", total / count)
```
**Output:**
```
Average of adults is 29.0
```

---

## 🧩 Practice Challenges

1. Print all even numbers between 1 and 20.  
2. Print each word in a sentence on a new line.  
3. Given a list of prices, print only those above 100.  
4. Calculate the product of all numbers in a list.  
5. Print all students with scores above 75 using `enumerate()`.

---


