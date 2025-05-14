## 📅 Day 4 - May 14, 2025

**✅ What I did:**
- Continued practicing arithmetic operations
- Solved arithmetic problems my mom gave me, such as calculating her yearly earnings based on daily income and work days per week.
- Practiced implementing real-life math problems using Python.
- Explored when to use expressions directly inside `print()` vs. assigning them to variables.

**📚 What I learned:**
- When it's better to assign operations to a variable (if reused) versus calculating directly in the `print()` function (if used only once).
- Importance of thinking ahead about the structure of the code to avoid unnecessary variables.

**💻 Example Code:**
```python
gananciadia = int(input('Ganancia por día: '))
dias = int(input('Días por semana: '))
ganancia_por_semana = gananciadia * dias
ganancia_por_año = ganancia_por_semana * 52.17

print('Si ganas {} por día y trabajas {} días a la semana, tu ganancia será: \nSEMANAL: {}\nANUAL: {}'.format(gananciadia, dias, ganancia_por_semana, ganancia_por_año))

#Note: Variable names are in Spanish because this script was originally written for my mom

# Successor example
n = int(input("Enter a number: "))
r = n + 1
print("The successor is".format(r))

# Using format for one-time operations
n = int(input("Enter a number: "))
print("The double is {}".format(n * 2))
