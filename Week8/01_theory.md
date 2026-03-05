# Week 8: Advanced Topics and Final Integration

## Theory

Wrap up with advanced concepts and project integration.

### Generators
```python
def gen():
    yield 1
    yield 2

for i in gen():
    print(i)
```

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

### Functional Tools
map, filter, reduce.

```python
nums = [1,2,3]
squares = list(map(lambda x: x**2, nums))
```

### APIs with requests
```python
import requests
response = requests.get("https://api.example.com")
```

### SQLite Basics
```python
import sqlite3
conn = sqlite3.connect("db.db")
cursor = conn.cursor()
cursor.execute("CREATE TABLE users (id INTEGER, name TEXT)")
```

### Testing Basics
```python
def test_add():
    assert add(1,2) == 3
```