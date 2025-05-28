## 📅 Day 18 – May 28, 2025  

**✅ What I learned:**

- I completed the **first part of the course** and passed the final quiz — I can now emit my certificate.
- I started **Module 2** and studied conditional structures:
- `if` is **mandatory**
- `elif` can be used **as many times as needed**
- `else` is **optional**

**Exercise completed today:**

```
# Empréstimo bancário
import time
valor_casa = float(input("Escriba el valor de la casa: "))
salario = float(input("Escriba su salário: "))
duracion_pago = int(input("Escriba por cuantos años pagará el valor de la casa: "))
print("\033[1mCon estas informaciones analizaré el valor de prestación mensual...\033[m")
time.sleep(2)
parcelas = valor_casa / (duracion_pago * 12)

if parcelas > salario * 30/100:
    print("El valor de las parcelas excede el 30% de su salario. Su empréstimo fue negado.")
else:
    print(f"Su crédito fue aprovado. El valor de las parcelas será {parcelas}")
