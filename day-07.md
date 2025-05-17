## 📅 Day 7 – May 17, 2025

**✅ What I did:**

- Finally got playing MP3 files in Python working.
- Tried the professor’s way using `pygame` and other things, but it didn’t work for me.
- Found an alternative using `playsound3` which worked.
- Learned about `random.sample` and `random.shuffle`:
  - `random.sample` when you want a shuffled list **without changing** the original.
  - `random.shuffle` when you want to **shuffle the original list** in place.

**💻 Example Code:**

```python
from playsound3 import playsound

playsound(r"C:\Users\Usuario\Downloads\gluesong.mp3")

```
**📝 Note:**

- I installed playsound3 using PyCharm, and the code worked perfectly.

- The original playsound package sometimes gives issues depending on the system, so playsound3 is a good alternative.

**🧠 Reflection:**

- Sometimes the simplest solutions aren’t the ones shown in class, so it’s good to explore alternatives.

- Understanding the difference between similar functions like random.sample and random.shuffle helps write better code.
