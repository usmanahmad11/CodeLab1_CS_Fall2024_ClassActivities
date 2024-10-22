
# Python If-Else Examples for Beginners

## 1. Basic `if-else` Example
```python
age = int(input("Enter your age: "))

if age >= 18:
    print("You are an adult.")
else:
    print("You are not an adult.")
```
**Explanation:**  
This code asks for the user's age and prints whether they are an adult based on the input.

---

## 2. `if-elif-else` Example
```python
marks = int(input("Enter your marks: "))

if marks >= 90:
    print("Grade: A")
elif marks >= 75:
    print("Grade: B")
elif marks >= 60:
    print("Grade: C")
else:
    print("Grade: F")
```
**Explanation:**  
This code determines the grade of a student based on their marks.

---

## 3. Multiple Conditions with `and` and `or`
```python
num = int(input("Enter a number: "))

if num > 0 and num < 10:
    print("The number is a single-digit positive number.")
else:
    print("The number is either negative or has more than one digit.")
```
**Explanation:**  
Here, the code checks if the number is a positive single-digit number.

---

## 4. Checking Even or Odd
```python
number = int(input("Enter a number: "))

if number % 2 == 0:
    print(f"{number} is an even number.")
else:
    print(f"{number} is an odd number.")
```
**Explanation:**  
This program determines if the entered number is even or odd using the modulus operator.

---

## 5. Nested `if-else`
```python
number = int(input("Enter a number: "))

if number >= 0:
    if number == 0:
        print("The number is zero.")
    else:
        print("The number is positive.")
else:
    print("The number is negative.")
```
**Explanation:**  
This code checks if the number is positive, negative, or zero using nested `if-else` statements.
