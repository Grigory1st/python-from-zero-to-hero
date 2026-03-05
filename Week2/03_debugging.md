# Week 2: Debugging Common Issues

<details>
<summary>ru</summary>

Неделя 2: Отладка распространенных проблем

</details>

### Infinite Loops
While loops that never end.

<details>
<summary>ru</summary>

Циклы While, которые никогда не заканчиваются.

</details>

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

<details>
<summary>ru</summary>

```python
# Ошибка
while True:
    print("Looping...")  # Никогда не останавливается

# Исправление: Добавьте условие
count = 0
while count < 10:
    print(count)
    count += 1
```

</details>

### Indentation Errors in Conditionals
```python
if True:
print("Wrong")  # IndentationError

# Fix
if True:
    print("Correct")
```

<details>
<summary>ru</summary>

```python
if True:
print("Неправильно")  # IndentationError

# Исправление
if True:
    print("Правильно")
```

</details>

### Off-by-One Errors in Loops
```python
for i in range(5):
    print(i)  # Prints 0-4, not 5
```

<details>
<summary>ru</summary>

```python
for i in range(5):
    print(i)  # Печатает 0-4, не 5
```

</details>

### Logical Errors
Conditions that don't work as expected.

<details>
<summary>ru</summary>

Условия, которые не работают как ожидалось.

</details>

```python
age = 20
if age > 18 or age < 65:  # Always true for age > 18
    print("Eligible")
```

<details>
<summary>ru</summary>

```python
age = 20
if age > 18 or age < 65:  # Всегда верно для age > 18
    print("Подходит")
```

</details>
