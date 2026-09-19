# Module 6 — Complete Reader

This document contains the complete read-only summary of all files currently present in the repository. It is formatted for easy reading and PDF export.

---

# 1. Abstraction

## 🎯 AIM
To create an abstract class named `Shape` with an abstract method `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

## 🧠 ALGORITHM
1. Import the `ABC` module.
2. Create an abstract class `Shape` with an abstract method `calculate_area()`.
3. Create subclass `Rectangle` with length and breadth values and override `calculate_area()`.
4. Create subclass `Circle` with radius and override `calculate_area()`.
5. Instantiate both classes and print their results.

## 💻 Program
```python
from abc import ABC
class Shape(ABC):
    def calculate_area(self):
        pass
class Rectangle(Shape):
    length = 5
    breadth = 3
    def calculate_area(self):
        return self.length * self.breadth

class Circle(Shape):
    radius = 4
    def calculate_area(self):
        return self.radius * self.radius * 3.14

rec = Rectangle()
cir = Circle()

print("Area of a rectangle:", rec.calculate_area())
print("Area of a circle:", cir.calculate_area())
```

## Output
<img width="598" height="171" alt="image" src="https://github.com/user-attachments/assets/7bce4c5d-3f24-4661-8522-bdc72c394ad8" />

## Result
Thus, the program has been successfully executed.

---

# 2. Encapsulation

## 🎯 AIM
To implement encapsulation in Python by defining a class `Rectangle` with private member variables `__length` and `__breadth`.

## 🧠 ALGORITHM
1. Define the class `Rectangle`.
2. Use private attributes `__length` and `__breadth`.
3. Initialize them in the constructor.
4. Display the private values from within the class.
5. Instantiate the class to show encapsulation.

## 💻 Program
```python
class Rectangle:
    def __init__(self, length, breadth):
        self.__length = length
        self.__breadth = breadth

    def display(self):
        print("Length:", self.__length)
        print("Breadth:", self.__breadth)

r = Rectangle(5, 3)
r.display()
```

## Output
(Blank in the repository file; this section represents the intended result of the program.)

## Result
The concept of encapsulation is demonstrated successfully.

---

# 3. Method Overriding

## 🧠 AIM
To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

## 📋 ALGORITHM
1. Define the `Fish` class with a method named `type()` that prints `"fish"`.
2. Define the `Shark` class as a subclass of `Fish`, and override the `type()` method to print `"shark"`.
3. Create an instance of `Fish` and an instance of `Shark`.
4. Call both methods and show the overridden behavior.

## 💻 PROGRAM
```python
class Fish:
    def type(self):
        print("fish")

class Shark:
    def type(self):
        print("shark")

obj_goldfish = Fish()
obj_hammerhead = Shark()

obj_goldfish.type()
obj_hammerhead.type()
```

## OUTPUT
<img width="839" height="289" alt="image" src="https://github.com/user-attachments/assets/4352198c-8aa7-4785-99ac-8a2ac652becc" />

## RESULT
Thus, the program is executed successfully.

---

# 4. Operator Overloading (Less Than `<`)

## 🎯 AIM
To write a Python program that demonstrates operator overloading by overloading the less than (`<`) operator using a custom class.

## 🧠 ALGORITHM
1. Create a class `A`.
2. Define the `__init__()` method to set the value `a`.
3. Define the `__lt__()` method.
4. Create two objects and compare them using `<`.
5. Print the respective message depending on their values.

## 💻 Program
```python
class A:
    def __init__(self, a):
        self.a = a

    def __lt__(self, other):
        return self.a < other.a

ob1 = A(200)
ob2 = A(30)

if(ob1 < ob2):
    print("ob1 is less than ob2")
else:
    print("ob2 is less than ob1")
```

## Output
<img width="1177" height="268" alt="image" src="https://github.com/user-attachments/assets/04136876-d58a-4afe-bf71-f1c5a618fd17" />

## Result
Thus, the program is executed successfully.

---

# 5. Polymorphism with Classes

This file appears to contain the same content as the operator-overloading exercise and demonstrates the same OOP concept using the less-than operator.

## Summary
The repository includes multiple examples of object-oriented programming, specifically:
- abstraction
- encapsulation
- method overriding
- operator overloading
- polymorphism-style class behavior

---

# Conclusion
Module 6 covers several core object-oriented programming concepts in Python. This reader compiles the main exercise files into one document for easier study and PDF export.
