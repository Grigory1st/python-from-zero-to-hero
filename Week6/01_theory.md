# Week 6: Object-Oriented Programming

## Theory

OOP organizes code into classes and objects.

<details>
<summary>🇷🇺 ООП организует код в классы и объекты</summary>

Это основная парадигма программирования, которая позволяет организовать даные и функции в переиспользуемые структуры, называемые классами.

</details>

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

<details>
<summary>🇷🇺 Классы и объекты</summary>

Класс - это шаблон для создания объектов. Объект - это экземпляр класса.

```python
class Person:
    def __init__(self, name, age):
        self.name = name  # атрибут
        self.age = age

    def greet(self):
        return f"Привет, {self.name}"

p = Person("Алиса", 25)
print(p.greet())  # Привет, Алиса
```

</details>

### Inheritance
```python
class Student(Person):
    def __init__(self, name, age, grade):
        super().__init__(name, age)
        self.grade = grade
```

<details>
<summary>🇷🇺 Наследование</summary>

Наследование позволяет создавать новые классы на основе существующих. Дочерний класс наследует свойства и методы родительского класса.

```python
class Student(Person):  # Student наследует от Person
    def __init__(self, name, age, grade):
        super().__init__(name, age)  # вызов конструктора родителя
        self.grade = grade
```

</details>

### Encapsulation
Use private attributes with `_` or `__`.

<details>
<summary>🇷🇺 Инкапсуляция</summary>

Инкапсуляция скрывает внутренние детали класса. Используйте `_` для защищенных и `__` для приватных атрибутов:

```python
class BankAccount:
    def __init__(self, balance):
        self.__balance = balance  # приватный атрибут
    
    def get_balance(self):
        return self.__balance
```

</details>