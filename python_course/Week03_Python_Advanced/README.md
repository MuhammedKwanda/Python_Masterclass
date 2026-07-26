# Week 3 — Advanced Python 🔧

> *Write code like a professional.*

---

## 🎯 Learning Objectives
- Understand Object-Oriented Programming (OOP)
- Work with files and external modules
- Handle errors gracefully with exceptions
- Use list comprehensions and lambda functions

---

## 📂 Contents

| File | Description |
|------|-------------|
| `01_OOP_Basics.ipynb` | Classes, objects, __init__, methods, attributes |
| `02_OOP_Advanced.ipynb` | Inheritance, encapsulation, polymorphism |
| `03_Modules_and_Packages.ipynb` | import, pip, standard library |
| `04_File_Handling.ipynb` | Reading/writing files, CSV, JSON |
| `05_Error_Handling.ipynb` | try/except/finally, custom exceptions |
| `06_Advanced_Concepts.ipynb` | List comprehensions, lambda, map, filter |
| `Week3_Exercises.ipynb` | Practice problems |

---

## 📖 Key Concepts

### OOP — Classes & Objects
```python
class Student:
    def __init__(self, name, gpa):
        self.name = name
        self.gpa = gpa

    def introduce(self):
        return f"I'm {self.name} with a GPA of {self.gpa}"

student1 = Student("Kwanda", 9.25)
print(student1.introduce())
```

### File Handling
```python
# Writing to a file
with open("notes.txt", "w") as f:
    f.write("Python is powerful!\n")

# Reading from a file
with open("notes.txt", "r") as f:
    print(f.read())
```

### Error Handling
```python
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Cannot divide by zero!")
finally:
    print("This always runs.")
```

### List Comprehensions
```python
squares = [x**2 for x in range(10)]
evens = [x for x in range(20) if x % 2 == 0]
```

---

## 📝 Assignment
Complete `Week3_Exercises.ipynb`.

**Key tasks:**
1. Build a `BankAccount` class with deposit, withdraw, and balance methods
2. Write a script that reads a CSV file and prints its contents
3. Create a function that handles common errors gracefully
