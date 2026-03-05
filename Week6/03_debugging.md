# Week 6: Debugging Common Issues

### AttributeError
Accessing non-existent attribute.

```python
p = Person("Alice", 25)
print(p.height)  # AttributeError
```

<details>
<summary>ru</summary>

Эта ошибка возникает, когда вы пытаетесь получить доступ к атрибуту, который не был определен в объекте.

```python
p = Person("Алиса", 25)
print(p.height)  # AttributeError: 'Person' object has no attribute 'height'
```

Решение: убедитесь, что атрибут определен в `__init__` или используйте методы класса.

</details>

### TypeError in __init__
Wrong arguments.

<details>
<summary>ru</summary>

Эта ошибка возникает, когда при создании объекта переданы неправильные аргументы.

```python
p = Person("Алиса")  # TypeError: __init__() missing 1 required positional argument: 'age'
```

Решение: передайте все требуемые аргументы или определите значения по умолчанию.

</details>
