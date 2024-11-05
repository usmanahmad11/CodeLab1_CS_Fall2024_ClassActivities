
# Python Tuples Exercises and Solutions

This document covers Python exercises related to tuples. Work through these exercises to understand tuple basics and more practical applications.

---

## Practice Exercises with Code

1. **Basic Tuple Creation**
    ```python
    # Creating a tuple
    fruits = ('apple', 'banana', 'cherry')
    print(fruits)
    print(type(fruits))

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

## Tasks with Code

1. **Employee Records**
    ```python
    # Creating employee records
    employees = [
        (101, 'Alice', 'HR', 50000),
        (102, 'Bob', 'Engineering', 75000),
        (103, 'Charlie', 'HR', 62000),
        (104, 'Diana', 'Engineering', 88000)
    ]

    # Filter employees in the HR department
    hr_employees = [emp for emp in employees if emp[2] == 'HR']
    print("HR Employees:", hr_employees)

    # Find employee with the highest salary
    highest_salary_employee = max(employees, key=lambda x: x[3])
    print("Highest Salary Employee:", highest_salary_employee)

    # Update salary of a specific employee
    employees = [(emp[0], emp[1], emp[2], emp[3] + 5000) if emp[0] == 101 else emp for emp in employees]
    print("Updated Employees:", employees)
    ```

2. **Coordinates in a Grid**
    ```python
    import math

    def calculate_distance(coord1, coord2):
        return math.sqrt((coord2[0] - coord1[0])**2 + (coord2[1] - coord1[1])**2)

    coord1 = (1, 2)
    coord2 = (4, 6)
    distance = calculate_distance(coord1, coord2)
    print("Distance between points:", distance)
    ```

3. **Tuples as Dictionary Keys**
    ```python
    # Dictionary with tuples as keys
    points = {
        (1, 1): "A",
        (2, 3): "B",
        (4, 5): "C"
    }

    # Retrieve point name by coordinates
    print(points.get((2, 3), "Point not found"))  # Output: "B"

    # Add a new point
    points[(6, 8)] = "D"
    print("Points after adding:", points)

    # Delete a point
    points.pop((1, 1), None)
    print("Points after deletion:", points)
    ```

4. **Tuple Sorting**
    ```python
    students = [
        ('Alice', 20, 85),
        ('Bob', 22, 90),
        ('Charlie', 21, 88),
        ('Diana', 20, 95)
    ]

    # Sort by name
    students_sorted_by_name = sorted(students, key=lambda x: x[0])
    print("Sorted by Name:", students_sorted_by_name)

    # Sort by age
    students_sorted_by_age = sorted(students, key=lambda x: x[1])
    print("Sorted by Age:", students_sorted_by_age)

    # Sort by grade in descending order
    students_sorted_by_grade = sorted(students, key=lambda x: x[2], reverse=True)
    print("Sorted by Grade:", students_sorted_by_grade)
    ```

5. **Product Inventory**
    ```python
    products = [
        (101, 'Laptop', 5, 1200),
        (102, 'Phone', 10, 800),
        (103, 'Tablet', 3, 600),
        (104, 'Monitor', 15, 300)
    ]

    # Product with the highest price
    most_expensive_product = max(products, key=lambda x: x[3])
    print("Most Expensive Product:", most_expensive_product)

    # Products with low quantity
    low_stock_products = [prod for prod in products if prod[2] < 5]
    print("Low Stock Products:", low_stock_products)

    # Total inventory value
    total_inventory_value = sum(prod[2] * prod[3] for prod in products)
    print("Total Inventory Value:", total_inventory_value)
    ```

---

These exercises provide hands-on experience with tuples in Python, covering immutability, indexing, tuple methods, nested tuples, dictionary keys, and sorting. Happy coding!
