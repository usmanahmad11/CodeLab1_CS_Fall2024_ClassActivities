
## 1. **Basic Line Plot**
```python
import matplotlib.pyplot as plt
import numpy as np

x = np.linspace(-10, 10, 100)
y = 2 * x + 1

plt.plot(x, y, color='blue', linewidth=2)
plt.title('Line Plot: y = 2x + 1')
plt.xlabel('X values')
plt.ylabel('Y values')
plt.grid(True)
plt.show()
```

## 2. **Multiple Lines on the Same Plot**
```python
import matplotlib.pyplot as plt
import numpy as np

x = np.linspace(-5, 5, 100)
y1 = x
y2 = x**2
y3 = x**3

plt.plot(x, y1, label='y = x', color='red')
plt.plot(x, y2, label='y = x^2', color='green')
plt.plot(x, y3, label='y = x^3', color='blue')

plt.title('Multiple Lines on Same Plot')
plt.xlabel('X values')
plt.ylabel('Y values')
plt.legend()
plt.grid()
plt.show()
```

## 3. **Bar Chart**
```python
import matplotlib.pyplot as plt

cities = ['City A', 'City B', 'City C', 'City D', 'City E']
population = [5, 7, 8, 6, 4]

plt.bar(cities, population, color='skyblue')
plt.title('Population of Cities')
plt.xlabel('Cities')
plt.ylabel('Population (in millions)')
plt.show()
```

## 4. **Scatter Plot**
```python
import matplotlib.pyplot as plt
import numpy as np

x = np.random.rand(50)
y = np.random.rand(50)

plt.scatter(x, y, color='red', marker='o')
plt.title('Scatter Plot of Random Points')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.grid()
plt.show()
```

## 5. **Pie Chart**
```python
import matplotlib.pyplot as plt

companies = ['Company A', 'Company B', 'Company C', 'Company D']
market_share = [30, 25, 25, 20]

explode = (0.1, 0, 0, 0)  # Explode the largest slice
plt.pie(market_share, labels=companies, autopct='%1.1f%%', explode=explode, shadow=True, startangle=140)
plt.title('Market Share of Companies')
plt.show()
```

## 6. **Subplots (2x2 Grid)**
```python
import matplotlib.pyplot as plt
import numpy as np

x = np.linspace(0, 10, 100)
y1 = x
y2 = np.random.rand(10)
y3 = np.random.rand(50)
y4 = np.random.randn(100)

fig, ax = plt.subplots(2, 2)

# Subplot 1: Line plot
ax[0, 0].plot(x, y1, color='blue')
ax[0, 0].set_title('Line Plot')

# Subplot 2: Bar chart
ax[0, 1].bar(range(10), y2, color='green')
ax[0, 1].set_title('Bar Chart')

# Subplot 3: Scatter plot
ax[1, 0].scatter(range(50), y3, color='red')
ax[1, 0].set_title('Scatter Plot')

# Subplot 4: Histogram
ax[1, 1].hist(y4, bins=20, color='orange')
ax[1, 1].set_title('Histogram')

plt.tight_layout()
plt.show()
```

## 7. **Histogram**
```python
import matplotlib.pyplot as plt
import numpy as np

data = np.random.normal(0, 1, 1000)  # Mean = 0, Std = 1

plt.hist(data, bins=30, color='purple', alpha=0.7)
plt.axvline(data.mean(), color='red', linestyle='dashed', linewidth=1)
plt.title('Histogram of Normally Distributed Data')
plt.xlabel('Value')
plt.ylabel('Frequency')
plt.show()
```

## 8. **Custom Line Plot: Sine Curve**
```python
import matplotlib.pyplot as plt
import numpy as np

x = np.linspace(-2 * np.pi, 2 * np.pi, 100)
y = np.sin(x)

plt.plot(x, y, color='magenta', linestyle='--', linewidth=2, marker='o', markersize=5)
plt.title('Sine Wave')
plt.xlabel('X values (radians)')
plt.ylabel('sin(x)')
plt.grid()
plt.show()
```

## 9. **Stacked Bar Chart**
```python
import matplotlib.pyplot as plt
import numpy as np

months = ['Jan', 'Feb', 'Mar']
rent = [1000, 1000, 1000]
utilities = [200, 180, 220]
food = [300, 350, 400]
transport = [150, 200, 180]

plt.bar(months, rent, label='Rent')
plt.bar(months, utilities, bottom=rent, label='Utilities')
plt.bar(months, food, bottom=np.array(rent)+np.array(utilities), label='Food')
plt.bar(months, transport, bottom=np.array(rent)+np.array(utilities)+np.array(food), label='Transport')

plt.title('Monthly Expenses')
plt.ylabel('Amount ($)')
plt.legend()
plt.show()
```

## 10. **3D Surface Plot**
```python
import matplotlib.pyplot as plt
import numpy as np
from mpl_toolkits.mplot3d import Axes3D

x = np.linspace(-5, 5, 50)
y = np.linspace(-5, 5, 50)
x, y = np.meshgrid(x, y)
z = np.sin(np.sqrt(x**2 + y**2))

fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')
ax.plot_surface(x, y, z, cmap='viridis')

ax.set_title('3D Surface Plot')
ax.set_xlabel('X-axis')
ax.set_ylabel('Y-axis')
ax.set_zlabel('Z-axis')
plt.show()
```
