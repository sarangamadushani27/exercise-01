# exercise-01
# Python Exercises Repository 

This repository contains some basic Python exercises that demonstrate different programming concepts, including lambda functions, functions, classes, and inheritance.  

## Exercises Included  

### 1. Lambda Function for Multiplication  
A simple lambda function that multiplies two numbers:  
```python
product = lambda x, y: x * y
print(product(5, 6))  # Output: 30
```

### 2. Function to Calculate Circle Area  
A function that calculates the area of a circle using the `math` module:  
```python
import math

def circle_area(radius):
    return math.pi * radius ** 2

print(circle_area(10))  # Output: 314.1592653589793
```

### 3. Simple Calculator Function  
A function that performs addition, subtraction, multiplication, and division:  
```python
def calculator(a, b, operation):
    if operation == 'a':  # Addition
        return a + b
    elif operation == 's':  # Subtraction
        return a - b
    elif operation == 'm':  # Multiplication
        return a * b
    elif operation == 'd':  # Division
        if b != 0:
            return a / b
        else:
            return "Error: Division by zero"
    else:
        return "Error: Invalid operation"

print(calculator(2, 5, 'd'))  # Output: 0.4

### 4. Rectangle Class  
A class that represents a rectangle and calculates its area:  
```python
class Rectangle:
    def __init__(self, length, width):
        self.length = length
        self.width = width

    def area(self):
        return self.length * self.width

r = Rectangle(5, 10)
print(r.area())  # Output: 50

### 5. Inheritance - Shape and Square Classes  
A base class `Shape` and a derived class `Square` that calculates the area of a square:  
```python
class Shape:
    def __init__(self, name, length):
        self.name = name
        self.length = length

    def area(self):
        return 0  # Default area for Shape

class Square(Shape):
    def __init__(self, name, length):
        super().__init__(name, length)  # Initialize parent class attributes

    def area(self):
        return self.length ** 2  # Calculate square area

    def describe(self):
        return f"This is a: {self.name}"  # Describe the shape

s = Square('square', 5)
print(f"The area is: {s.area()}")  # Output: The area is: 25
print(s.describe())  # Output: This is a: square

This repository is a collection of fundamental Python concepts like lambda functions, functions, classes, and inheritance. Each example is simple and easy to understand, making it useful for beginners learning Python.  

