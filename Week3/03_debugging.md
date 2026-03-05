# Week 3: Debugging Common Issues

<details>
<summary>ru</summary>

Неделя 3: Отладка распространенных проблем

</details>

### UnboundLocalError
```python
x = 10
def func():
    print(x)  # Ok
    x = 5  # Error: UnboundLocalError

# Fix: Use global or different name
```

<details>
<summary>ru</summary>

```python
x = 10
def func():
    print(x)  # Нормально
    x = 5  # Ошибка: UnboundLocalError

# Исправление: Употребите global или другое имя
```

</details>

### TypeError in Functions
Wrong argument types.

<details>
<summary>ru</summary>

Неправильные типы аргументов.

</details>

### Recursion Depth
Infinite recursion.

<details>
<summary>ru</summary>

Бесконечная рекурсия.

</details>

```python
def recurse():
    recurse()  # RecursionError

# Fix: Add base case
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n-1)
```

<details>
<summary>ru</summary>

```python
def recurse():
    recurse()  # RecursionError - бесконечная петля

# Исправление: Добавьте базовый случай
def factorial(n):
    if n == 0:  # Базовый случай
        return 1
    return n * factorial(n-1)
```

</details>
