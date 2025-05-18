# 🎓 Hackerrank:Python Program to Find Students with the Second Lowest Grade

This program reads student names and their corresponding grades, identifies the **second lowest grade**, and prints the names of all students who have that grade in **alphabetical order**.

---

## 🎯 Aim

To write a Python program to:
- Read a list of students and their grades.
- Identify the second lowest grade.
- Print the names of students who have that grade, sorted alphabetically.

---

## 🧠 Algorithm

1. **Read** an integer `n` representing the number of students.
2. **Read** each student’s name and grade, and store them as a sublist inside a list.
3. **Extract** all the grades and sort them.
4. **Identify** the second lowest grade from the sorted grade list.
5. **Collect** names of all students whose grade matches the second lowest grade.
6. **Sort** the names alphabetically.
7. **Print** each name on a new line.

---

## 💻  Program
```
n = int(input())
students = []

for _ in range(n):
    name = input()
    grade = float(input())
    students.append([name, grade])

grades = sorted(set([g for _, g in students]))
second_lowest = grades[1]

names = sorted([name for name, grade in students if grade == second_lowest])

for name in names:
    print(name)

```
## Output
![image](https://github.com/user-attachments/assets/8e9d274e-3a0b-41af-8e52-e1afb2c8964e)

## Result
Therefore the given Python program has been executed successfully and the output has been verified.

