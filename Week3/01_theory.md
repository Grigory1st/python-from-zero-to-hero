# Week 3: Functions

## Theory

Functions are reusable blocks of code. They help organize code and avoid repetition, crucial for larger programs.

### Defining Functions
```python
def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))
```

### Parameters and Arguments
- Parameters: Variables in function definition.
- Arguments: Values passed to function.

```python
def add(a, b):
    return a + b

result = add(5, 3)  # 8
```

### Return Values
Functions can return values or None.

### Scope
Variables inside functions are local.

```python
x = 10  # Global
def func():
    x = 5  # Local
    print(x)  # 5
func()
print(x)  # 10
```

### Built-in Functions
Like `len()`, `max()`, `min()`.

### Lambda Functions
Anonymous functions.

```python
square = lambda x: x**2
print(square(4))  # 16
```