##  Day 14 – May 24, 2025

**✅ What I did:**

- Practiced conditionals using `if`, `elif`, and `else`.
- Learned how to find the **largest** and **smallest** of three numbers with multiple `if` statements.
- Understood the logic better when using `elif`, which makes code more readable and efficient.
- Learned what a **leap year** mathematically is and how to implement the logic in Python using the `datetime` module.

### 💡 Leap Year Logic:
A year is a leap year if:
- It's divisible by **4**, and **not divisible by 100**,  
  **OR**  
- It's divisible by **400**

### 🧠 Code examples I wrote:

# Leap Year Checker

```
from datetime import date

ano = int(input("Coloque el año para calcular si es bisiesto, si es el año actual coloque '0': "))
if ano == 0:
    ano = date.today().year

if ano % 4 == 0 and ano % 100 != 0 or ano % 400 == 0:
    print(f"El año es {ano} Bisiesto")
else:
    print(f"El año {ano} no es bisiesto")
```
# Finding the largest and smallest numbers
```
a = float(input("Ingresa un número"))
b = float(input("Ingresa un número"))
c = float(input("Ingresa un número"))

menor = a
if b < c and b < a:
    menor = b
if c < a and c < b:
    menor = c

mayor = a
if b > c and b > a:
    mayor = b
if c > a and c > b:
    mayor = c

print(f"El numero mayor es: {mayor}")
print(f"El numero menor es: {menor}")
```
