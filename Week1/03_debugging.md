# Week 1: Debugging Common Issues

Debugging is a crucial skill. Here are common errors you'll encounter and how to fix them.

<details>
<summary>🇷🇺 Русский перевод (введение)</summary>

Отладка — это важный навык. Вот распространенные ошибки, которые вы встретите, и как их исправить.

</details>

### NameError

Occurs when you try to use a variable that hasn't been defined.

<details>
<summary>🇷🇺 Русский перевод (NameError)</summary>

Возникает, когда вы пытаетесь использовать переменную, которая не была определена.

</details>

```python
# Error example
print(name)  # NameError: name 'name' is not defined

# Fix: Define the variable first
name = "Alice"
print(name)
```

<details>
<summary>🇷🇺 Русский комментарий</summary>

```python
# Пример ошибки
print(name)  # NameError: name 'name' is not defined

# Исправление: Сначала определите переменную
name = "Alice"
print(name)
```

</details>

### TypeError

Happens when you try to perform an operation on incompatible types.

<details>
<summary>🇷🇺 Русский перевод (TypeError)</summary>

Происходит, когда вы пытаетесь выполнить операцию над несовместимыми типами.

</details>

```python
# Error example
age = 25
print("Age: " + age)  # TypeError: can only concatenate str (not "int") to str

# Fix: Convert to string
print("Age: " + str(age))
```

<details>
<summary>🇷🇺 Русский комментарий</summary>

```python
# Пример ошибки
age = 25
print("Age: " + age)  # TypeError: can only concatenate str (not "int") to str

# Исправление: Преобразуйте в строку
print("Age: " + str(age))
```

</details>

### SyntaxError

Invalid Python syntax.

<details>
<summary>🇷🇺 Русский перевод (SyntaxError)</summary>

Неправильный синтаксис Python.

</details>

```python
# Error example
print("Hello"  # SyntaxError: unexpected EOF while parsing

# Fix: Add closing parenthesis
print("Hello")
```

<details>
<summary>🇷🇺 Русский комментарий</summary>

```python
# Пример ошибки
print("Hello"  # SyntaxError: unexpected EOF while parsing

# Исправление: Добавьте закрывающую скобку
print("Hello")
```

</details>

### IndentationError

Python uses indentation to define code blocks.

<details>
<summary>🇷🇺 Русский перевод (IndentationError)</summary>

Python использует отступ для определения блоков кода.

</details>

```python
# Error example
if True:
print("Indented")  # IndentationError

# Fix: Indent properly
if True:
    print("Indented")
```

<details>
<summary>🇷🇺 Русский комментарий</summary>

```python
# Пример ошибки
if True:
print("Indented")  # IndentationError

# Исправление: Правильно отступите
if True:
    print("Indented")
```

</details>

### Tips
- Read error messages carefully.
- Use `print()` to debug variable values.
- Check for typos in variable names.

<details>
<summary>🇷🇺 Русский перевод (советы)</summary>

- Внимательно читайте сообщения об ошибках.
- Используйте `print()` для отладки значений переменных.
- Проверьте опечатки в названиях переменных.

</details>