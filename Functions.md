
# Python Functions: Exercises with Solutions

## Exercise 1: Greet a User
**Objective:** Write a function that greets a user by their name.

**Code:**
```python
def greet_user(name):
    """Greets the user with their name."""
    return f"Hello, {name}! Welcome to Python programming."

# Example
print(greet_user("Usman"))
```

---

## Exercise 2: Add Two Numbers
**Objective:** Write a function to add two numbers.

**Code:**
```python
def add_numbers(num1, num2):
    """Adds two numbers and returns the result."""
    return num1 + num2

# Example
print(add_numbers(5, 10))
```

---

## Exercise 3: Check Even or Odd
**Objective:** Write a function to check whether a number is even or odd.

**Code:**
```python
def check_even_odd(number):
    """Checks if a number is even or odd."""
    return "Even" if number % 2 == 0 else "Odd"

# Example
print(check_even_odd(7))
print(check_even_odd(8))
```

---

## Exercise 4: Find the Largest Number
**Objective:** Write a function to find the largest of three numbers.

**Code:**
```python
def find_largest(num1, num2, num3):
    """Finds and returns the largest of three numbers."""
    return max(num1, num2, num3)

# Example
print(find_largest(10, 20, 15))
```

---

## Exercise 5: Calculate Factorial
**Objective:** Write a function to calculate the factorial of a number.

**Code:**
```python
def calculate_factorial(n):
    """Calculates the factorial of a number."""
    factorial = 1
    for i in range(1, n + 1):
        factorial *= i
    return factorial

# Example
print(calculate_factorial(5))
```

---

## Exercise 6: Reverse a String
**Objective:** Write a function to reverse a string.

**Code:**
```python
def reverse_string(text):
    """Reverses the input string."""
    return text[::-1]

# Example
print(reverse_string("Python"))
```

---

## Exercise 7: Check Prime Number
**Objective:** Write a function to check whether a number is prime.

**Code:**
```python
def is_prime(number):
    """Checks if a number is prime."""
    if number < 2:
        return False
    for i in range(2, int(number ** 0.5) + 1):
        if number % i == 0:
            return False
    return True

# Example
print(is_prime(7))
print(is_prime(10))
```

---

## Exercise 8: Count Vowels in a String
**Objective:** Write a function to count the number of vowels in a string.

**Code:**
```python
def count_vowels(text):
    """Counts the number of vowels in the input string."""
    vowels = "aeiouAEIOU"
    count = 0
    for char in text:
        if char in vowels:
            count += 1
    return count

# Example
print(count_vowels("I love Python programming."))
```

---

## Exercise 9: Find the Maximum in a List
**Objective:** Write a function to find the maximum number in a list.

**Code:**
```python
def find_max_in_list(numbers):
    """Finds the maximum number in a list."""
    return max(numbers)

# Example
print(find_max_in_list([3, 5, 2, 9, 1]))
```

---

## Exercise 10: Convert Temperature
**Objective:** Write a function to convert temperatures between Celsius and Fahrenheit.

**Code:**
```python
def convert_temperature(temperature, scale):
    """Converts temperature between Celsius and Fahrenheit."""
    if scale == "C":
        return (temperature * 9/5) + 32  # Celsius to Fahrenheit
    elif scale == "F":
        return (temperature - 32) * 5/9  # Fahrenheit to Celsius
    else:
        return "Invalid scale"

# Example
print(convert_temperature(0, "C"))  # Celsius to Fahrenheit
print(convert_temperature(32, "F"))  # Fahrenheit to Celsius
```
