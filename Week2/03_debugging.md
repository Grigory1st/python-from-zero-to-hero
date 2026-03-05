# Week 2: Debugging Common Issues

### Infinite Loops
While loops that never end.

```python
# Error
while True:
    print("Looping...")  # Never stops

# Fix: Add condition
count = 0
while count < 10:
    print(count)
    count += 1
```

### Indentation Errors in Conditionals
```python
if True:
print("Wrong")  # IndentationError

# Fix
if True:
    print("Correct")
```

### Off-by-One Errors in Loops
```python
for i in range(5):
    print(i)  # Prints 0-4, not 5
```

### Logical Errors
Conditions that don't work as expected.

```python
age = 20
if age > 18 or age < 65:  # Always true for age > 18
    print("Eligible")
```