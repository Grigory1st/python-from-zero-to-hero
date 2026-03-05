# Week 3: Functions

## Theory

Functions are reusable blocks of code. They help organize code and avoid repetition, crucial for larger programs.

<details>
<summary>ru</summary>

Функции - это переиспользуемые блоки кода. Они помогают организовать код и исключить повторения, что критически важно для больших программ.

</details>

### Defining Functions
```python
def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))
```

<details>
<summary>ru</summary>

```python
def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))  # Отправить привет для рим
```

</details>

### Parameters and Arguments
- Parameters: Variables in function definition.
- Arguments: Values passed to function.

<details>
<summary>ru</summary>

- Параметры: Переменные в определении функции.
- Аргументы: Значения, переданные в функцию.

</details>

```python
def add(a, b):
    return a + b

result = add(5, 3)  # 8
```

<details>
<summary>ru</summary>

```python
def add(a, b):
    return a + b

result = add(5, 3)  # 8 - Складываются 5 и 3
```

</details>

### Return Values
Functions can return values or None.

<details>
<summary>ru</summary>

Функции могут возвращать значения или None.

</details>

### Scope
Variables inside functions are local.

<details>
<summary>ru</summary>

Переменные внутри функций являются локальными.

</details>

```python
x = 10  # Global
def func():
    x = 5  # Local
    print(x)  # 5
func()
print(x)  # 10
```

<details>
<summary>ru</summary>

```python
x = 10  # Глобальная переменная
def func():
    x = 5  # Локальная переменная
    print(x)  # 5
func()
print(x)  # 10
```

</details>

### Built-in Functions
Like `len()`, `max()`, `min()`.

<details>
<summary>ru</summary>

Например `len()`, `max()`, `min()`.

</details>

### Lambda Functions
Anonymous functions.

<details>
<summary>ru</summary>

Анонимные функции.

</details>

```python
square = lambda x: x**2
print(square(4))  # 16
```

<details>
<summary>ru</summary>

```python
square = lambda x: x**2
print(square(4))  # 16 - Вычисляет 4 в квадрате
```

</details>
