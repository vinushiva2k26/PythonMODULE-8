# # 🔢 Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.

---

## 💻Program

```python
student_marks = {
    "Vinu": [85, 90, 88, 92, 87],
    "Ravi": [78, 80, 82, 79, 81],
    "Priya": [95, 93, 97, 96, 94]
}

total_marks = {}

for student, marks in student_marks.items():
    total_marks[student] = sum(marks)

topper = max(total_marks, key=total_marks.get)

print("Total Marks:", total_marks)
print("Topper:", topper, "-", total_marks[topper])
```

## Output

```text
Total Marks: {'Vinu': 442, 'Ravi': 400, 'Priya': 475}
Topper: Priya - 475
```

## Result

Thus, the Python program was successfully executed to calculate the total marks of students and identify the topper.
