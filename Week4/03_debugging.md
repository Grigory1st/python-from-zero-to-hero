# Week 4: Debugging Common Issues

<details>
<summary>🇷🇺 Русский перевод (введение)</summary>

Отладка распространенных проблем

</details>

### IndexError
Accessing out of range.

<details>
<summary>🇷🇺 Русский перевод</summary>

Обращение за пределы списка.

</details>

```python
lst = [1,2]
print(lst[2])  # IndexError

# Fix: Check len
```

<details>
<summary>🇷🇺 Русский комментарий</summary>

```python
lst = [1,2]
print(lst[2])  # IndexError - индекс 3 не существует

# Исправление: Проверьте длину
if index < len(lst):
    print(lst[index])
```

</details>

### KeyError
Invalid dict key.

<details>
<summary>🇷🇺 Русский перевод</summary>

Неверный ключ словаря.

</details>

```python
d = {"a":1}
print(d["b"])  # KeyError

# Fix: Use get()
print(d.get("b", "Not found"))
```

<details>
<summary>🇷🇺 Русский комментарий</summary>

```python
d = {"a":1}
print(d["b"])  # KeyError - ключа не существует

# Исправление: Пользуйте get()
print(d.get("b", "Not found"))  # Вернет значение по умолчанию
```

</details>

### TypeError with Sets
Sets don't support indexing.

<details>
<summary>🇷🇺 Русский перевод</summary>

Множества не поддерживают индексацию.

</details>