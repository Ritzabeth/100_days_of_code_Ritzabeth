## 📅 Day 22 – June 1, 2025

**✅ What I did today:**

- Practiced number conversions in Python: binary, octal, and hexadecimal.
- I-dentified and fixed a common error when trying to slice [2:] from an integer.

**📚 What I learned:**

- The functions bin(), oct(), and hex() return strings with prefixes (0b, 0o, 0x), and to remove those prefixes, you need to apply slicing after converting the number to a string.

```
print(bin(num)[2:]) # Shows binary number without the '0b'
```
- Data types matter: you can’t slice an int, only strings or sequences.
