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

print(f'The area of the wall is {:.2f} m², you will need {:.2f} liters of paint).format(area,paint))
