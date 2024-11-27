
# Python Dictionary Exercises

## Exercise 1: Create and Access a Dictionary
**Task**: Create a dictionary called `student` with the following key-value pairs:
- Name: "Alice"
- Age: 24
- Major: "Computer Science"

Then, access and print:
1. The value of the "Name" key.
2. The value of the "Major" key.

**Solution**:
```python
# Creating the dictionary
student = {
    "Name": "Alice",
    "Age": 24,
    "Major": "Computer Science"
}

# Accessing and printing values
print("Name:", student["Name"])
print("Major:", student["Major"])
```

---

## Exercise 2: Add and Update Values
**Task**:
1. Add a new key-value pair to the `student` dictionary: `GPA: 3.8`.
2. Update the `Age` key to 25.

**Solution**:
```python
# Adding a new key-value pair
student["GPA"] = 3.8

# Updating the Age
student["Age"] = 25

# Printing the updated dictionary
print(student)
```

---

## Exercise 3: Loop Through a Dictionary
**Task**: Loop through the `student` dictionary and print each key-value pair in the format:
`Key: Value`.

**Solution**:
```python
for key, value in student.items():
    print(f"{key}: {value}")
```

---

## Exercise 4: Check if a Key Exists
**Task**: Write a function `check_key(dictionary, key)` that checks if a given key exists in a dictionary. Return `"Key exists"` if it does, otherwise `"Key does not exist"`.

**Solution**:
```python
def check_key(dictionary, key):
    if key in dictionary:
        return "Key exists"
    else:
        return "Key does not exist"

# Testing the function
print(check_key(student, "Name"))  # Output: Key exists
print(check_key(student, "Hobbies"))  # Output: Key does not exist
```

---

## Exercise 5: Count Occurrences
**Task**: Given a list of words, count the frequency of each word using a dictionary.

**Input**: `["apple", "banana", "apple", "orange", "banana", "apple"]`  
**Output**: `{"apple": 3, "banana": 2, "orange": 1}`

**Solution**:
```python
words = ["apple", "banana", "apple", "orange", "banana", "apple"]
word_count = {}

for word in words:
    if word in word_count:
        word_count[word] += 1
    else:
        word_count[word] = 1

print(word_count)
```

---

## Exercise 6: Merge Two Dictionaries
**Task**: Merge the following dictionaries into one:
- `dict1 = {"a": 1, "b": 2}`
- `dict2 = {"b": 3, "c": 4}`

**Expected Output**: `{'a': 1, 'b': 3, 'c': 4}`

**Solution**:
```python
dict1 = {"a": 1, "b": 2}
dict2 = {"b": 3, "c": 4}

# Merging dictionaries
merged_dict = {**dict1, **dict2}
print(merged_dict)
```

---

## Exercise 7: Remove Keys
**Task**: Remove the key `Age` from the `student` dictionary.

**Solution**:
```python
# Removing a key
student.pop("Age", None)  # Using pop with a default value to avoid KeyError if the key doesn't exist

# Printing the updated dictionary
print(student)
```

---

## Exercise 8: Nested Dictionaries
**Task**: Create a dictionary `classroom` with two students' data as nested dictionaries:
- Student1: Name: "John", Age: 20
- Student2: Name: "Emma", Age: 22

Access and print:
1. The name of Student2.
2. The age of Student1.

**Solution**:
```python
classroom = {
    "Student1": {"Name": "John", "Age": 20},
    "Student2": {"Name": "Emma", "Age": 22}
}

# Accessing values
print("Student2 Name:", classroom["Student2"]["Name"])
print("Student1 Age:", classroom["Student1"]["Age"])
```

---

## Exercise 9: Sort a Dictionary
**Task**: Sort the dictionary `{"z": 10, "b": 5, "a": 15}` by keys and values.

**Solution**:
```python
# Dictionary to sort
data = {"z": 10, "b": 5, "a": 15}

# Sorting by keys
sorted_by_keys = dict(sorted(data.items()))
print("Sorted by keys:", sorted_by_keys)

# Sorting by values
sorted_by_values = dict(sorted(data.items(), key=lambda item: item[1]))
print("Sorted by values:", sorted_by_values)
```

---

## Exercise 10: Dictionary Comprehension
**Task**: Create a dictionary where the keys are numbers from 1 to 5, and the values are their squares.

**Solution**:
```python
squares = {x: x**2 for x in range(1, 6)}
print(squares)
```
