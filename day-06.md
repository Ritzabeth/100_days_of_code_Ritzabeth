## 📅 Day 6 – May 16, 2025

**✅ What I did:**
- Learned how to use modules in Python.  
- Practiced using `import` and `from ... import` to access specific functions.  
- Explored both built-in modules and external modules via PyPI.  

**📚 What I learned:**
- How to import specific functions from a module: `from math import hypot, sqrt`.  
- The importance of code reuse through modules.  
- Basic idea of PyPI as a repository for third-party modules.

**💻 Example Code / Código de ejemplo:**
```python
from math import hypot

x = float(input('Cateto oposto = '))
y = float(input('Cateto adyacente = '))

# Using hypot to calculate hypotenuse
h = hypot(x, y)
print(f"La hipotenusa es: {h}")

````
**Note

At first, I wrote:

```python

h = hypot(sqrt(x**2 + y**2))  # ❌
```
But this is unnecessary and incorrect, because hypot(x, y) already calculates the square root of the sum of the squares.
So the correct and cleaner version is simply:

```python
h = hypot(x, y)  # ✅
````

**🧠 Key Insights / Reflexiones:**

- You don’t need to manually apply the Pythagorean theorem when using hypot(x, y) — Python does it for you.
- Importing only what you need from a module keeps your code clean.
- Even if you're new, trying things and reviewing results helps you understand deeper.
