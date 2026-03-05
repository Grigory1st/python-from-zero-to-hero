# Week 7: Exceptions and Debugging

## Theory

Handle errors gracefully.

### Try-Except
```python
try:
    x = int(input())
except ValueError:
    print("Invalid number")
```

### Raising Exceptions
```python
if age < 0:
    raise ValueError("Age cannot be negative")
```

### Finally
Always executes.

```python
try:
    f = open("file.txt")
except:
    print("Error")
finally:
    f.close()
```

### Debugging Tools
Use `pdb` or print statements.