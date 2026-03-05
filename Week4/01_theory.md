# Week 4: Data Structures

## Theory

Data structures store and organize data efficiently.

<details>
<summary>🇷🇺 Русский перевод (введение)</summary>

Структуры данных хранят и организуют данные эффективно.

</details>

### Lists
Mutable sequences.

<details>
<summary>🇷🇺 Русский перевод (Lists)</summary>

Изменяемые последовательности.

</details>

```python
fruits = ["apple", "banana"]
fruits.append("cherry")
print(fruits[0])  # apple
```

<details>
<summary>🇷🇺 Русский комментарий</summary>

```python
fruits = ["apple", "banana"]  # Помидоры
 fruits.append("cherry")  # добавить
 print(fruits[0])  # apple - первый элемент
```

</details>

### Tuples
Immutable sequences.

<details>
<summary>🇷🇺 Русский перевод (Tuples)</summary>

Неизменяемые последовательности.

</details>

```python
point = (1, 2)
```

<details>
<summary>🇷🇺 Русский комментарий</summary>

```python
point = (1, 2)  # Координаты
```

</details>

### Dictionaries
Key-value pairs.

<details>
<summary>🇷🇺 Русский перевод (Dictionaries)</summary>

Пары ключ-значение.

</details>

```python
person = {"name": "Alice", "age": 25}
print(person["name"])
```

<details>
<summary>🇷🇺 Русский комментарий</summary>

```python
person = {"name": "Alice", "age": 25}  # словарь
 print(person["name"])  # обращение по ключу
```

</details>

### Sets
Unique elements.

<details>
<summary>🇷🇺 Русский перевод (Sets)</summary>

Unique elements. (Уникальные элементы)

</details>

```python
nums = {1, 2, 3}
nums.add(4)
```

<details>
<summary>🇷🇺 Русский комментарий</summary>

```python
nums = {1, 2, 3}  # множество
 nums.add(4)  # нельзя добавить дубликаты
```

</details>

### List Comprehensions
```python
squares = [x**2 for x in range(5)]
```

<details>
<summary>🇷🇺 Русский комментарий</summary>

```python
squares = [x**2 for x in range(5)]  # квадраты [0, 1, 4, 9, 16]
```

</details>