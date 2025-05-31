## 📅 Day 20 – May 30, 2025

**✅ What I did:**

- Completed 10 exercises practicing conditionals, user input, and calculations.

- Built several small projects including:
- Loan approval based on salary and payment duration.
- BMI calculator with weight status classification.
- Payment discount and interest calculator based on payment method.
- Triangle validity and type checker.
- Age-based sports category and military enlistment eligibility.
- Rock-paper-scissors game with random computer choice and outcome messages.
- Grade average checker with pass, recovery, or fail status.

**📚 What I learned:**

- Structuring logic to validate conditions (e.g., triangle sides, game outcomes).
- Working with dates and calculating age with the datetime module.

💻 Example Code:

```
import time
import random
import datetime

# Loan approval
valor_casa = float(input("Escriba el valor de la casa: "))
salario = float(input("Escriba su salario: "))
duracion_pago = int(input("Años para pagar la casa: "))
print("\033[1mCon estas informaciones analizaré el valor de prestación mensual...\033[m")
time.sleep(2)
parcelas = valor_casa / (duracion_pago * 12)
if parcelas > salario * 0.30:
    print("El valor de las parcelas excede el 30% de su salario. Su empréstimo fue negado.")
else:
    print(f"Su crédito fue aprobado. El valor de las parcelas será {parcelas:.2f}")

# BMI Calculator
peso = float(input("Peso (kg): "))
altura = float(input("Altura (m): "))
IMC = peso / altura**2
if IMC < 18.5:
    print(f"IMC {IMC:.2f}, bajo de peso ideal")
elif 18.5 <= IMC <= 25:
    print(f"IMC {IMC:.2f}, dentro del peso ideal")
elif 25 < IMC <= 30:
    print(f"IMC {IMC:.2f}, sobrepeso")
elif 30 < IMC <= 40:
    print(f"IMC {IMC:.2f}, obesidad")
else:
    print(f"IMC {IMC:.2f}, obesidad mórbida")

# Payment Discount
valor = float(input("Valor de producto: "))
forma = input("Forma de pago: ").lower()
if forma == "efectivo":
    descuento = valor * 0.10
    print(f"Descuento {descuento:.2f}, valor total a pagar {valor - descuento:.2f}")
elif forma == "a vista":
    descuento = valor * 0.05
    print(f"Descuento {descuento:.2f}, valor total a pagar {valor - descuento:.2f}")
elif forma == "2x tarjeta":
    print(f"Sin descuento, valor total {valor:.2f}")
elif forma == "3x tarjeta":
    juros = valor * 0.20
    print(f"Juros {juros:.2f}, valor total a pagar {valor + juros:.2f}")
else:
    print("Forma de pago inválida")

# Triangle Checker
a = int(input("Primera medida: "))
b = int(input("Segunda medida: "))
c = int(input("Tercera medida: "))
if a + b > c and a + c > b and b + c > a:
    print("Estas rectas pueden formar un triángulo")
    if a == b == c:
        print("Es un triángulo equilátero")
    elif a == b or b == c or c == a:
        print("Es un triángulo isósceles")
    else:
        print("Es un triángulo escaleno")
else:
    print("Estas rectas NO pueden formar un triángulo")

# Age Sports Category
ano = int(input("Escriba su año de nacimiento: "))
edad = datetime.date.today().year - ano
if edad <= 9:
    print("CATEGORIA MIRIN")
elif 10 <= edad <= 14:
    print("CATEGORIA INFANTIL")
elif 15 <= edad <= 19:
    print("CATEGORIA JUNIOR")
elif 20 <= edad <= 20:
    print("CATEGORIA SENIOR")
else:
    print("CATEGORIA MASTER")

# Military Enlistment
ano_nac = int(input("¿En qué año naciste? "))
edad = datetime.date.today().year - ano_nac
if edad < 18:
    print("Aún no es necesario que se aliste al servicio militar")
elif edad == 18:
    print("Ya es tiempo de alistarse al servicio militar")
else:
    print("Ya pasó el tiempo de alistarse al servicio militar")

# Rock-Paper-Scissors Game
yo = input("Piedra, papel o tijera? ").lower()
computador = random.choice(['piedra', 'papel', 'tijera'])
print(f"\033[2;33mELIGIENDO...\033[m")
time.sleep(2)
print(f"Computador eligió: {computador}")

if yo == computador:
    print("EMPATE!")
elif (yo == "piedra" and computador == "tijera") or \
     (yo == "papel" and computador == "piedra") or \
     (yo == "tijera" and computador == "papel"):
    print("GANASTE!")
elif (yo == "piedra" and computador == "papel") or \
     (yo == "papel" and computador == "tijera") or \
     (yo == "tijera" and computador == "piedra"):
    print("PERDISTE!")
else:
    print("Opción inválida")

# Grade Average
nota1 = float(input("Escriba su primera nota: "))
nota2 = float(input("Escriba su segunda nota: "))
media = (nota1 + nota2) / 2
if media < 5.0:
    print(f"Tu media fue {media:.2f}, fuiste \033[1mREPROVADO\033[m")
elif 5.0 <= media <= 6.9:
    print(f"Tu media fue {media:.2f}, necesitarás entrar en \033[1mRECUPERACIÓN\033[m")
else:
    print(f"Fuiste \033[1mAPROVADO\033[m con una media de {media:.2f}")
