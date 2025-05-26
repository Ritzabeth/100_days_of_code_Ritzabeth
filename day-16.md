## 📅 Day 16 – May 26, 2025  

**✅ What I did:**

Today I finished watching the full ANSI escape sequences class and really got to understand how to style terminal output in Python.

**✅What I learned:**

- ANSI escape codes start with `\033[` and end with `m`.
- The final `\033[m` is used to **reset** the formatting.
- If there’s **one number** inside, it refers to **text style** (like bold or underline).
- If the number starts with **3**, it’s for **text color**.
- If it starts with **4**, it’s for the **background color**.
- You can **create a variable** to store a color/style and use it multiple times, which is cleaner and reusable.
- When inserting variables into strings with formatting, you can use `{}` inside f-strings and pass the variable in `[ ]`.

### 🧠 Reflection:

This was a fun and visual part of learning Python. It felt like adding a bit of personality to the code. As a bonus, I’m going back through all the **36 exercises** I’ve completed so far and adding **ANSI escape sequences** to make the terminal output more colorful and readable. It’s not part of the main curriculum, but it makes the learning process more fun and personal.
