# Week 5: File Handling and Modules

## Theory

Work with files and organize code into modules.

### File I/O
```python
# Write
with open("file.txt", "w") as f:
    f.write("Hello")

# Read
with open("file.txt", "r") as f:
    content = f.read()
```

### Modules
```python
import math
print(math.sqrt(16))
```

### CSV Files
```python
import csv
with open("data.csv", "r") as f:
    reader = csv.reader(f)
    for row in reader:
        print(row)
```