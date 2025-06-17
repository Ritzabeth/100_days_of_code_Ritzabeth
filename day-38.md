## 📅 Day 38 – June 17, 2025

**✅ What I learned today:**

- How tiny mistakes in syntax or string formatting can break the output — even if the logic is correct.

- Fixed a bug in a script that checks whether a number is prime. The issue was with how the color formatting and string display were written.

**💻 Before (buggy version):**

```
num = int(input("Ingresa un numero:"))
tot = 0
for i in range(1, num + 1):
    if num % i == 0:
        print(f"\033[33m{i}", end="")   # missing spacing, unclear output
        tot += 1
    else:
        print(f"\033[31m'{i}", end="")  # typo: extra quote mark inside string
```

**🔧 Problems noticed:**

- The output had an unwanted ' character.
- Numbers were hard to read because they had no spaces.
- Final message was glued to the loop output (no line break).

**✅ After (cleaned version):**

```
num = int(input("Ingresa un numero:"))
tot = 0
for i in range(1, num + 1):
    if num % i == 0:
        print(f"\033[33m{i}", end=" ")
        tot += 1
    else:
        print(f"\033[31m{i}", end=" ")

print(f"\n\033[mEl numero {num} fue divisible {tot} veces")
if tot == 2:
    print("Por eso es primo")
else:
    print("Por eso no es primo")
```
**🧠 What this taught me:**

- Spacing and formatting affect how readable the program is.
- A single typo (like a stray quote) can cause confusing output.
- print(..., end=" ") makes your output cleaner when printing in a loop.
- Color codes (\033[31m) don’t fix logic; they’re just for style — and should be reset when needed.
