## 📅 Day 34 – June 13, 2025

✅ What I did:
- Corrected several for and range() exercises after better understanding how their parameters work.
- Compared my solutions with the instructor's and analyzed the differences.
- Used my own logic to simplify an exercise using sum(), then reviewed the traditional version.

### 💻 Example Code Highlights:

**Even numbers up to 50**

```
# My corrected version:
for c in range(0, 52, 2):
    print(c)

# Instructor's version:
for c in range(2, 51, 2):
    print(c)
```
**Sum of odd numbers that are multiples of 3**
```
# My optimized version:
total = sum(range(3, 500, 6))
print(total)

# Instructor's traditional solution:
soma = 0
cont = 0
for c in range(1, 501, 2):
    if c % 3 == 0:
        soma += c
        cont += 1
print(f"The sum of the {cont} values is {soma}")
```
**Sum only even numbers among 6 inputs**
```
# My solution:
s = 0
for i in range(6):
    valores = int(input("Enter a number: "))
    if valores % 2 == 0:
        s += valores
print(f"The sum of the even numbers is: {s}")

# Instructor’s enriched version:
soma = 0
cont = 0
for i in range(1, 7):
    valores = int(input("Enter the {}th value: ".format(i)))
    if valores % 2 == 0:
        soma += valores
        cont += 1
print("You entered {} even numbers, and the sum is {}".format(cont, soma))
```
**First 10 terms of an arithmetic progression (AP)**
```
# My version:
first = int(input("Enter the first number of the AP: "))
step = int(input("Enter the common difference: "))
for i in range(10):
    term = first + (i * step)
    print(term)

# Instructor’s version:
first = int(input("First term: "))
step = int(input("Common difference: "))
tenth = first + (10 - 1) * step
for c in range(first, tenth + step, step):
    print(c)
```
**📚 What I learned:**
- How to better control range() behavior, especially its upper limit.

- That range(10, 0, -1) doesn’t include 0, but range(10, -1, -1) does.

- That sum(range(...)) can be a powerful and elegant solution when you understand the pattern.

- How to enrich a program with counters and formatted strings to give more information.

- That I can compare and evaluate different solutions without assuming the instructor's version is always better.
