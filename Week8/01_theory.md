# Week 8: Advanced Topics and Final Integration

## Theory

Wrap up with advanced concepts and project integration.

<details>
<summary>🇷🇺 Обзор продвинутых концепций и интеграции проекта</summary>

Здесь мы подведем итог изученным темам и посмотрим, как они взаимосвязаны.

</details>

### Generators
```python
def gen():
    yield 1
    yield 2

for i in gen():
    print(i)
```

<details>
<summary>🇷🇺 Генераторы</summary>

Генераторы позволяют итеративно возвращать значения, экономя память.

```python
def gen():
    yield 1
    yield 2

for i in gen():
    print(i)  # 1, затем 2
```

</details>

### Decorators
```python
def decorator(func):
    def wrapper():
        print("Before")
        func()
        print("After")
    return wrapper

@decorator
def say_hello():
    print("Hello")
```

<details>
<summary>🇷🇺 Декораторы</summary>

Декоратор — это функция, которая оборачивает другую функцию, добавляя поведение.

```python
def decorator(func):
    def wrapper():
        print("Перед")
        func()
        print("После")
    return wrapper

@decorator
def say_hello():
    print("Привет")
```

</details>

### Functional Tools
map, filter, reduce.

```python
nums = [1,2,3]
squares = list(map(lambda x: x**2, nums))
```

<details>
<summary>🇷🇺 Функциональные инструменты</summary>

`map` применяет функцию к каждому элементу, `filter` отбирает, `reduce` аккумулирует.

```python
nums = [1,2,3]
squares = list(map(lambda x: x**2, nums))  # [1,4,9]
```

</details>

### APIs with requests
```python
import requests
response = requests.get("https://api.example.com")
```

<details>
<summary>🇷🇺 API с requests</summary>

Библиотека requests делает HTTP-запросы простыми.

</details>

### SQLite Basics
```python
import sqlite3
conn = sqlite3.connect("db.db")
cursor = conn.cursor()
cursor.execute("CREATE TABLE users (id INTEGER, name TEXT)")
```

<details>
<summary>🇷🇺 Основы SQLite</summary>

SQLite — встроенная СУБД, не требующая сервера.

</details>

### Testing Basics
```python
def test_add():
    assert add(1,2) == 3
```

<details>
<summary>🇷🇺 Основы тестирования</summary>

Пишем простые unit-тесты с assert для проверки функций.

</details>