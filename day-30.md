## 📅 Day 30 – June 9, 2025

**What I did today:**

Today I forgot to study, but I decided to at least review a key concept so I wouldn’t mentally break my streak:

**🧠 Light Review: enumerate() in Python**

I learned that:

- enumerate() lets me loop through a list while getting both the index and the value at the same time, without having to write range(len(list)).

- It’s cleaner, more readable, and helps relate elements by their position in different lists.

**💻 Practical Example:**
```
animals = ["cat", "dog", "rabbit"]
for i, animal in enumerate(animals):
    print(f"Animal #{i}: {animal}")
````
📌 This is useful if I have two related lists, like names and ages, and I want to loop through both in parallel using the same index.

