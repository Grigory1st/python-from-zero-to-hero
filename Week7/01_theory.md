# Week 7: Exceptions and Debugging

## Theory

Handle errors gracefully.

<details>
<summary>🇷🇺 Обрабатывайте ошибки милостиво</summary>

Обработка исключений - критичный навык для надежного кода.

</details>

### Try-Except
```python
try:
    x = int(input())
except ValueError:
    print("Invalid number")
```

<details>
<summary>🇷🇺 Попытка-Отлов</summary>

Конструкция try-except перехватывает ошибки:

```python
try:
    x = int(input())  # Может не удаться
    print(f"Число: {x}")
except ValueError:  # Отлов от ошибки
    print("Некорректное число")
```

</details>

### Raising Exceptions
```python
if age < 0:
    raise ValueError("Age cannot be negative")
```

<details>
<summary>🇷🇺 Вызов исключений</summary>

Вы можете вызывать исключения с ключевым словом `raise`:

```python
def check_age(age):
    if age < 0:
        raise ValueError("Возраст не может быть отрицательным")
    return age
```

</details>

### Finally
Always executes.

<details>
<summary>🇷🇺 Блок Never Finally</summary>

Блок `finally` выполняется всегда, دаже при ошибке:

```python
try:
    f = open("file.txt")  # Открыть файл
    data = f.read()
except FileNotFoundError:  # если файл не найден
    print("Ошибка")
finally:  # Это сРавняется всегда
    f.close()  # Закрыть файл
```

</details>

### Debugging Tools
Use `pdb` or print statements.

<details>
<summary>🇷🇺 Инструменты отладки</summary>

Популярные инструменты:

- `pdb` - дебюгер Python
- `print()` - вывод атомов выполнения
- `assert` - проверка высказывания

</details>