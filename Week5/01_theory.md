# Week 5: File Handling and Modules

## Theory

Work with files and organize code into modules.

<details>
<summary>ru</summary>

Работайте с файлами и организуйте код в модули.

</details>

### File I/O
```python
# Write
with open("file.txt", "w") as f:
    f.write("Hello")

# Read
with open("file.txt", "r") as f:
    content = f.read()
```

<details>
<summary>ru</summary>

```python
# Запись
with open("file.txt", "w") as f:
    f.write("Hello")

# Просмотр
with open("file.txt", "r") as f:
    content = f.read()
```

</details>

### Modules
```python
import math
print(math.sqrt(16))
```

<details>
<summary>ru</summary>

```python
import math  # импортируем модуль
print(math.sqrt(16))  # квадратный корень
```

</details>

### CSV Files
```python
import csv
with open("data.csv", "r") as f:
    reader = csv.reader(f)
    for row in reader:
        print(row)
```

<details>
<summary>ru</summary>

```python
import csv  # модуль для CSV
with open("data.csv", "r") as f:
    reader = csv.reader(f)  # на каждой линии строка становится списком
    for row in reader:
        print(row)
```

</details>
