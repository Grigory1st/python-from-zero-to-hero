# Week 2: Control Flow - Conditionals and Loops

## Theory

This week, we dive into control flow, allowing your programs to make decisions and repeat actions. This is essential for automating tasks like processing lists of data or responding to user choices.

<details>
<summary>ru</summary>

На этой неделе мы погружаемся в управление потоком, позволяя вашим программам принимать решения и повторять действия. Это необходимо для автоматизации задач, таких как обработка списков данных или реагирование на выбор пользователя.

</details>

### Conditionals (if-else)
Use `if`, `elif`, and `else` to execute code based on conditions.

<details>
<summary>ru</summary>

Используйте `if`, `elif` и `else` для выполнения кода на основе условий.

</details>

```python
age = int(input("Enter your age: "))
if age >= 18:
    print("You are an adult.")
elif age >= 13:
    print("You are a teenager.")
else:
    print("You are a child.")
```

<details>
<summary>ru</summary>

```python
age = int(input("Введите ваш возраст: "))
if age >= 18:
    print("Вы взрослый.")
elif age >= 13:
    print("Вы подросток.")
else:
    print("Вы ребенок.")
```

</details>

### Comparison Operators
- `==` (equal)
- `!=` (not equal)
- `>` (greater than)
- `<` (less than)
- `>=` (greater or equal)
- `<=` (less or equal)

<details>
<summary>ru</summary>

- `==` (равенство)
- `!=` (не равно)
- `>` (больше чем)
- `<` (меньше чем)
- `>=` (больше или равно)
- `<=` (меньше или равно)

</details>

### Logical Operators
- `and`: Both conditions true
- `or`: At least one true
- `not`: Negate condition

<details>
<summary>ru</summary>

- `and`: Оба условия истинны
- `or`: По крайней мере одно истинно
- `not`: Отрицание условия

</details>

```python
is_student = True
has_id = False
if is_student and has_id:
    print("Access granted.")
```

<details>
<summary>ru</summary>

```python
is_student = True
has_id = False
if is_student and has_id:
    print("Доступ разрешен.")
```

</details>

### Loops
Loops repeat code until a condition is met.

<details>
<summary>ru</summary>

Циклы повторяют код до тех пор, пока условие выполнится.

</details>

#### While Loop
```python
count = 0
while count < 5:
    print(count)
    count += 1
```

<details>
<summary>ru</summary>

#### Цикл While
```python
count = 0
while count < 5:
    print(count)
    count += 1
```

</details>

#### For Loop
```python
for i in range(5):
    print(i)
```

<details>
<summary>ru</summary>

#### Цикл For
```python
for i in range(5):
    print(i)
```

</details>

### Loop Control
- `break`: Exit loop
- `continue`: Skip to next iteration

<details>
<summary>ru</summary>

- `break`: Выход из цикла
- `continue`: Переход к следующей итерации

</details>

```python
for num in range(10):
    if num == 5:
        break
    print(num)
```

<details>
<summary>ru</summary>

```python
for num in range(10):
    if num == 5:
        break  # Выход из цикла
    print(num)
```

</details>

These tools let you handle real-world scenarios like validating user input or iterating over data.

<details>
<summary>ru</summary>

Эти инструменты позволяют вам обрабатывать реальные сценарии, такие как валидация пользовательского ввода или итерация по данным.

</details>
