## 📅 Day 11 – May 20, 2025

**✅ What I did:**
Today I learned how to use conditional structures (simple and compound) in Python. I applied this in exercises where decisions had to be made based on user input and comparisons.

**✅ What I accomplished:**
-  Learned how to use if and else to control program flow based on conditions.
-  Created a mini game where:
  - The computer generates a random number between 0 and 5.
  -  The user guesses a number.
  - The program checks if the guess matches the generated number.

**Example code:**

```python
import random
pregunta = int(input("Escribe un número entre 0 y 5:"))
numero_escogido = random.choice([0,1,2,3,4,5])
print(numero_escogido)
if pregunta == numero_escogido:
    print("¡Ganaste! El número escogido fue el mismo generado aleatoriamente.")
else:
    print("Oops, intenta nuevamente.")
```
- Understood how the indentation (tab) defines which code belongs to which conditional block.
  - No tab = always executed
  - Indented under `if` = executed only if condition is True
  - Indented under `else` = executed only if condition is False
-Identified `if` as the True block, and `else` as the False block

