
# Python Dictionaries

**Level:** UK Level 4  
**Duration:** 1.5 hours

---

## Learning Objectives
By the end of this lecture, students should be able to:
1. Define what a dictionary is in Python and understand its key-value structure.
2. Create, access, modify, and delete elements in a dictionary.
3. Apply dictionary methods and perform basic operations.
4. Utilize dictionaries in coding examples for real-world applications.

---

## Lecture Outline

### 1. Introduction to Dictionaries (10 mins)
- Explain dictionaries as a collection data type in Python.
- Highlight the key-value pair structure.
- Discuss unique keys and mutable values.
- Use a simple analogy (like a contact book) to illustrate key-value relationships.

**Code Example: Basic Dictionary**  
```python
# Example of a dictionary
student = {
    "name": "Alice",
    "age": 20,
    "courses": ["Math", "Physics"]
}
print(student)
```

### 2. Creating Dictionaries (10 mins)
- Discuss different methods to create a dictionary.
- Using curly braces `{}` or the `dict()` function.
- Mention dictionary comprehension briefly.

**Code Example: Different Ways to Create a Dictionary**  
```python
# Using curly braces
student_info = {
    "name": "Bob",
    "age": 21,
    "major": "Computer Science"
}

# Using dict function
student_info2 = dict(name="Emma", age=22, major="Biology")

print(student_info)
print(student_info2)
```

### 3. Accessing Dictionary Elements (10 mins)
- Accessing values using keys.
- The `.get()` method for safe access.

**Code Example: Accessing Values**  
```python
student = {
    "name": "Charlie",
    "age": 19,
    "major": "Physics"
}

# Accessing using key
print(student["name"])   # Output: Charlie

# Using .get() to access key safely
print(student.get("GPA", "Not Available"))  # Output: Not Available
```

### 4. Modifying Dictionary Elements (10 mins)
- Adding new key-value pairs.
- Modifying existing values.
- Removing elements using `del`, `.pop()`, and `.popitem()`.

**Code Example: Modifying a Dictionary**  
```python
student = {
    "name": "Dave",
    "age": 20,
    "major": "Chemistry"
}

# Adding a new key-value pair
student["GPA"] = 3.8

# Modifying an existing key-value pair
student["age"] = 21

# Removing a key-value pair
student.pop("major")

print(student)
```

### 5. Dictionary Methods and Operations (15 mins)
- Important dictionary methods: `.keys()`, `.values()`, `.items()`.
- Looping through dictionaries.
- Check if a key exists using `in` keyword.

**Code Example: Using Dictionary Methods**  
```python
student = {
    "name": "Eve",
    "age": 22,
    "major": "Biology"
}

# Using .keys(), .values(), and .items()
print(student.keys())    # Output: dict_keys(['name', 'age', 'major'])
print(student.values())  # Output: dict_values(['Eve', 22, 'Biology'])
print(student.items())   # Output: dict_items([('name', 'Eve'), ('age', 22), ('major', 'Biology')])

# Looping through a dictionary
for key, value in student.items():
    print(f"{key}: {value}")

# Check if a key exists
if "GPA" in student:
    print("GPA is:", student["GPA"])
else:
    print("GPA key not found")
```

### 6. Nesting Dictionaries (10 mins)
- Demonstrate how dictionaries can contain other dictionaries.
- Use an example of a school with students' details as nested dictionaries.

**Code Example: Nested Dictionary**  
```python
school = {
    "student1": {"name": "Alice", "age": 20, "GPA": 3.9},
    "student2": {"name": "Bob", "age": 21, "GPA": 3.6},
}

# Accessing nested dictionary values
print(school["student1"]["name"])  # Output: Alice
print(school["student2"]["GPA"])   # Output: 3.6
```

### 7. Real-World Application of Dictionaries (15 mins)
- Show a practical example, such as a dictionary to store product details in an e-commerce inventory.

**Code Example: E-Commerce Inventory**  
```python
inventory = {
    "item1": {"name": "Laptop", "price": 1200, "stock": 10},
    "item2": {"name": "Smartphone", "price": 800, "stock": 15},
}

# Checking stock for each item
for item_id, details in inventory.items():
    print(f"{details['name']}: ${details['price']} - {details['stock']} in stock")
```

### 8. Class Activity: Building a Contact List (15 mins)
- Have students create a simple contact book where each contact has details like name, phone number, and email stored in a dictionary.
- Example task: Add a contact, update a contact, delete a contact, and search for a contact.

**Activity Outline:**  
```python
# Starting code
contacts = {}

# Add a contact
contacts["Alice"] = {"phone": "123-456-7890", "email": "alice@example.com"}

# Allow students to expand by adding more contacts, modifying, or deleting them
```

### 9. Q&A and Recap (10 mins)
- Address any questions.
- Recap key points, especially dictionary structure, common operations, and practical use cases.

---

## Homework Assignment
- **Task:** Create a student management system using dictionaries, where students’ details (like name, age, grade) are stored. Include options for adding, updating, and deleting students.
- **Additional Challenge:** Add functionality to calculate the average grade of students using dictionary values.

---

This lecture outline covers all key aspects of Python dictionaries, from basics to real-world applications, along with interactive coding activities.
