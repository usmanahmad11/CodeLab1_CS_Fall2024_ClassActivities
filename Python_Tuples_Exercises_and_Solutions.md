
# Python Tuples Exercises and Solutions

This document covers Python exercises related to tuples. Work through these exercises to understand tuple basics and more practical applications.

---

## Practice Exercises with Code

1. **Basic Tuple Creation**
    ```python
    # Creating a tuple
    fruits = ('apple', 'banana', 'cherry')
    print(fruits)
  
    # Trying to modify the tuple (will raise an error)
    # fruits[0] = 'orange'
    ```

2. **Accessing Elements**
    ```python
    # Accessing elements by index
    print(fruits[1])  # Output: 'banana'
    print(fruits[-1])  # Output: 'cherry'
    ```

3. **Unpacking Tuples**
    ```python
    colors = ('red', 'green', 'blue')
    color1, color2, color3 = colors
    print(color1)  # Output: 'red'
    print(color2)  # Output: 'green'
    print(color3)  # Output: 'blue'
    ```

4. **Tuple Concatenation**
    ```python
    numbers1 = (1, 2, 3)
    numbers2 = (4, 5, 6)
    numbers_combined = numbers1 + numbers2
    print(numbers_combined)  # Output: (1, 2, 3, 4, 5, 6)
    ```

5. **Tuple Slicing**
    ```python
    alphabet = ('a', 'b', 'c', 'd', 'e', 'f', 'g')
    print(alphabet[:3])  # Output: ('a', 'b', 'c')
    print(alphabet[-3:])  # Output: ('e', 'f', 'g')
    print(alphabet[::2])  # Output: ('a', 'c', 'e', 'g')
    ```

6. **Tuple Methods**
    ```python
    numbers = (1, 2, 2, 3, 4, 4, 4, 5)
    print(numbers.count(4))  # Output: 3
    print(numbers.index(2))  # Output: 1
    ```

7. **Nested Tuples**
    ```python
    nested = (1, 2, (3, 4), 5)
    print(nested[2][1])  # Output: 4
    ```

8. **Tuple Membership Testing**
    ```python
    colors = ('red', 'green', 'blue')
    print('yellow' in colors)  # Output: False
    print('blue' in colors)  # Output: True
    ```

---


