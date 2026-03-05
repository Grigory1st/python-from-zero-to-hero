# Week 8: Debugging Common Issues

### Generator Exhaustion
Generators can be used only once.

<details>
<summary>ru</summary>

Если вы итеративно проходите генератор, следующий цикл не вернёт элементы — его нужно пересоздать.

```python
def gen():
    yield 1

g = gen()
print(next(g))
# print(next(g))  # StopIteration
```

</details>

### Decorator Issues
Forgetting to return wrapper.

<details>
<summary>ru</summary>

Не возвращение `wrapper` приведёт к тому, что декорируемая функция станет `None`.

</details>

### API Errors
Handle HTTP errors.

<details>
<summary>ru</summary>

Проверяйте `response.status_code` и используйте try/except для сетевых ошибок.

</details>

### SQL Injection
Use parameterized queries.

<details>
<summary>ru</summary>

Не вставляйте пользовательский ввод напрямую в SQL; используйте `?` или именованные параметры.

```python
cursor.execute("SELECT * FROM users WHERE name=?", (name,))
```

</details>
