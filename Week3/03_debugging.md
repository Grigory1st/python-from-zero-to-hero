# Week 3: Debugging Common Issues

### UnboundLocalError
```python
x = 10
def func():
    print(x)  # Ok
    x = 5  # Error: UnboundLocalError

# Fix: Use global or different name
```

### TypeError in Functions
Wrong argument types.

### Recursion Depth
Infinite recursion.

```python
def recurse():
    recurse()  # RecursionError

# Fix: Add base case
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n-1)
```