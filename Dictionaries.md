
# Python Dictionary Exercises

## 1. Create and Access
- Create a dictionary to store information about a book (e.g., title, author, year published, genre).
- Access and print the value of the author.
- Update the year published to the current year.

---

## 2. Word Frequency Counter
Write a program that takes a string input from the user and:
- Splits it into words.
- Counts how many times each word appears.
- Stores the counts in a dictionary.
- Prints the dictionary.

Example:
```python
Input: "apple banana apple orange banana banana"
Output: {'apple': 2, 'banana': 3, 'orange': 1}
```

---

## 3. Convert Two Lists into a Dictionary
Given two lists:
```python
keys = ['name', 'age', 'city']
values = ['Alice', 25, 'London']
```
Write a program to combine them into a dictionary:
```python
{'name': 'Alice', 'age': 25, 'city': 'London'}
```

---

## 4. Nested Dictionary
Create a nested dictionary representing a classroom with:
- Class name as the key (e.g., "Math").
- A dictionary as the value, containing a list of student names and their average grades.

Example:
```python
{
  "Math": {"students": ["Alice", "Bob"], "average_grade": 85},
  "Science": {"students": ["Tom", "Jerry"], "average_grade": 90}
}
```

---

## 5. Invert a Dictionary
Write a function that inverts a dictionary. For example:
```python
Input: {'a': 1, 'b': 2, 'c': 1}
Output: {1: ['a', 'c'], 2: ['b']}
```

---

## 6. Find the Maximum Value
Write a program to find the key with the maximum value in a dictionary.

Example:
```python
data = {'a': 10, 'b': 30, 'c': 20}
Output: 'b'
```

---

## 7. Merge Two Dictionaries
Write a program that merges two dictionaries. If a key is present in both, add their values together.

Example:
```python
dict1 = {'a': 10, 'b': 20}
dict2 = {'b': 30, 'c': 40}
Output: {'a': 10, 'b': 50, 'c': 40}
```

---

## 8. Dictionary Comprehension
Use a dictionary comprehension to create a dictionary where keys are numbers from 1 to 10, and values are their squares.

Example:
```python
{1: 1, 2: 4, 3: 9, ..., 10: 100}
```

---

## 9. Translate Grades
Create a program that converts letter grades to GPA using a dictionary.

Example:
```python
grades = ['A', 'B', 'C', 'A', 'F']
grade_to_gpa = {'A': 4.0, 'B': 3.0, 'C': 2.0, 'D': 1.0, 'F': 0.0}
Output: [4.0, 3.0, 2.0, 4.0, 0.0]
```

---

## 10. Check for Key Existence
Write a program that:
- Prompts the user for a key.
- Checks if the key exists in the dictionary.
- If it exists, prints the value; otherwise, adds the key with a default value.
