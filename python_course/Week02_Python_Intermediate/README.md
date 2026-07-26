# Week 2 — Control Flow & Functions 🔄

> *Make your programs think and repeat.*

---

## 🎯 Learning Objectives
- Use if/elif/else to make decisions in code
- Write for and while loops to repeat actions
- Define and call functions
- Understand scope and return values

---

## 📂 Contents

| File | Description |
|------|-------------|
| `01_Conditionals.ipynb` | if, elif, else, comparison operators, logical operators |
| `02_Loops.ipynb` | for loops, while loops, range(), break, continue |
| `03_Lists_and_Tuples.ipynb` | Creating, indexing, slicing, list methods |
| `04_Dictionaries_and_Sets.ipynb` | Key-value pairs, set operations |
| `05_Functions.ipynb` | def, parameters, return, default args, *args, **kwargs |
| `Week2_Exercises.ipynb` | Practice problems |

---

## 📖 Topics Covered

### Conditionals
```python
score = 85
if score >= 90:
    print("A")
elif score >= 75:
    print("B")
else:
    print("C")
```

### Loops
```python
# for loop
for i in range(1, 6):
    print(f"Week {i}")

# while loop
count = 0
while count < 5:
    print(count)
    count += 1
```

### Functions
```python
def greet(name, greeting="Hello"):
    return f"{greeting}, {name}!"

print(greet("Kwanda"))           # Hello, Kwanda!
print(greet("Amina", "Sannu"))   # Sannu, Amina!
```

---

## 📝 Assignment
Complete `Week2_Exercises.ipynb`.

**Key tasks:**
1. Build a simple grade calculator using conditionals
2. Write a loop that prints the multiplication table for any number
3. Create a function that checks if a number is prime
