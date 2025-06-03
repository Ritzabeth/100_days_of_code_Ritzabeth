## 📅 Day 23 – June 2, 2025

**✅ What I did:**

- Reviewed and corrected a triangle classification script I wrote earlier.
- Compared my version to a cleaner and more concise version from the instructor.
- Fixed syntax errors like incorrect quotes, wrong conditionals, and inconsistent logic.

**🧠 What I learned:**

- How to properly use comparison operators like == and !=.
- That if r1 == r2 == r3: is a valid and clean way to check for an equilateral triangle.
- The importance of input validation and clear conditional structure.

**💻 Final Code:**
```
r1 = float(input("Primer segmento: "))
r2 = float(input("Segundo segmento: "))
r3 = float(input("Tercer segmento: "))

if r1 < r2 + r3 and r2 < r1 + r3 and r3 < r1 + r2:
    print("Los segmentos pueden formar un triángulo", end=' - ')
    if r1 == r2 == r3:
        print("EQUILÁTERO!")
    elif r1 != r2 and r2 != r3 and r3 != r1:
        print("ESCALENO!")
    else:
        print("ISÓSCELES!")
else:
    print("Los segmentos NO pueden formar un triángulo.")
```
**📌 Reflection:**

Today was a light day, but even small corrections taught me a lot.
