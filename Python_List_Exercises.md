
# Python List Exercises with Solutions

These exercises cover basic list operations in Python, including creating lists, accessing elements, manipulating lists, and simple algorithms using lists.

---

## Exercise 1: Create a List
**Task:** Create a list called `fruits` that contains the following elements: `"apple"`, `"banana"`, `"cherry"`, `"date"`. Print the list.

**Solution:**
```python
# Solution
fruits = ["apple", "banana", "cherry", "date"]
print(fruits)
```

---

## Exercise 2: Access List Elements
**Task:** Given a list `numbers = [10, 20, 30, 40, 50]`, print the first and last elements.

**Solution:**
```python
# Solution
numbers = [10, 20, 30, 40, 50]
print("First element:", numbers[0])
print("Last element:", numbers[-1])
```

---

## Exercise 3: Update List Element
**Task:** Replace the second element of the list `animals = ["cat", "dog", "bird"]` with `"hamster"`. Print the updated list.

**Solution:**
```python
# Solution
animals = ["cat", "dog", "bird"]
animals[1] = "hamster"
print(animals)
```

---

## Exercise 4: Append and Remove Elements
**Task:** Start with an empty list called `colors`.
1. Add `"red"`, `"green"`, and `"blue"` to the list.
2. Then, remove `"green"` from the list.
3. Print the final list.

**Solution:**
```python
# Solution
colors = []
colors.append("red")
colors.append("green")
colors.append("blue")
colors.remove("green")
print(colors)
```

---

## Exercise 5: List Length
**Task:** Write a program that finds and prints the length of the list `names = ["Alice", "Bob", "Charlie", "Diana"]`.

**Solution:**
```python
# Solution
names = ["Alice", "Bob", "Charlie", "Diana"]
print("Length of the list:", len(names))
```

---

## Exercise 6: Sum of List Elements
**Task:** Given a list `numbers = [4, 7, 1, 8, 5]`, find and print the sum of all elements in the list.

**Solution:**
```python
# Solution
numbers = [4, 7, 1, 8, 5]
total_sum = sum(numbers)
print("Sum of elements:", total_sum)
```

---

## Exercise 7: Find Maximum and Minimum Elements
**Task:** Using the list `ages = [23, 45, 18, 34, 60]`, find and print the maximum and minimum values.

**Solution:**
```python
# Solution
ages = [23, 45, 18, 34, 60]
print("Maximum age:", max(ages))
print("Minimum age:", min(ages))
```

---

## Exercise 8: Sort a List
**Task:** Sort the list `scores = [88, 56, 92, 78, 61]` in ascending order and print the sorted list.

**Solution:**
```python
# Solution
scores = [88, 56, 92, 78, 61]
scores.sort()
print("Sorted list:", scores)
```

---

## Exercise 9: Check if Element Exists in List
**Task:** Write a program that checks if the value `5` is in the list `numbers = [1, 3, 5, 7, 9]`. Print `"Found"` if it is, otherwise print `"Not Found"`.

**Solution:**
```python
# Solution
numbers = [1, 3, 5, 7, 9]
if 5 in numbers:
    print("Found")
else:
    print("Not Found")
```

---

## Exercise 10: Count Occurrences of an Element
**Task:** Given a list `items = [1, 2, 2, 3, 4, 4, 4, 5]`, count and print how many times `4` appears in the list.

**Solution:**
```python
# Solution
items = [1, 2, 2, 3, 4, 4, 4, 5]
count_of_4 = items.count(4)
print("Count of 4:", count_of_4)
```

---

These exercises provide a solid foundation for learning list operations in Python. If you'd like more advanced exercises, feel free to ask!
