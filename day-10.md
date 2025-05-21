## 📅 Day 9 – May 20, 2025

**✅ What I did:**

- Practiced string manipulation: `.upper()` and `.strip()` to clean user input.
- Learned to count letters and find their positions using `.count()`, `.find()`, and `.rfind()`.
- Solved the problem of counting how many times the letter "A" appears in a phrase, showing the first and last position (adding +1 for human-friendly indexing).
- Used `.split()` to separate a full name into a list of words.
- Deeply understood the logic behind Python indexing vs human counting:
  - Why the last index is `len(list) - 1`.
  - Difference between human counting (1, 2, 3, 4) and Python indices (0, 1, 2, 3).
- Debugged and fixed code to correctly display the first and last name.
- 
**💻 Example Code:**

```python
# Count letter A and find positions
phrase = input("Enter a phrase: ").upper().strip()
print(f"The letter 'A' appears {phrase.count('A')} times.")
print(f"The first 'A' appears at position {phrase.find('A') + 1}")
print(f"The last 'A' appears at position {phrase.rfind('A') + 1}")

# Split full name into first and last name
full_name = input("Enter your full name: ").strip()
names = full_name.split()
print(f"First name: {names[0]}")
print(f"Last name: {names[len(names) - 1]}")
````
### 🧠 Reflection:

Understanding the difference between indices and elements was a big “aha” moment today. The last index is always one less than the total elements because Python counts from zero.
