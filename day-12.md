## 📅 Day 11 – May 21, 2025

**✅ What I did:**

- 🚗 Speed Violation Fine: If the driver exceeds 80 km/h, a fine is applied — R$7.00 for each km above the limit.

```python
velocidad = float(input("Velocidad en km/h:"))
if velocidad > 80:
    print("Por exceder el límite de velocidad, estás multado")
    multa = (velocidad - 80) * 7
    print(f"La multa total será {multa}")
else:
    print()
```

- 🔢 Even or Odd: This program checks if a number is even or odd using the modulo operator (%).

```python
num = int(input("Escriba un numero entero:"))
if num % 2 == 0:
    print("Su número es par")
else:
    print("Su número es impar")
```
- 🛣️ Distance-Based Ticket Pricing: Price depends on the length of the trip:
  - ≤ 200 km: R$0.50/km
  - 200 km: R$0.45/km

```
distancia = float(input("Escriba la distancia recorrida en KM"))
if distancia <= 200:
    costo = distancia * 0.50
    print(f"El precio total será {costo:.2f}")
else:
    costo = distancia * 0.45
    print(f"El precio total será {costo:.2f}")
```
- 🧪 Attempted (Needs Fixing): Find the Largest and Smallest Number. **I tried this:**
```
num1 = float(input("Ingresa un número"))
num2 = float(input("Ingresa un número"))
num3 = float(input("Ingresa un número"))
if num1 > num2 > num3:
  print(f"El número mayor es: {num1:.0f}")
  print(f"El número menor es: {num3:.0f}")
else:
  print(f"El número mayor es: {num3:.0f}")
  print(f"El número menor es: {num1:.0f}")
```
But this logic only works if the numbers are in exact descending order. If not, it gives wrong results — for example, even if num3 is not the highest, it prints it as the max.
✅ I will rewrite this logic properly on my next session.
