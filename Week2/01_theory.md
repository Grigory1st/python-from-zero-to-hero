# Week 2: Control Flow - Conditionals and Loops

## Theory

This week, we dive into control flow, allowing your programs to make decisions and repeat actions. This is essential for automating tasks like processing lists of data or responding to user choices.

### Conditionals (if-else)
Use `if`, `elif`, and `else` to execute code based on conditions.

```python
age = int(input("Enter your age: "))
if age >= 18:
    print("You are an adult.")
elif age >= 13:
    print("You are a teenager.")
else:
    print("You are a child.")
```

### Comparison Operators
- `==` (equal)
- `!=` (not equal)
- `>` (greater than)
- `<` (less than)
- `>=` (greater or equal)
- `<=` (less or equal)

### Logical Operators
- `and`: Both conditions true
- `or`: At least one true
- `not`: Negate condition

```python
is_student = True
has_id = False
if is_student and has_id:
    print("Access granted.")
```

### Loops
Loops repeat code until a condition is met.

#### While Loop
```python
count = 0
while count < 5:
    print(count)
    count += 1
```

#### For Loop
```python
for i in range(5):
    print(i)
```

### Loop Control
- `break`: Exit loop
- `continue`: Skip to next iteration

```python
for num in range(10):
    if num == 5:
        break
    print(num)
```

These tools let you handle real-world scenarios like validating user input or iterating over data.