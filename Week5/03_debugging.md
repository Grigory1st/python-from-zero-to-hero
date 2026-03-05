# Week 5: Debugging Common Issues

<details>
<summary>ru</summary>

Отладка распространенных проблем

</details>

### FileNotFoundError
```python
open("nonexistent.txt")  # Error

# Fix: Check if exists or handle exception
```

<details>
<summary>ru</summary>

```python
open("nonexistent.txt")  # Ошибка - файл не найден

# Исправление: Проверьте если существует или обработайте исключение
```

</details>

### PermissionError
No write permission.

<details>
<summary>ru</summary>

Нет разрешения на запись.

</details>

### ImportError
Module not found.

<details>
<summary>ru</summary>

Модуль не найден.

</details>

```python
import nonexistent  # ImportError
```

<details>
<summary>ru</summary>

```python
import nonexistent  # Ошибка - модуль не тричуется
```

</details>
