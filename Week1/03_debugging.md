# Week 1: Debugging Common Issues

Debugging is a crucial skill. Here are common errors you'll encounter and how to fix them.

### NameError
Occurs when you try to use a variable that hasn't been defined.

```python
# Error example
print(name)  # NameError: name 'name' is not defined

# Fix: Define the variable first
name = "Alice"
print(name)
```

### TypeError
Happens when you try to perform an operation on incompatible types.

```python
# Error example
age = 25
print("Age: " + age)  # TypeError: can only concatenate str (not "int") to str

# Fix: Convert to string
print("Age: " + str(age))
```

### SyntaxError
Invalid Python syntax.

```python
# Error example
print("Hello"  # SyntaxError: unexpected EOF while parsing

# Fix: Add closing parenthesis
print("Hello")
```

### IndentationError
Python uses indentation to define code blocks.

```python
# Error example
if True:
print("Indented")  # IndentationError

# Fix: Indent properly
if True:
    print("Indented")
```

### Tips
- Read error messages carefully.
- Use `print()` to debug variable values.
- Check for typos in variable names.