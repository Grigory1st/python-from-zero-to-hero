# Week 6: Object-Oriented Programming

## Theory

OOP organizes code into classes and objects.

### Classes and Objects
```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def greet(self):
        return f"Hello, {self.name}"

p = Person("Alice", 25)
print(p.greet())
```

### Inheritance
```python
class Student(Person):
    def __init__(self, name, age, grade):
        super().__init__(name, age)
        self.grade = grade
```

### Encapsulation
Use private attributes with `_` or `__`.