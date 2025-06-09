## 📅 Day 25 – June 4, 2025

**✅ What I did (learning with ChatGPT):**

- Learned how to use the same index i to loop through two lists at the same time (e.g., names[i] and ages[i]).
- Understood that i has no magic: it’s just a number you use as a key to access multiple aligned lists.
- Learned how to reason through a loop’s logic: it’s not about repeating things randomly.
- Started seeing the mental pattern: index → position → value → action.

**💻 Example Code:**

```
names = ["Ana", "Luis", "Carlos"]
ages = [21, 25, 30]

for i in range(len(names)):
    print(f"{names[i]} is {ages[i]} years old")
```
**📚 What I learned:**

- You can use range() with len(list) to access by index.

- Lists can be looped in parallel if they’re the same length.

- Thinking in steps helps you understand what the code is doing in each iteration.


