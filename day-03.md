## 📅 Day 3 – May 13, 2025

**✅ What I did:**
- Learned and practiced all Python arithmetic operators: `+`, `-`, `*`, `/`, `**`, `//`, `%`.
- Reviewed the order of precedence in mathematical expressions.
- Built a mini-project: a script to calculate the area of a wall and the paint needed.

**📚 What I learned:**
- Addition (`+`), subtraction (`-`), multiplication (`*`), division (`/`)
- Exponentiation (`**`), floor division (`//`), modulus (`%`)
- Precedence rules: `()`, `**`, `*`, `//`, `%`, then `+`, `-`
- How an incorrect use of `**` (1/2) applies a square root and can break logic.

**💻 Example Code:**
```python
al = float(input('Height of the wall (m): '))
lar = float(input('Width of the wall (m): '))
area = al * lar
paint = area / 2

print('The area of the wall is {:.2f} m², you will need {:.2f} liters of paint).format(area,paint))

```
**Note – Update from May 14, 2025**

At the time I wrote the code above, I was following a video from a course that used the .format() method for string formatting. Since I am new to Python and didn’t realize f-strings were more modern (introduced in Python 3.6+), I used what the instructor showed.

Later, I learned that f-strings are a cleaner and more readable way to do the same thing. Here’s the updated version using f-strings instead of .format().

Updated version of my code using an f-string:

```python
print(f"The area of the wall is {area:.2f} m², you will need {paint:.2f} liters of paint.")
