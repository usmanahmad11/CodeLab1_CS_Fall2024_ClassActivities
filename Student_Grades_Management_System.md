
# Student Grades Management System

## Problem Statement
You are tasked with creating a Python program to manage student grades for a class. The program should:
1. Allow users to input student names and their grades.
2. Calculate the average grade of the class.
3. Determine the highest and lowest grades along with the respective student names.
4. Allow the user to display all student grades in a readable format.

## Solution Approach
This problem involves using basic Python concepts such as loops, lists, dictionaries, functions, and conditionals. Here's a structured approach:

---

### Steps to Solve

1. **Understand the Problem**
   - Inputs: Student names and grades.
   - Outputs:
     - Average grade of the class.
     - Student with the highest and lowest grades.
     - A display of all student names and their respective grades.

2. **Plan the Solution**
   - Use a dictionary to store student names as keys and their grades as values.
   - Implement separate functions for input, calculations, and display:
     - Input function to collect student data.
     - Calculation function for average, highest, and lowest grades.
     - Display function to print the results in a readable format.

3. **Write the Pseudo Code**

---

### Pseudo Code

```plaintext
START

FUNCTION get_student_data():
    Initialize an empty dictionary, student_grades
    WHILE True:
        Prompt user for student name (or type 'done' to finish)
        IF name is 'done':
            BREAK
        Prompt user for grade
        Validate grade is a number
        Add student name and grade to student_grades
    RETURN student_grades

FUNCTION calculate_statistics(student_grades):
    IF student_grades is empty:
        RETURN "No data available"
    Calculate average grade
    Find highest grade and corresponding student
    Find lowest grade and corresponding student
    RETURN average, highest grade, lowest grade, and respective students

FUNCTION display_results(student_grades, statistics):
    Print all students and their grades
    Print average grade
    Print highest and lowest grades along with respective students

MAIN PROGRAM:
    Call get_student_data() to get student grades
    Call calculate_statistics() with student_grades
    Call display_results() with student_grades and statistics

END
```

---

### Code Implementation

Here’s how the pseudo code translates to Python:

```python
# Function to get student data
def get_student_data():
    student_grades = {}
    while True:
        name = input("Enter student name (or type 'done' to finish): ").strip()
        if name.lower() == 'done':
            break
        try:
            grade = float(input(f"Enter grade for {name}: "))
            student_grades[name] = grade
        except ValueError:
            print("Invalid grade. Please enter a number.")
    return student_grades

# Function to calculate statistics
def calculate_statistics(student_grades):
    if not student_grades:
        return None
    
    average_grade = sum(student_grades.values()) / len(student_grades)
    highest_student = max(student_grades, key=student_grades.get)
    lowest_student = min(student_grades, key=student_grades.get)
    return {
        'average': average_grade,
        'highest': (highest_student, student_grades[highest_student]),
        'lowest': (lowest_student, student_grades[lowest_student])
    }

# Function to display results
def display_results(student_grades, statistics):
    if not student_grades:
        print("No student data to display.")
        return
    
    print("\n--- Student Grades ---")
    for student, grade in student_grades.items():
        print(f"{student}: {grade}")
    
    print("\n--- Statistics ---")
    print(f"Average Grade: {statistics['average']:.2f}")
    print(f"Highest Grade: {statistics['highest'][0]} ({statistics['highest'][1]})")
    print(f"Lowest Grade: {statistics['lowest'][0]} ({statistics['lowest'][1]})")

# Main Program
if __name__ == "__main__":
    student_grades = get_student_data()
    statistics = calculate_statistics(student_grades)
    display_results(student_grades, statistics)
```

---

### Explanation of Code
1. **`get_student_data`**:
   - Uses a `while` loop to repeatedly prompt for input.
   - Validates the grade to ensure it is a number.

2. **`calculate_statistics`**:
   - Computes average using `sum()` and `len()`.
   - Finds the highest and lowest grades using `max()` and `min()`.

3. **`display_results`**:
   - Displays all student data and the computed statistics in a user-friendly format.

4. **Main Program**:
   - Controls the overall flow by calling the functions in sequence.

---

### Sample Input and Output
#### Input:
```
Enter student name (or type 'done' to finish): Alice
Enter grade for Alice: 85
Enter student name (or type 'done' to finish): Bob
Enter grade for Bob: 90
Enter student name (or type 'done' to finish): Charlie
Enter grade for Charlie: 78
Enter student name (or type 'done' to finish): done
```

#### Output:
```
--- Student Grades ---
Alice: 85.0
Bob: 90.0
Charlie: 78.0

--- Statistics ---
Average Grade: 84.33
Highest Grade: Bob (90.0)
Lowest Grade: Charlie (78.0)
```

---

Let me know if you'd like further enhancements or a discussion on extending this case study!
