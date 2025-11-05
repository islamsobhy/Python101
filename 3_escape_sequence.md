# 🐍 Python Escape Sequences

Escape sequences are special characters in Python strings that represent spaces, tabs, newlines, or non-printable characters.  
They start with a backslash (`\`).

---

## 📘 Common Escape Sequences

| Escape Sequence | Meaning | Example | Output |
|------------------|----------|----------|---------|
| `\b` | Backspace | `print("Hello\bWorld")` | `HellWorld` |
| `\n` | New line | `print("Hello\nWorld")` | <pre>Hello<br>World</pre> |
| `\t` | Horizontal tab | `print("Hello\tWorld")` | `Hello    World` |
| `\r` | Carriage return | `print("Hello\rWorld")` | `World` |
| `\'` | Single quote | `print('It\'s OK')` | `It's OK` |
| `\"` | Double quote | `print("He said, \"Hi\"")` | `He said, "Hi"` |
| `\\` | Backslash | `print("C:\\Users\\")` | `C:\Users\` |
| `\xhh` | Hex character value | `print("\x48\x69")` | `Hi` |

---

## 💻 Demo Script

You can copy and run this Python script to see all escape sequences in action:

```python
# escape_sequences_demo.py

print("Escape Sequence Demonstration:\n")

print("1. Backspace (\\b):", "Hello\bWorld")
print("2. New line (\\n):", "Hello\nWorld")
print("3. Tab (\\t):", "Hello\tWorld")
print("4. Carriage return (\\r):", "Hello\rWorld")
print("5. Single quote (\\'):", 'It\'s OK')
print('6. Double quote (\\"):', "He said, \"Hi\"")
print("7. Backslash (\\\\):", "C:\\Users\\")
print("8. Hex value (\\xhh):", "\x48\x69")  # H = 48, i = 69 in hex
