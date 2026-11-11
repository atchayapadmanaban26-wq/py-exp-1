# Student Academic Performance Calculator

## 1. AIM
To develop a Python program that calculates a student's total marks and percentage based on the number of subjects and assigns a grade and performance level according to the percentage obtained.

## 2. ALGORITHM
1. Start the program.
2. Get the student's name as input.
3. Get the number of subjects.
4. Initialize the total marks to zero.
5. Use a `for` loop to get the marks for each subject.
6. Add each subject's marks to the total.
7. Calculate the percentage by dividing the total marks by the number of subjects.
8. Check the percentage using conditional statements (`if`, `elif`, `else`).
9. Assign the appropriate grade and performance level:
   - 90 and above – A+ (Outstanding)
   - 80 to 89 – A (Excellent)
   - 70 to 79 – B (Very Good)
   - 60 to 69 – C (Good)
   - 50 to 59 – D (Average)
   - Below 50 – F (Needs Improvement)
10. Display the student's name, total marks, percentage, and performance.
11. Stop the program.

## 3. PROGRAM

```python
name = input("enter name:")
n = int(input("enter number of subjects:"))
total = 0

for i in range(1, n+1):
    mark = float(input(f"enter mark for subjects{i}:"))
    total += mark

percentage = total / n

if percentage >= 90:
    grade = "A+"
    performance = "outstanding"
elif percentage >= 80:
    grade = "A"
    performance = "excellent"
elif percentage >= 70:
    grade = "B"
    performance = "very good"
elif percentage >= 60:
    grade = "C"
    performance = "good"
elif percentage >= 50:
    grade = "D"
    performance = "average"
else:
    grade = "F"
    performance = "needs improvement"

print("\n-----academic performance-----")
print("student name:", name)
print("total marks:", total)
print("percentage:", round(percentage, 2), "%")
print("performance:", performance)
```

## 4. OUTPUT

```text
enter name: Atchaya
enter number of subjects: 5
enter mark for subjects1: 95
enter mark for subjects2: 90
enter mark for subjects3: 85
enter mark for subjects4: 92
enter mark for subjects5: 88

-----academic performance-----
student name: Atchaya
total marks: 450.0
percentage: 90.0 %
performance: outstanding
```

## 5. RESULT

Thus, the Python program to calculate the student's total marks, percentage, grade, and academic performance using loops and conditional statements was successfully executed.
