# Week 7: Debugging Common Issues

### Broad Except
Catching all exceptions hides bugs.

```python
try:
    # code
except:  # Bad
    pass
```

<details>
<summary>ru</summary>

Проблема: баре `except:` ловит все исключения, большие части маскируют основные ошибки.

Совет: специфическо укажите типы исключений:

```python
try:
    # код
except ValueError:  # ЛУЧШЕ
    pass
```

</details>

### Not Raising Appropriate Exceptions
Use built-in or custom.

<details>
<summary>ru</summary>

Проблема: ѓсли в коде есть недействительные данные, вызвовите аппроприатное исключение.

Совет:

```python
if not isinstance(value, int):
    raise TypeError("Ожидался целое число")
```

</details>

### Finally Not Used for Cleanup
Use finally for resources.

<details>
<summary>ru</summary>

Проблема: ресурсы (dbfile, соединения базы данных, файлы) не чистятся исправно.

Совет: всегда используйте finally:

```python
f = None
try:
    f = open("file.txt")
except FileNotFoundError:
    print("Ошибка")
finally:
    if f:
        f.close()  # Гарантированно закрыётся
```

</details>
