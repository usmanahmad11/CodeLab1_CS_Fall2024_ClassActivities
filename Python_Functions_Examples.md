
# Python Functions Examples

## Example 1: Basic Function
```python
# Define a function
def greet(name):
    """
    This function greets the person whose name is passed as an argument.
    """
    return f"Hello, {name}!"

# Call the function
print(greet("Usman"))
```

## Example 2: Function with Default Arguments
```python
# Function with a default argument
def greet_with_time(name, time_of_day="morning"):
    """
    Greets the person with a specific time of day.
    """
    return f"Good {time_of_day}, {name}!"

print(greet_with_time("Usman"))
print(greet_with_time("Ahmad", "evening"))
```

## Example 3: Function with Multiple Arguments
```python
# Function to calculate the sum of two numbers
def add_numbers(a, b):
    return a + b

# Function to calculate the product of two numbers
def multiply_numbers(a, b):
    return a * b

# Calling the functions
print("Sum:", add_numbers(5, 10))
print("Product:", multiply_numbers(5, 10))
```


## Example 4: Functions Returning Multiple Values
```python
# Function to return the sum and product of two numbers
def sum_and_product(a, b):
    return a + b, a * b

# Unpacking the returned values
sum_result, product_result = sum_and_product(3, 7)
print("Sum:", sum_result)
print("Product:", product_result)
```

## Example 5: Lambda Function
```python
# Anonymous function to calculate the square of a number
square = lambda x: x ** 2
print("Square of 5:", square(5))
```
