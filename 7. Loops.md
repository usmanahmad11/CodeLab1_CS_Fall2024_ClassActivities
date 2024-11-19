
# Python Loop Exercises

A structured list of exercises to practice using `for` and `while` loops in Python, starting from basic exercises and gradually increasing in difficulty.

---

## Easy Exercises

### 1. Print Numbers from 1 to 10
Write a program that prints numbers from 1 to 10 using a `for` loop.
```python
for i in range(1, 11):
    print(i)
```

### 2. Sum of First 5 Numbers
Use a `for` loop to find and print the sum of the first 5 positive integers.
```python
total = 0
for i in range(1, 6):
    total += i
print("Sum:", total)
```

### 3. Print Each Character in a String
Ask the user to input a string and then print each character in the string on a new line using a `for` loop.
```python
text = input("Enter a string: ")
for char in text:
    print(char)
```

---

## Moderate Exercises

### 4. Count Down from a Given Number
Write a program that asks the user for a number and then counts down to zero using a `while` loop.
```python
number = int(input("Enter a number: "))
while number >= 0:
    print(number)
    number -= 1
```

### 5. Multiplication Table
Write a program that prints the multiplication table of a number entered by the user up to 10.
```python
num = int(input("Enter a number: "))
for i in range(1, 11):
    print(f"{num} x {i} = {num * i}")
```

### 6. Sum of Elements in a List
Given a list of numbers, use a `for` loop to calculate and print the sum of all elements in the list.
```python
numbers = [3, 5, 7, 9, 11]
total = 0
for num in numbers:
    total += num
print("Sum of list elements:", total)
```

### 7. Find Minimum in a List
Given a list of numbers, find and print the minimum value using a `for` loop.
```python
numbers = [12, 4, 56, 17, 8]
minimum = numbers[0]
for num in numbers:
    if num < minimum:
        minimum = num
print("Minimum value:", minimum)
```

---

## Challenging Exercises

### 8. Guess the Number Game
Write a program that generates a random number between 1 and 50, and asks the user to guess it. Continue asking until they guess correctly, providing feedback if their guess is too high or too low.
```python
import random
target = random.randint(1, 50)
guess = None
while guess != target:
    guess = int(input("Guess a number between 1 and 50: "))
    if guess < target:
        print("Too low!")
    elif guess > target:
        print("Too high!")
print("Correct! You guessed the number.")
```

### 9. Check for Prime Numbers
Write a program that takes an integer input and checks if it's a prime number.
```python
num = int(input("Enter a number: "))
is_prime = True
if num <= 1:
    is_prime = False
else:
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            is_prime = False
            break
if is_prime:
    print(f"{num} is a prime number.")
else:
    print(f"{num} is not a prime number.")
```

### 10. Factorial Calculation
Ask the user for a positive integer and calculate its factorial using a `for` loop.
```python
num = int(input("Enter a positive integer: "))
factorial = 1
for i in range(1, num + 1):
    factorial *= i
print(f"Factorial of {num} is {factorial}")
```

### 11. Calculate Average of Input Numbers
Continuously ask the user for numbers and calculate the average of those numbers. Stop the loop when the user types 'done' and print the average.
```python
total = 0
count = 0
while True:
    user_input = input("Enter a number (or type 'done' to finish): ")
    if user_input.lower() == 'done':
        break
    total += int(user_input)
    count += 1
if count > 0:
    print("Average:", total / count)
else:
    print("No numbers were entered.")
```

---

## Advanced Exercises

### 12. Find Smallest and Largest Numbers
Continuously ask the user to input numbers. Track the smallest and largest numbers entered, and stop the loop when the user types 'stop'. Print the smallest and largest numbers.
```python
smallest = None
largest = None
while True:
    user_input = input("Enter a number (or type 'stop' to end): ")
    if user_input.lower() == 'stop':
        break
    num = int(user_input)
    if smallest is None or num < smallest:
        smallest = num
    if largest is None or num > largest:
        largest = num
print("Smallest number:", smallest)
print("Largest number:", largest)
```

### 13. Fibonacci Sequence
Generate the first `n` numbers of the Fibonacci sequence, where `n` is provided by the user.
```python
n = int(input("Enter the number of Fibonacci terms: "))
a, b = 0, 1
for _ in range(n):
    print(a, end=" ")
    a, b = b, a + b
print()
```

### 14. Count the Occurrences of Each Word in a Sentence
Ask the user to input a sentence and count the occurrences of each word in the sentence.
```python
sentence = input("Enter a sentence: ")
words = sentence.split()
word_count = {}
for word in words:
    if word in word_count:
        word_count[word] += 1
    else:
        word_count[word] = 1
print("Word occurrences:", word_count)
```

---

Each exercise builds on the basics of loops and incorporates other concepts in Python. Happy coding!
